# GitHub Setup: Deploying to Google Cloud Run

This guide explains how to configure GitHub for the Cloud Run deployment workflows in this repo. It covers the four jobs that failed for you:

- Deploy Frontend to Cloud RUN (`.github/workflows/gcp_frontend.yml`)
- Deploy Personas to Cloud RUN (`.github/workflows/gcp_personas.yml`)
- Deploy Plugins to Cloud RUN (`.github/workflows/gcp_plugins.yml`)
- Deploy Apps-Js to Cloud RUN (`.github/workflows/gcp_apps_js.yml`)

If a job fails in ~10–20 seconds, it’s almost always missing/invalid GitHub Secrets or Variables.

---

## 1) Prerequisites (Google Cloud)

In your GCP project:

1. Enable required APIs
   - Cloud Run Admin API
   - Cloud Build API
   - Container Registry API (for `gcr.io`) or Artifact Registry API (if you change to `us-docker.pkg.dev`)
   - IAM Service Account Credentials API

2. Create a service account for GitHub Actions (example: `github-deployer@<PROJECT_ID>.iam.gserviceaccount.com`).

3. Grant roles to that service account
   - Cloud Run Admin: `roles/run.admin`
   - Service Account User: `roles/iam.serviceAccountUser`
   - Storage Admin (for pushing images to `gcr.io`): `roles/storage.admin`

4. Create and download a JSON key for this service account. You will paste its JSON content into a GitHub Secret in step 3 below.

Note: The workflows currently use a JSON key (`credentials_json`). You can later migrate to OIDC (Workload Identity Federation) if you prefer keyless auth.

---

## 2) Create GitHub Environments

These workflows automatically select an environment based on the branch:

- `main` branch → environment: `prod`
- `development` branch → environment: `development`

In GitHub:

1. Go to: Settings → Environments → New environment.
2. Create two environments named exactly: `development` and `prod`.
3. (Optional) Add protection rules or reviewers if you want gated deployments.

You can store Variables/Secrets at the environment level so `prod` and `development` can differ.

---

## 3) Add GitHub Variables and Secrets

Go to: Settings → Secrets and variables → Actions.

You’ll add one Repository Variable and a set of Secrets (prefer environment‑scoped under `development` and `prod`).

### 3.1 Repository Variables

- Variable: `GCP_PROJECT_ID` → set to your Google Cloud project ID (e.g., `my-project-123`).

This is referenced by the workflows as `vars.GCP_PROJECT_ID`.

### 3.2 Required Secrets (all workflows)

- Secret: `GCP_CREDENTIALS` → paste the full JSON key you downloaded for the GitHub deployer service account.

Used by: `.github/workflows/gcp_frontend.yml`, `.github/workflows/gcp_personas.yml`, `.github/workflows/gcp_plugins.yml`, `.github/workflows/gcp_apps_js.yml`.

Add this secret at least at the repository level. If you prefer per‑environment separation, add it to both environments (`development` and `prod`).

### 3.3 Frontend secrets

Workflow: `.github/workflows/gcp_frontend.yml` (service `frontend`)

Add these secrets (environment‑scoped recommended):

- `NEXT_PUBLIC_FIREBASE_API_KEY`
- `NEXT_PUBLIC_FIREBASE_AUTH_DOMAIN`
- `NEXT_PUBLIC_FIREBASE_PROJECT_ID`
- `NEXT_PUBLIC_FIREBASE_STORAGE_BUCKET`
- `NEXT_PUBLIC_FIREBASE_MESSAGING_SENDER_ID`
- `NEXT_PUBLIC_FIREBASE_APP_ID`
- `NEXT_PUBLIC_FIREBASE_MEASUREMENT_ID`

Where to get them: Firebase Console → Project settings → Your apps → Web app config.

### 3.4 Personas secrets

Workflow: `.github/workflows/gcp_personas.yml` (service `omi-web`)

Add as applicable (environment‑scoped recommended):

- `NEXT_PUBLIC_FIREBASE_API_KEY`
- `NEXT_PUBLIC_FIREBASE_AUTH_DOMAIN`
- `NEXT_PUBLIC_FIREBASE_PROJECT_ID`
- `NEXT_PUBLIC_FIREBASE_STORAGE_BUCKET`
- `NEXT_PUBLIC_FIREBASE_MESSAGING_SENDER_ID`
- `NEXT_PUBLIC_FIREBASE_APP_ID`
- `NEXT_PUBLIC_FIREBASE_VAPID_KEY` (Firebase Web Push if you use notifications)
- `NEXT_PUBLIC_RAPIDAPI_KEY` (if you use RapidAPI integrations)
- `NEXT_PUBLIC_RAPIDAPI_HOST`
- `NEXT_PUBLIC_LINKEDIN_API_KEY` (if you use LinkedIn integrations)
- `NEXT_PUBLIC_LINKEDIN_API_HOST`
- `OPENROUTER_API_KEY` (if using OpenRouter)
- `CLAUDE_API_KEY` (if using Anthropic Claude)
- `NEXT_PUBLIC_MIXPANEL_TOKEN` (analytics, if used)
- `NEXT_PUBLIC_EXTRA_PROMPT_RULES` (optional text to inject into prompts)

