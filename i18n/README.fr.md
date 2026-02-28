[English](../README.md) · [العربية](README.ar.md) · [Español](README.es.md) · [Français](README.fr.md) · [日本語](README.ja.md) · [한국어](README.ko.md) · [Tiếng Việt](README.vi.md) · [中文 (简体)](README.zh-Hans.md) · [中文（繁體）](README.zh-Hant.md) · [Deutsch](README.de.md) · [Русский](README.ru.md)


<p align="center">
  <img src="https://raw.githubusercontent.com/lachlanchen/lachlanchen/main/logos/banner.png" alt="LazyingArt banner" />
</p>

<div align="center">

# **omi**

Découvrez Omi, le wearable IA open source leader mondial, qui capture les conversations, fournit des résumés, des actions à effectuer et exécute des actions pour vous. Connectez simplement Omi à votre appareil mobile et profitez de transcriptions automatiques de haute qualité pour vos réunions, discussions et mémos vocaux, où que vous soyez.

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

<h3>

[Site](https://omi.me/) | [Télécharger](https://omi.me/download) | [Docs](https://docs.omi.me/) | [Acheter le omi Dev Kit](https://www.omi.me/products/omi-dev-kit-2) | [Acheter le Omi Glass Dev Kit](https://www.omi.me/glass)

</h3>

</div>

## Table des matières

- [Aperçu](#aperçu)
- [Fonctionnalités](#fonctionnalités)
- [Démarrage rapide (2 min)](#démarrage-rapide-2-min)
- [Structure du projet](#structure-du-projet)
- [Prérequis](#prérequis)
- [Installation](#installation)
- [Utilisation](#utilisation)
- [Configuration](#configuration)
- [Exemples](#exemples)
- [Notes de développement](#notes-de-développement)
- [Dépannage](#dépannage)
- [Feuille de route](#feuille-de-route)
- [Documentation](#documentation)
- [Contributions](#contributions)
- [Support et communauté](#support-et-communauté)
- [Licence](#licence)

## Aperçu

Ce dépôt est le monorepo de l’écosystème open source Omi.

| Inclut | Détails |
| --- | --- |
| Hardware/Firmware | Firmware du wearable Omi + ressources matérielles |
| Omi Glass | Firmware/matériel/app Omi Glass |
| Mobile | App compagnon Flutter |
| Backend | Services backend FastAPI |
| Web | Frontend principal Omi + Personas |
| Écosystème | Écosystème de plugins/intégrations |
| SDKs | Python, React Native, Swift |
| Infra Agent | Serveur MCP |
| Docs | Source de la documentation |

Le quick-start du README racine est volontairement orienté onboarding utilisateur/développeur. La configuration complète spécifique à chaque composant se trouve dans les README de chaque sous-projet et dans la documentation Omi.

## Fonctionnalités

- ⚡ Flows de traitement audio IA et de transcription en temps réel
- 🔋 Workflows d’appareil wearable Bluetooth basse consommation
- 🧩 Stack logicielle open source couvrant firmware, apps, backend, web et SDKs
- 🎙️ UX pensée d’abord pour le wearable pour les réunions, discussions et mémos vocaux
- 🔗 Écosystème webhook/app pour déclencher des actions personnalisées
- 🛠️ Architecture plugin/intégration pour étendre les capacités

## Démarrage rapide (2 min)

### 1) Télécharger l’app omi

[<img src='https://upload.wikimedia.org/wikipedia/commons/7/78/Google_Play_Store_badge_EN.svg' alt='Get it on Google Play' height="50px" width="180px">](https://play.google.com/store/apps/details?id=com.friend.ios)
[<img src='https://upload.wikimedia.org/wikipedia/commons/3/3c/Download_on_the_App_Store_Badge.svg' alt="Download on the App Store" height="50px" width="180px">](https://apps.apple.com/us/app/friend-ai-wearable/id6502156163)
[<img src='https://github.com/user-attachments/assets/59c47ec7-3da0-47d7-be2f-7467e4189499' alt="Download MacOS app" height="50px" width="180px">](https://apps.apple.com/us/app/omi-ai-smart-meeting-notes/id6502156163)

### 2) Créer un webhook

Créez un webhook via [webhook.site](https://webhook.site) puis copiez cette URL.

<img src="https://github.com/user-attachments/assets/083a6ec4-4694-4c7a-843a-4a1a0c254453" width="500">

### 3) Dans l’app omi

| Explore => Create an App                                                                                  | Select Capability                                                                                       | Paste Webhook URL                                                                                         | Install App                                                                                             |
| --------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------- |
| <img src="https://github.com/user-attachments/assets/31809b81-7de2-4381-b5fc-5c9714972211" width="200"> | <img src="https://github.com/user-attachments/assets/59cfbe8e-7e3b-437f-81f7-25eb50ccdd7d" width="200"> | <img src="https://github.com/user-attachments/assets/3d864ee8-555f-4ded-b4db-87ff78128323" width = "200"> | <img src="https://github.com/user-attachments/assets/58cf6da6-e245-415e-92e7-dc1f46583cfc" width="200"> |

### 4) Parlez puis vérifiez les événements

Commencez à parler, vous verrez la transcription en temps réel sur [webhook.site](https://webhook.site).

## Structure du projet

### Dans ce dépôt

- [omi device](https://github.com/BasedHardware/omi/tree/main/omi)
- [omi glass](https://github.com/BasedHardware/omi/tree/main/omiGlass)
- [omi app](https://github.com/BasedHardware/omi/tree/main/app)
- [ai personas (web)](https://github.com/BasedHardware/omi/tree/main/web/personas-open-source)
- [SDKs](./sdks)

Note: d’anciennes références peuvent mentionner `personas-open-source` à la racine du dépôt ; dans ce dépôt, il se trouve actuellement sous `web/personas-open-source`.

### Vue d’ensemble

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
├── web/personas-open-source/# Personas web app
└── scripts/                 # tooling (format hooks, OTA helper)
```

## Prérequis

Utilisez les exigences pertinentes pour le composant ciblé.

| Tooling | Utilisé pour |
| --- | --- |
| Git | Contrôle de version |
| Node.js 18+ and npm | web, personas, certains workflows de plugins |
| Python 3.10+ | backend, MCP, SDK Python |
| Flutter SDK | app mobile |
| Xcode/CocoaPods | développement iOS |
| Android Studio + Android SDK | développement Android |
| `ffmpeg` + `opus` | workflows backend/audio |
| Docker (optional) | déploiements MCP/web |
| Google Cloud + Firebase | workflows backend/app |

## Installation

Comme il s’agit d’un monorepo, l’installation se fait par composant.

### Cloner le dépôt

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

### Frontend principal (Next.js)

```bash
cd web/frontend
npm install
cp .env.template .env.local
npm run dev
```

### App web Personas (Next.js)

```bash
cd web/personas-open-source
npm install
npm run dev
```

### Serveur MCP

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

## Utilisation

### Parcours utilisateur dans l’app

1. Installez l’app Omi via les liens store ci-dessus.
2. Associez/utilisez votre appareil Omi.
3. Créez une app via le flux quick-start webhook.
4. Parlez et observez les événements de transcription en temps réel sur votre endpoint webhook.

### Backend local avec l’app

1. Démarrez le backend localement sur le port `8000`.
2. Exposez le backend local via un domaine statique ngrok.
3. Définissez `BASE_API_URL` de l’app vers votre URL ngrok.
4. Utilisez l’app Omi avec votre backend local.

### Workflows SDK

- SDK Python : scannez les appareils BLE avec `omi-scan`, décodez les paquets Opus et transcrivez via Deepgram.
- SDK React Native : connectez-vous, streamez des octets audio, inspectez codec/batterie.
- SDK Swift (`omi-lib`) : scan/connexion/transcription avec les APIs `OmiManager`.

## Configuration

La configuration est distribuée par composant. Utilisez le template/readme de chaque sous-projet comme source de vérité.

- `backend/.env.template` -> clés API backend/configuration infrastructure
- `web/frontend/.env.template` -> variables d’environnement du frontend web
- Valeurs d’environnement `app` -> configuration d’exécution de l’app mobile
- Variables d’environnement `mcp` -> `OMI_API_KEY` et `OMI_API_BASE_URL` optionnelle
- Clés spécifiques SDK :
  - Le SDK Python utilise `DEEPGRAM_API_KEY`
  - Personas utilise des variables d’environnement Firebase/OpenRouter/RapidAPI/Mixpanel

Si vous ne savez pas quelles variables sont requises, conservez les valeurs par défaut et suivez d’abord le README spécifique de ce composant avant de supprimer/modifier des valeurs.

## Exemples

### Quick-start webhook (depuis le flux racine)

Utilisez [webhook.site](https://webhook.site), installez votre app personnalisée dans Omi, puis vérifiez que les événements de transcription apparaissent en temps réel.

### Commande de lancement backend

```bash
cd backend
uvicorn main:app --reload --env-file .env
```

### Commande de lancement frontend

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

- L’automatisation CI/CD et de déploiement est configurée dans :
  - `.github/workflows/`
  - `codemagic.yaml`
- Le script racine `scripts/pre-commit` formate les fichiers indexés pour :
  - Dart dans `app/`
  - Python dans `backend/`
  - C/C++ dans `omi/` et `omiGlass/`
- Le `Package.swift` à la racine du dépôt publie le package Swift `omi-lib` depuis `sdks/swift`.
- Le dossier `i18n/` existe et est réservé aux variantes multilingues de README/contenu.

## Dépannage

- Problème de modèle/réseau backend en local : si vous rencontrez le problème connu de téléchargement SSL, appliquez le contournement `ssl` documenté dans `backend/README.md`, puis réessayez.
- L’app ne peut pas joindre le backend local : vérifiez que le domaine ngrok est actif et que `BASE_API_URL` pointe vers cette URL publique exacte.
- Problèmes de découverte BLE : confirmez que les autorisations Bluetooth de la plateforme sont accordées (Terminal/Xcode/app Android selon le cas).
- Incohérence de chemins dans d’anciennes docs : certains documents/textes de référence hérités peuvent afficher des chemins obsolètes (par exemple le chemin racine `personas-open-source` ou la casse `omi/OmiGlass`). Dans ce dépôt, utilisez la structure de dossiers actuelle ci-dessus.

## Feuille de route

Cette section reflète les signaux actuels du dépôt et peut évoluer :

- Continuer à améliorer les workflows firmware/hardware pour Omi et OmiGlass
- Étendre l’écosystème app/plugin et les outils développeur
- Améliorer les expériences web pour memories/apps/personas
- Renforcer les intégrations MCP + SDK pour les écosystèmes d’agents externes
- Ajouter et maintenir des variantes README multilingues dans `i18n/`

## Documentation

- [Introduction](https://docs.omi.me/)
- [omi App setup](https://docs.omi.me/doc/developer/AppSetup)
- [Buying Guide](https://docs.omi.me/doc/assembly/Buying_Guide/)
- [Build the device](https://docs.omi.me/doc/assembly/Build_the_device/)
- [Install firmware](https://docs.omi.me/doc/get_started/Flash_device/)
- [Create your own app in 1 minute](https://docs.omi.me/doc/developer/apps/Introduction)

## Contributions

- Consultez notre [guide de contribution](https://docs.omi.me/doc/developer/Contribution/).
- Gagnez en contribuant ! Consultez les [bounties rémunérées 🤑](https://omi.me/bounties).
- Consultez les [issues en cours](https://github.com/BasedHardware/Omi/issues).
- Rejoignez le [Discord](http://discord.omi.me).
- Développez vos propres [Plugins/Integrations](https://docs.omi.me/doc/developer/apps/Introduction).

## Support et communauté

- Site principal : [omi.me](https://omi.me/)
- Téléchargements : [omi.me/download](https://omi.me/download)
- Docs : [docs.omi.me](https://docs.omi.me/)
- Chat communauté : [discord.omi.me](http://discord.omi.me)
- Suivre les mises à jour : [x.com/kodjima33](https://x.com/kodjima33)
- Matériel/dev kits :
  - [Acheter le omi Dev Kit](https://www.omi.me/products/omi-dev-kit-2)
  - [Acheter le Omi Glass Dev Kit](https://www.omi.me/glass)

## Licence

Omi est disponible sous <a href="https://github.com/BasedHardware/omi/blob/main/LICENSE">MIT License</a>
