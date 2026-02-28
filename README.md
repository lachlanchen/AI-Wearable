[English](README.md) · [العربية](i18n/README.ar.md) · [Español](i18n/README.es.md) · [Français](i18n/README.fr.md) · [日本語](i18n/README.ja.md) · [한국어](i18n/README.ko.md) · [Tiếng Việt](i18n/README.vi.md) · [中文 (简体)](i18n/README.zh-Hans.md) · [中文（繁體）](i18n/README.zh-Hant.md) · [Deutsch](i18n/README.de.md) · [Русский](i18n/README.ru.md)


[![LazyingArt banner](https://github.com/lachlanchen/lachlanchen/raw/main/figs/banner.png)](https://github.com/lachlanchen/lachlanchen/blob/main/figs/banner.png)

<div align="center">

# **omi**

_AI-powered wearable for instant meetings and chats: capture, summarize, and act—hands-free._

Meet Omi, the world’s leading open-source AI wearable that captures conversations, gives summaries, action items and does actions for you. Simply connect Omi to your mobile device and enjoy automatic, high-quality transcriptions of meetings, chats, and voice memos wherever you are.

<p align="center">
  <img src="https://github.com/user-attachments/assets/834d3fdb-31b5-4f22-ae35-da3d2b9a8f59" alt="Omi" width="49%" />
  <img src="https://github.com/user-attachments/assets/fdad4226-e5ce-4c55-b547-9101edfa3203" alt="Image" width="49%" />
</p>

![CleanShot 2025-02-08 at 18 22 23](https://github.com/user-attachments/assets/7a658366-9e02-4057-bde5-a510e1f0217a)

[![Discord Follow](https://img.shields.io/discord/1192313062041067520?label=Discord&color=5865F2)](http://discord.omi.me)
[![Twitter Follow](https://img.shields.io/twitter/follow/kodjima33?color=1DA1F2)](https://x.com/kodjima33)
[![License: MIT](https://img.shields.io/badge/License-MIT-ffd43b.svg)](https://opensource.org/licenses/MIT)
[![GitHub Repo stars](https://img.shields.io/github/stars/BasedHardware/Omi?color=f5b301)](https://github.com/BasedHardware/Omi)
[![Monorepo](https://img.shields.io/badge/Repo-Monorepo-2ea44f)](https://github.com/BasedHardware/Omi)
[![Docs](https://img.shields.io/badge/docs-omi.me-0ea5e9)](https://docs.omi.me/)
[![GitHub release](https://img.shields.io/github/v/release/BasedHardware/Omi?color=0ea5e9&style=flat-square)](https://github.com/BasedHardware/Omi/releases)
[![GitHub issues](https://img.shields.io/github/issues/BasedHardware/Omi?color=ef4444&style=flat-square)](https://github.com/BasedHardware/Omi/issues)
[![Contributors](https://img.shields.io/github/contributors/BasedHardware/Omi?color=14b8a6&style=flat-square)](https://github.com/BasedHardware/Omi/graphs/contributors)
[![GitHub forks](https://img.shields.io/github/forks/BasedHardware/Omi?color=0ea5e9&style=flat-square)](https://github.com/BasedHardware/Omi/network/members)
[![GitHub last commit](https://img.shields.io/github/last-commit/BasedHardware/Omi?color=8b5cf6&style=flat-square)](https://github.com/BasedHardware/Omi/commits/main)

[![Website](https://img.shields.io/badge/omi.me-Website-0ea5e9?style=for-the-badge)](https://omi.me/)
[![Download](https://img.shields.io/badge/omi.me-Download-14b8a6?style=for-the-badge)](https://omi.me/download)
[![Docs](https://img.shields.io/badge/docs-omi.me-6366f1?style=for-the-badge)](https://docs.omi.me/)
[![Dev%20Kit](https://img.shields.io/badge/Buy-Omi%20Dev%20Kit-0ea5e9?style=for-the-badge)](https://www.omi.me/products/omi-dev-kit-2)
[![Glass%20Kit](https://img.shields.io/badge/Buy-Omi%20Glass-8b5cf6?style=for-the-badge)](https://www.omi.me/glass)

</div>

## ⚡ Quick Links

| Resource | Link |
| --- | --- |
| 🌐 Project site | [omi.me](https://omi.me/) |
| ⬇️ Download center | [omi.me/download](https://omi.me/download) |
| 📚 Documentation | [docs.omi.me](https://docs.omi.me/) |
| 🛠️ Omi Dev Kit | [Buy Omi Dev Kit](https://www.omi.me/products/omi-dev-kit-2) |
| 👓 Omi Glass Dev Kit | [Buy Omi Glass](https://www.omi.me/glass) |

---

## Table of Contents

- [📌 Overview](#overview)
- [⚡️ Features](#features)
- [🚀 Quick Start (2 min)](#quick-start-2-min)
- [🏗️ Project Structure](#project-structure)
- [🧰 Prerequisites](#prerequisites)
- [🛠️ Installation](#installation)
- [🧪 Usage](#usage)
- [⚙️ Configuration](#configuration)
- [🧾 Examples](#examples)
- [🧭 Development Notes](#development-notes)
- [🐞 Troubleshooting](#troubleshooting)
- [🗺️ Roadmap](#roadmap)
- [📚 Documentation](#documentation)
- [🤝 Contribution](#contribution)
- [❤️ Support](#%E2%9D%A4%EF%B8%8F-support)
- [💬 Contact & Community](#contact--community)
- [📜 License](#license)

## Overview

This repository is the open-source Omi ecosystem monorepo.

| Includes | Details |
| --- | --- |
| 🧠 Omi Hardware | Omi wearable firmware + hardware assets |
| 🥽 Omi Glass | Omi Glass firmware/hardware/app |
| 📱 Mobile | Flutter companion app |
| 🌐 Backend | FastAPI backend services |
| 🕸️ Web | Main Omi frontend + Personas |
| 🧩 Ecosystem | Plugins/integrations ecosystem |
| 📦 SDKs | Python, React Native, Swift |
| 🔗 Agent Infra | MCP server |
| 📘 Docs | Documentation source |

The root README is focused on onboarding and day-to-day developer workflow. Full component-specific setup and deeper operational notes live in each subproject README and `docs/`.

## Features

- ⚡ Real-time AI audio processing and transcription flows
- 🔋 Low-power Bluetooth wearable device workflows
- 🧩 Open-source software stack across firmware, apps, backend, web, and SDKs
- 🎙️ Wearable-first UX for meetings, chats, and voice memos
- 🔗 Webhook/app ecosystem for triggering custom actions
- 🛠️ Plugin and integration architecture for extending capabilities

## Quick Start (2 min)

### 1) Download omi App

[<img src='https://upload.wikimedia.org/wikipedia/commons/7/78/Google_Play_Store_badge_EN.svg' alt='Get it on Google Play' height="50px" width="180px">](https://play.google.com/store/apps/details?id=com.friend.ios)
[<img src='https://upload.wikimedia.org/wikipedia/commons/3/3c/Download_on_the_App_Store_Badge.svg' alt="Download on the App Store" height="50px" width="180px">](https://apps.apple.com/us/app/friend-ai-wearable/id6502156163)
[<img src='https://github.com/user-attachments/assets/59c47ec7-3da0-47d7-be2f-7467e4189499' alt="Download MacOS app" height="50px" width="180px">](https://apps.apple.com/us/app/omi-ai-smart-meeting-notes/id6502156163)

### 2) Create a webhook

Create webhook using [webhook.site](https://webhook.site) and copy this URL.

<img src="https://github.com/user-attachments/assets/083a6ec4-4694-4c7a-843a-4a1a0c254453" width="500">

### 3) In omi App

| Explore => Create an App                                                                                  | Select Capability                                                                                       | Paste Webhook URL                                                                                         | Install App                                                                                             |
| --------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------- |
| <img src="https://github.com/user-attachments/assets/31809b81-7de2-4381-b5fc-5c9714972211" width="200"> | <img src="https://github.com/user-attachments/assets/59cfbe8e-7e3b-437f-81f7-25eb50ccdd7d" width="200"> | <img src="https://github.com/user-attachments/assets/3d864ee8-555f-4ded-b4db-87ff78128323" width="200"> | <img src="https://github.com/user-attachments/assets/58cf6da6-e245-415e-92e7-dc1f46583cfc" width="200"> |

### 4) Speak and verify events

Start speaking, you'll see real-time transcript on [webhook.site](https://webhook.site).

## Project Structure

### In this repo

| Component | Purpose |
| --- | --- |
| [omi device](https://github.com/BasedHardware/omi/tree/main/omi) | Omi hardware + firmware |
| [omi glass](https://github.com/BasedHardware/omi/tree/main/omiGlass) | Omi Glass hardware + firmware |
| [omi app](https://github.com/BasedHardware/omi/tree/main/app) | Flutter companion application |
| [ai personas (web)](https://github.com/BasedHardware/omi/tree/main/web/personas-open-source) | Personas web app |
| [SDKs](./sdks) | Python, React Native, and Swift SDKs |

Note: older references may mention `personas-open-source` at repository root; in this repository it is currently under `web/personas-open-source`.

### High-level map

```text
.
├── app/                     # Flutter companion app
├── backend/                 # FastAPI backend
├── docs/                    # Mintlify docs
├── mcp/                     # MCP server for memories/conversations
├── omi/                     # Omi hardware + firmware
├── omiGlass/                # Omi Glass hardware + firmware + app
├── plugins/                 # Integrations/apps/plugins
├── sdks/                    # python / react-native / swift
├── web/frontend/            # Main Next.js frontend
├── web/personas-open-source/ # Personas web app
├── scripts/                 # tooling (format hooks, OTA helper)
└── i18n/                    # Multilingual content and translations
```

## Prerequisites

Use the requirements relevant to your target component.

| Tooling | Used for |
| --- | --- |
| Git | Source control |
| Node.js 18+ and npm | web, personas, some plugin workflows |
| Python 3.10+ | backend, MCP, Python SDK |
| Flutter SDK | mobile app |
| Xcode/CocoaPods | iOS development |
| Android Studio + Android SDK | Android development |
| `ffmpeg` + `opus` | backend/audio workflows |
| Docker (optional) | MCP/web deployments |
| Google Cloud + Firebase | backend/app workflows |

### Assumptions for setup

- Some commands rely on external credentials (Firebase, OpenAI/Deepgram/API providers), which you typically configure per component using its `.env` template. See component READMEs if values are missing from local docs.
- If you only need one surface, install/build only that component to keep iteration fast.

## Installation

Because this is a monorepo, install per component.

### Clone repository

```bash
git clone https://github.com/BasedHardware/omi.git
cd omi
```

### App (Flutter)

```bash
cd app
bash setup.sh ios
# or
bash setup.sh android

flutter run --flavor dev
```

### Backend (FastAPI)

```bash
cd backend
cp .env.template .env
pip install -r requirements.txt
uvicorn main:app --reload --env-file .env
```

### Main frontend (Next.js)

```bash
cd web/frontend
npm install
cp .env.template .env.local
npm run dev
```

### Personas web app (Next.js)

```bash
cd web/personas-open-source
npm install
npm run dev
```

### MCP server

```bash
cd mcp
# See mcp/README.md for Docker-based Claude Desktop setup
```

### SDKs

```bash
cd sdks/python && pip install -e .
cd ../react-native && npm install
# Swift package is exposed via root Package.swift as `omi-lib`
```

## Usage

### End-user app flow

1. Install the Omi app from the store links above.
2. Pair/use your Omi device.
3. Create an app via the webhook quick-start flow.
4. Speak and observe real-time transcript events at your webhook endpoint.

### Local backend with app

1. Start backend locally on port `8000`.
2. Expose local backend via ngrok static domain.
3. Set app `BASE_API_URL` to your ngrok URL.
4. Use Omi app against your local backend.

### SDK workflows

- Python SDK: scan for BLE devices with `omi-scan`, decode Opus packets, and transcribe via Deepgram.
- React Native SDK: connect, stream audio bytes, inspect codec/battery.
- Swift SDK (`omi-lib`): scan/connect/transcribe using `OmiManager` APIs.

## Configuration

Configuration is distributed by component. Use each subproject template/readme as source of truth.

- `backend/.env.template` -> backend API keys/infrastructure config
- `web/frontend/.env.template` -> web frontend env vars
- `app` environment values -> mobile app runtime configuration
- `mcp` env vars -> `OMI_API_KEY` and optional `OMI_API_BASE_URL`
- SDK-specific keys:
  - Python SDK uses `DEEPGRAM_API_KEY`
  - Personas uses Firebase/OpenRouter/RapidAPI/Mixpanel env vars

If you are unsure which variables are required, preserve defaults and follow the specific README in that component before removing/changing values.

## Examples

### Webhook quick-start (from root flow)

Use [webhook.site](https://webhook.site), install your custom app in Omi, then verify transcript events appear in real time.

### Backend run command

```bash
cd backend
uvicorn main:app --reload --env-file .env
```

### Frontend run command

```bash
cd web/frontend
npm run dev
```

### Python SDK scan

```bash
cd sdks/python
omi-scan
```

## Development Notes

- CI/CD and deployment automation are configured in:
  - `.github/workflows/`
  - `codemagic.yaml`
- Root `scripts/pre-commit` formats staged files for:
  - Dart in `app/`
  - Python in `backend/`
  - C/C++ in `omi/` and `omiGlass/`
- `Package.swift` at repository root publishes Swift package `omi-lib` from `sdks/swift`.
- `i18n/` directory exists and is reserved for multilingual README/content variants.

## Troubleshooting

- Backend model/network issue on local setup: if you hit the known SSL download issue, apply the `ssl` workaround documented in `backend/README.md` and retry.
- App cannot reach local backend: verify ngrok domain is running and `BASE_API_URL` points to that exact public URL.
- BLE discovery issues: confirm platform Bluetooth permissions are granted (Terminal/Xcode/Android app as applicable).
- Path mismatch in older docs: some legacy docs/reference text may show outdated paths (for example `personas-open-source` root path or `omi/OmiGlass` casing). In this repo use current directory layout shown above.

## Roadmap

This section reflects current repository signals and may evolve:

- Continue improving firmware/hardware workflows for Omi and OmiGlass
- Expand app/plugin ecosystem and developer tooling
- Improve web experiences for memories/apps/personas
- Strengthen MCP + SDK integrations for external agent ecosystems
- Add and maintain multilingual README variants in `i18n/`

## Documentation

- [Introduction](https://docs.omi.me/)
- [omi App setup](https://docs.omi.me/doc/developer/AppSetup)
- [Buying Guide](https://docs.omi.me/doc/assembly/Buying_Guide/)
- [Build the device](https://docs.omi.me/doc/assembly/Build_the_device/)
- [Install firmware](https://docs.omi.me/doc/get_started/Flash_device/)
- [Create your own app in 1 minute](https://docs.omi.me/doc/developer/apps/Introduction)

## Contribution

- Check out our [contributions guide](https://docs.omi.me/doc/developer/Contribution/).
- Earn from contributing! Check the [paid bounties 🤑](https://omi.me/bounties).
- Check out the [current issues](https://github.com/BasedHardware/Omi/issues).
- Join the [Discord](http://discord.omi.me).
- Build your own [Plugins/Integrations](https://docs.omi.me/doc/developer/apps/Introduction).

## ❤️ Support

| Donate | PayPal | Stripe |
| --- | --- | --- |
| [![Donate](https://camo.githubusercontent.com/24a4914f0b42c6f435f9e101621f1e52535b02c225764b2f6cc99416926004b7/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f446f6e6174652d4c617a79696e674172742d3045413545393f7374796c653d666f722d7468652d6261646765266c6f676f3d6b6f2d6669266c6f676f436f6c6f723d7768697465)](https://chat.lazying.art/donate) | [![PayPal](https://camo.githubusercontent.com/d0f57e8b016517a4b06961b24d0ca87d62fdba16e18bbdb6aba28e978dc0ea21/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f50617950616c2d526f6e677a686f754368656e2d3030343537433f7374796c653d666f722d7468652d6261646765266c6f676f3d70617970616c266c6f676f436f6c6f723d7768697465)](https://paypal.me/RongzhouChen) | [![Stripe](https://camo.githubusercontent.com/1152dfe04b6943afe3a8d2953676749603fb9f95e24088c92c97a01a897b4942/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f5374726970652d446f6e6174652d3633354246463f7374796c653d666f722d7468652d6261646765266c6f676f3d737472697065266c6f676f436f6c6f723d7768697465)](https://buy.stripe.com/aFadR8gIaflgfQV6T4fw400) |

## Contact & Community

- Main site: [omi.me](https://omi.me/)
- Downloads: [omi.me/download](https://omi.me/download)
- Docs: [docs.omi.me](https://docs.omi.me/)
- Community chat: [discord.omi.me](http://discord.omi.me)
- Follow updates: [x.com/kodjima33](https://x.com/kodjima33)
- Hardware/dev kits:
  - [Buy omi Dev Kit](https://www.omi.me/products/omi-dev-kit-2)
  - [Buy Omi Glass Dev Kit](https://www.omi.me/glass)

## License

Omi is available under <a href="https://github.com/BasedHardware/omi/blob/main/LICENSE">MIT License</a>