Add only the ones you need; however, missing required build args may cause build failures depending on code paths.

### 3.5 Plugins secrets

Workflow: `.github/workflows/gcp_plugins.yml` (service `plugins`)

No app‑specific secrets are required by default. You still need:

- `GCP_CREDENTIALS` (see above)
- `GCP_PROJECT_ID` variable

### 3.6 Apps‑Js secrets

Workflow: `.github/workflows/gcp_apps_js.yml` (service `apps-js`)

Add the following (use environment scope if you want different values for `development` and `prod`):

- `OPENAI_API_KEY`
- `OPENROUTER_API_KEY`
- `UPSTASH_REDIS_HOST`
- `UPSTASH_REDIS_PASSWORD`
- `UPSTASH_REDIS_PORT`
- `JWT_SECRET`
- `GOOGLE_CLIENT_ID`
- `GOOGLE_CLIENT_SECRET`
- `GOOGLE_REDIRECT_URI` (matches your OAuth consent redirect)
- `GOOGLE_CALLBACK_URL` (if your app expects a different callback path)
- `BASE_URL` (public URL the service will run at)
- `SUPABASE_URL`
- `SUPABASE_KEY`
- `OMI_APP_ID`
- `OMI_APP_SECRET`
- `DECK_APP_ID`
- `DECK_APP_SECRET`
- `SLIDESGPT_API_KEY`

Notes:
- Exact values depend on your third‑party providers (Google OAuth, Upstash, Supabase, etc.).
- If some features aren’t used, you may omit their keys, but ensure the Docker build and runtime don’t expect them unconditionally.

---

## 4) Region and Service Names

Each workflow sets `REGION: us-central1` and the service name via `SERVICE`. If you need a different region or service name, edit the workflow files:

- Frontend: `.github/workflows/gcp_frontend.yml`
- Personas: `.github/workflows/gcp_personas.yml`
- Plugins: `.github/workflows/gcp_plugins.yml`
- Apps-Js: `.github/workflows/gcp_apps_js.yml`

The first deploy will create the Cloud Run service if it doesn’t exist (permissions allowing).

---

## 5) Trigger a Deployment

You can deploy in two ways:

- Push to `main` (targets `prod`) or `development` (targets `development`) touching the relevant folder:
  - Frontend → changes under `web/frontend/**`
  - Personas → changes under `web/personas-open-source/**`
  - Plugins → changes under `plugins/example/**`
  - Apps‑Js → changes under `plugins/apps-js/**`

- Manually trigger via Actions → select the workflow → “Run workflow”. Some workflows let you specify a branch.

When it finishes, GitHub will print the Cloud Run URL.

---

## 6) Common Failures and Fixes

- Fails in ~10–20s at Google Auth
  - Missing/invalid `GCP_CREDENTIALS` secret. Paste the exact JSON from the service account you created.
  - `GCP_PROJECT_ID` variable missing or wrong.
  - GCP APIs not enabled or SA lacks `run.admin` / `storage.admin`.

- Docker push errors to `gcr.io`
  - Ensure Container Registry API enabled and the SA has `roles/storage.admin`.
  - If you switch to Artifact Registry, update image URLs and grant `roles/artifactregistry.writer` instead.

- Deploy to Cloud Run permission denied
  - SA needs `roles/run.admin` and often `roles/iam.serviceAccountUser`.

- Lint job fails (not deployment related)
  - Run locally: `cd web/frontend && npm ci && npm run lint && npm run lint:format -- --check`
  - Fix ESLint/Prettier errors, commit, and push. See `.github/workflows/lint.yml`.

---

## 7) Optional: Keyless Auth with OIDC (Advanced)

For better security, you can remove JSON keys and use GitHub OIDC (Workload Identity Federation):

1. In GCP IAM, create a Workload Identity Pool and Provider trusted with `token.actions.githubusercontent.com`.
2. Grant your GitHub repo (`repo: <owner>/<repo>`) permission to impersonate the deployer service account.
3. Update the workflows to use:

```yaml
- uses: google-github-actions/auth@v2
  with:
    workload_identity_provider: "projects/<NUM>/locations/global/workloadIdentityPools/<POOL>/providers/<PROVIDER>"
    service_account: "github-deployer@<PROJECT_ID>.iam.gserviceaccount.com"
```

4. Remove `credentials_json` usage and the `GCP_CREDENTIALS` secret.

Only do this once deployments work with the JSON key method.

---

## 8) Where Things Live (for reference)

- Frontend workflow: `.github/workflows/gcp_frontend.yml`
- Personas workflow: `.github/workflows/gcp_personas.yml`
- Plugins workflow: `.github/workflows/gcp_plugins.yml`
- Apps‑Js workflow: `.github/workflows/gcp_apps_js.yml`
- Lint workflow: `.github/workflows/lint.yml`

If you need help wiring any specific provider (Firebase, Google OAuth, Upstash, Supabase, etc.), create an issue with what you’re trying to deploy and which secrets you’re missing.

