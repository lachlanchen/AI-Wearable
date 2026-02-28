[English](../README.md) · [العربية](README.ar.md) · [Español](README.es.md) · [Français](README.fr.md) · [日本語](README.ja.md) · [한국어](README.ko.md) · [Tiếng Việt](README.vi.md) · [中文 (简体)](README.zh-Hans.md) · [中文（繁體）](README.zh-Hant.md) · [Deutsch](README.de.md) · [Русский](README.ru.md)


[![LazyingArt banner](https://github.com/lachlanchen/lachlanchen/raw/main/figs/banner.png)](https://github.com/lachlanchen/lachlanchen/blob/main/figs/banner.png)

<div align="center">

# **omi**

_IA portable pour des réunions et conversations instantanées : capture, résume et agit, les mains libres._

Découvrez Omi, la solution open source IA portable la plus avancée au monde pour capter les conversations, générer des résumés, créer des actions à exécuter et réaliser des actions à votre place. Connectez simplement Omi à votre appareil mobile et profitez de transcriptions automatiques de haute qualité pour réunions, conversations et notes vocales, où que vous soyez.

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

## ⚡ Liens rapides

| Ressource | Lien |
| --- | --- |
| 🌐 Site du projet | [omi.me](https://omi.me/) |
| ⬇️ Centre de téléchargement | [omi.me/download](https://omi.me/download) |
| 📚 Documentation | [docs.omi.me](https://docs.omi.me/) |
| 🛠️ Omi Dev Kit | [Acheter Omi Dev Kit](https://www.omi.me/products/omi-dev-kit-2) |
| 👓 Omi Glass Dev Kit | [Acheter Omi Glass](https://www.omi.me/glass) |

---

## Table des matières

- [📌 Aperçu](#aperçu)
- [⚡️ Fonctionnalités](#fonctionnalités)
- [🚀 Démarrage rapide (2 min)](#démarrage-rapide-2-min)
- [🏗️ Structure du projet](#structure-du-projet)
- [🧰 Prérequis](#prérequis)
- [🛠️ Installation](#installation)
- [🧪 Utilisation](#utilisation)
- [⚙️ Configuration](#configuration)
- [🧾 Exemples](#exemples)
- [🧭 Notes de développement](#notes-de-développement)
- [🐞 Dépannage](#dépannage)
- [🗺️ Feuille de route](#feuille-de-route)
- [📚 Documentation](#documentation)
- [🤝 Contribution](#contribution)
- [❤️ Support](#%E2%9D%A4%EF%B8%8F-support)
- [💬 Contact & Communauté](#contact--communauté)
- [📜 Licence](#licence)

## Aperçu

Ce dépôt est le monorepo open-source de l’écosystème Omi.

| Inclus | Détails |
| --- | --- |
| 🧠 Omi Hardware | Firmware + ressources matérielles Omi |
| 🥽 Omi Glass | Firmware/matériel/application Omi Glass |
| 📱 Mobile | Application compagnon Flutter |
| 🌐 Backend | Services backend FastAPI |
| 🕸️ Web | Frontend principal Omi + Personas |
| 🧩 Écosystème | Plugins/intégrations |
| 📦 SDKs | Python, React Native, Swift |
| 🔗 Agent Infra | Serveur MCP |
| 📘 Docs | Source de documentation |

Le README racine se concentre sur l’onboarding et le flux de travail quotidien des développeurs. Les configurations complètes de chaque composant et les notes opérationnelles détaillées se trouvent dans les README de chaque sous-projet et dans `docs/`.

## Fonctionnalités

- ⚡ Traitement audio IA et transcriptions en temps réel
- 🔋 Flux de travail pour appareil portable Bluetooth basse consommation
- 🧩 Stack logicielle open-source couvrant firmware, applications, backend, web et SDKs
- 🎙️ UX pensée pour l’usage portable : réunions, chats et notes vocales
- 🔗 Écosystème webhook/app pour déclencher des actions personnalisées
- 🛠️ Architecture de plugins et d’intégrations pour étendre les fonctionnalités

## Démarrage rapide (2 min)

### 1) Télécharger l’application Omi

[<img src='https://upload.wikimedia.org/wikipedia/commons/7/78/Google_Play_Store_badge_EN.svg' alt='Get it on Google Play' height="50px" width="180px">](https://play.google.com/store/apps/details?id=com.friend.ios)
[<img src='https://upload.wikimedia.org/wikipedia/commons/3/3c/Download_on_the_App_Store_Badge.svg' alt="Download on the App Store" height="50px" width="180px">](https://apps.apple.com/us/app/friend-ai-wearable/id6502156163)
[<img src='https://github.com/user-attachments/assets/59c47ec7-3da0-47d7-be2f-7467e4189499' alt="Download MacOS app" height="50px" width="180px">](https://apps.apple.com/us/app/omi-ai-smart-meeting-notes/id6502156163)

### 2) Créer un webhook

Créez un webhook avec [webhook.site](https://webhook.site) puis copiez cette URL.

<img src="https://github.com/user-attachments/assets/083a6ec4-4694-4c7a-843a-4a1a0c254453" width="500">

### 3) Dans l’application Omi

| Explorer => Créer une app | Choisir une capacité | Coller l’URL du webhook | Installer l’app |
| --- | --- | --- | --- |
| <img src="https://github.com/user-attachments/assets/31809b81-7de2-4381-b5fc-5c9714972211" width="200"> | <img src="https://github.com/user-attachments/assets/59cfbe8e-7e3b-437f-81f7-25eb50ccdd7d" width="200"> | <img src="https://github.com/user-attachments/assets/3d864ee8-555f-4ded-b4db-87ff78128323" width="200"> | <img src="https://github.com/user-attachments/assets/58cf6da6-e245-415e-92e7-dc1f46583cfc" width="200"> |

### 4) Parler et vérifier les événements

Commencez à parler : les transcriptions arrivent en temps réel sur [webhook.site](https://webhook.site).

## Structure du projet

### Dans ce dépôt

| Composant | Rôle |
| --- | --- |
| [omi device](https://github.com/BasedHardware/omi/tree/main/omi) | Matériel + firmware Omi |
| [omi glass](https://github.com/BasedHardware/omi/tree/main/omiGlass) | Matériel + firmware Omi Glass |
| [omi app](https://github.com/BasedHardware/omi/tree/main/app) | Application compagnon Flutter |
| [ai personas (web)](https://github.com/BasedHardware/omi/tree/main/web/personas-open-source) | Application web Personas |
| [SDKs](./sdks) | SDKs Python, React Native et Swift |

Note : certaines références plus anciennes peuvent mentionner `personas-open-source` à la racine du dépôt ; dans ce dépôt, il se trouve désormais sous `web/personas-open-source`.

### Vue d’ensemble haut niveau

```text
.
├── app/                     # Application compagnon Flutter
├── backend/                 # Backend FastAPI
├── docs/                    # Documentation Mintlify
├── mcp/                     # Serveur MCP pour mémoires/conversations
├── omi/                     # Matériel + firmware Omi
├── omiGlass/                # Matériel + firmware + app Omi Glass
├── plugins/                 # Intégrations/apps/plugins
├── sdks/                    # python / react-native / swift
├── web/frontend/            # Frontend Next.js principal
├── web/personas-open-source/ # Application web Personas
├── scripts/                 # outils (format hooks, OTA helper)
└── i18n/                    # Contenu multilingue et traductions
```

## Prérequis

Utilisez les prérequis adaptés au composant cible.

| Outil | Utilisé pour |
| --- | --- |
| Git | Gestion de version |
| Node.js 18+ et npm | web, personas, certains flux de plugin |
| Python 3.10+ | backend, MCP, SDK Python |
| Flutter SDK | application mobile |
| Xcode/CocoaPods | développement iOS |
| Android Studio + Android SDK | développement Android |
| `ffmpeg` + `opus` | flux audio/backend |
| Docker (optionnel) | déploiements MCP/web |
| Google Cloud + Firebase | flux backend/app |

### Hypothèses de configuration

- Certaines commandes dépendent de credentials externes (Firebase, OpenAI/Deepgram/fournisseurs d’API), généralement configurés par composant via son modèle `.env`. Consultez le README du composant concerné si des valeurs sont absentes de la documentation locale.
- Si vous ne travaillez que sur une surface, installez et build uniquement ce composant pour accélérer l’itération.

## Installation

Ce dépôt étant un monorepo, installez par composant.

### Cloner le dépôt

```bash
git clone https://github.com/BasedHardware/omi.git
cd omi
```

### App (Flutter)

```bash
cd app
bash setup.sh ios
# ou
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

### Frontend principal (Next.js)

```bash
cd web/frontend
npm install
cp .env.template .env.local
npm run dev
```

### Application web Personas (Next.js)

```bash
cd web/personas-open-source
npm install
npm run dev
```

### Serveur MCP

```bash
cd mcp
# Consultez mcp/README.md pour la configuration de Claude Desktop basée sur Docker
```

### SDKs

```bash
cd sdks/python && pip install -e .
cd ../react-native && npm install
# Le package Swift est exposé via le Package.swift racine en tant que `omi-lib`
```

## Utilisation

### Flux côté utilisateur final

1. Installez l’application Omi via les liens de téléchargement ci-dessus.
2. Associez et utilisez votre appareil Omi.
3. Créez une app via le flux de démarrage rapide webhook.
4. Parlez, puis observez les événements de transcription en temps réel sur votre endpoint webhook.

### Backend local avec l’app

1. Démarrez le backend local sur le port `8000`.
2. Exposez le backend local via un domaine statique ngrok.
3. Renseignez `BASE_API_URL` dans l’app avec votre URL ngrok.
4. Utilisez l’application Omi avec votre backend local.

### Flux de travail des SDK

- SDK Python : recherchez les appareils BLE avec `omi-scan`, décodez les paquets Opus et transcrivez via Deepgram.
- SDK React Native : connectez-vous, stream d’octets audio, inspectez codec et batterie.
- SDK Swift (`omi-lib`) : scan/connect/transcription via les API `OmiManager`.

## Configuration

La configuration est répartie par composant. Utilisez le template/README de chaque sous-projet comme source de vérité.

- `backend/.env.template` -> clés d’API et config d’infrastructure backend
- `web/frontend/.env.template` -> variables d’environnement du frontend web
- valeurs d’environnement `app` -> configuration runtime de l’application mobile
- variables d’environnement `mcp` -> `OMI_API_KEY` et `OMI_API_BASE_URL` optionnel
- clés spécifiques aux SDK :
  - Le SDK Python utilise `DEEPGRAM_API_KEY`
  - Personas utilise les variables Firebase/OpenRouter/RapidAPI/Mixpanel

Si vous n’êtes pas certain des variables requises, conservez les valeurs par défaut et suivez le README propre au composant avant de modifier ou supprimer des valeurs.

## Exemples

### Démarrage rapide webhook (depuis le flux racine)

Utilisez [webhook.site](https://webhook.site), installez votre application personnalisée dans Omi, puis vérifiez que les événements de transcription apparaissent en temps réel.

### Commande backend

```bash
cd backend
uvicorn main:app --reload --env-file .env
```

### Commande frontend

```bash
cd web/frontend
npm run dev
```

### Scan SDK Python

```bash
cd sdks/python
omi-scan
```

## Notes de développement

- Les workflows CI/CD et l’automatisation de déploiement sont configurés dans :
  - `.github/workflows/`
  - `codemagic.yaml`
- Le script racine `scripts/pre-commit` formate les fichiers mis en staging pour :
  - Dart dans `app/`
  - Python dans `backend/`
  - C/C++ dans `omi/` et `omiGlass/`
- Le `Package.swift` à la racine publie le package Swift `omi-lib` depuis `sdks/swift`.
- Le dossier `i18n/` existe et est réservé aux variantes README/contenus multilingues.

## Dépannage

- Problème de modèle/réseau en local : si vous rencontrez le problème SSL connu du téléchargement, appliquez le contournement `ssl` documenté dans `backend/README.md`, puis réessayez.
- L’application ne peut pas joindre le backend local : vérifiez que le domaine ngrok fonctionne et que `BASE_API_URL` pointe vers l’URL publique exacte.
- Problèmes de découverte BLE : vérifiez que les permissions Bluetooth sont accordées (Terminal/Xcode/app Android selon le cas).
- Problèmes de chemins dans les docs anciens : certaines références historiques peuvent afficher des chemins obsolètes (par exemple `personas-open-source` à la racine ou la casse `omi/OmiGlass`). Utilisez la structure actuelle indiquée plus haut.

## Feuille de route

Cette section reflète les signaux actuels du dépôt et peut évoluer :

- Continuer d’améliorer les flux firmware/matériel pour Omi et OmiGlass
- Étendre l’écosystème app/plugins et les outils de développement
- Améliorer les expériences web pour mémoires/apps/personas
- Renforcer les intégrations MCP + SDK pour les écosystèmes d’agents externes
- Ajouter et maintenir des variantes README multilingues dans `i18n/`

## Documentation

- [Introduction](https://docs.omi.me/)
- [Configuration de l’app Omi](https://docs.omi.me/doc/developer/AppSetup)
- [Guide d’achat](https://docs.omi.me/doc/assembly/Buying_Guide/)
- [Assembler l’appareil](https://docs.omi.me/doc/assembly/Build_the_device/)
- [Installer le firmware](https://docs.omi.me/doc/get_started/Flash_device/)
- [Créer votre propre app en 1 minute](https://docs.omi.me/doc/developer/apps/Introduction)

## Contribution

- Consultez notre [guide de contribution](https://docs.omi.me/doc/developer/Contribution/).
- Gagnez de l’argent en contribuant ! Consultez les [bounties rémunérés 🤑](https://omi.me/bounties).
- Consultez les [issues en cours](https://github.com/BasedHardware/Omi/issues).
- Rejoignez le [Discord](http://discord.omi.me).
- Construisez vos propres [plugins/integrations](https://docs.omi.me/doc/developer/apps/Introduction).

## ❤️ Support

| Donate | PayPal | Stripe |
| --- | --- | --- |
| [![Donate](https://camo.githubusercontent.com/24a4914f0b42c6f435f9e101621f1e52535b02c225764b2f6cc99416926004b7/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f446f6e6174652d4c617a79696e674172742d3045413545393f7374796c653d666f722d7468652d6261646765266c6f676f3d6b6f2d6669266c6f676f436f6c6f723d7768697465)](https://chat.lazying.art/donate) | [![PayPal](https://camo.githubusercontent.com/d0f57e8b016517a4b06961b24d0ca87d62fdba16e18bbdb6aba28e978dc0ea21/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f50617950616c2d526f6e677a686f754368656e2d3030343537433f7374796c653d666f722d7468652d6261646765266c6f676f3d70617970616c266c6f676f436f6c6f723d7768697465)](https://paypal.me/RongzhouChen) | [![Stripe](https://camo.githubusercontent.com/1152dfe04b6943afe3a8d2953676749603fb9f95e24088c92c97a01a897b4942/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f5374726970652d446f6e6174652d3633354246463f7374796c653d666f722d7468652d6261646765266c6f676f3d737472697065266c6f676f436f6c6f723d7768697465)](https://buy.stripe.com/aFadR8gIaflgfQV6T4fw400) |

## Contact & Communauté

- Site principal : [omi.me](https://omi.me/)
- Téléchargements : [omi.me/download](https://omi.me/download)
- Documentation : [docs.omi.me](https://docs.omi.me/)
- Chat communautaire : [discord.omi.me](http://discord.omi.me)
- Suivre les nouveautés : [x.com/kodjima33](https://x.com/kodjima33)
- Kits matériels :
  - [Acheter Omi Dev Kit](https://www.omi.me/products/omi-dev-kit-2)
  - [Acheter Omi Glass Dev Kit](https://www.omi.me/glass)

## Licence

Omi est disponible sous <a href="https://github.com/BasedHardware/omi/blob/main/LICENSE">licence MIT</a>
