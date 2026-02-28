[English](../README.md) · [العربية](README.ar.md) · [Español](README.es.md) · [Français](README.fr.md) · [日本語](README.ja.md) · [한국어](README.ko.md) · [Tiếng Việt](README.vi.md) · [中文 (简体)](README.zh-Hans.md) · [中文（繁體）](README.zh-Hant.md) · [Deutsch](README.de.md) · [Русский](README.ru.md)


**Sprachen:** Englisch (aktuell) | i18n-Varianten werden unter [`/i18n`](../i18n) hinzugefügt

<p align="center">
  <img src="https://raw.githubusercontent.com/lachlanchen/lachlanchen/main/logos/banner.png" alt="LazyingArt banner" />
</p>

<div align="center">

# **omi**

Lerne Omi kennen, das weltweit führende Open-Source-AI-Wearable, das Gespräche erfasst, Zusammenfassungen und Aktionspunkte liefert und Aufgaben für dich ausführt. Verbinde Omi einfach mit deinem Mobilgerät und erhalte automatisch hochwertige Transkriptionen von Meetings, Chats und Sprachnotizen, egal wo du bist.

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

[Site](https://omi.me/) | [Download](https://omi.me/download) | [Docs](https://docs.omi.me/) | [Buy omi Dev Kit](https://www.omi.me/products/omi-dev-kit-2) | [Buy Omi Glass Dev Kit](https://www.omi.me/glass)

</h3>

</div>

## Inhaltsverzeichnis

- [Überblick](#überblick)
- [Funktionen](#funktionen)
- [Schnellstart (2 min)](#schnellstart-2-min)
- [Projektstruktur](#projektstruktur)
- [Voraussetzungen](#voraussetzungen)
- [Installation](#installation)
- [Verwendung](#verwendung)
- [Konfiguration](#konfiguration)
- [Beispiele](#beispiele)
- [Hinweise zur Entwicklung](#hinweise-zur-entwicklung)
- [Fehlerbehebung](#fehlerbehebung)
- [Roadmap](#roadmap)
- [Dokumentation](#dokumentation)
- [Beiträge](#beiträge)
- [Support und Community](#support-und-community)
- [Lizenz](#lizenz)

## Überblick

Dieses Repository ist das Open-Source-Monorepo des Omi-Ökosystems.

| Enthält | Details |
| --- | --- |
| Hardware/Firmware | Omi-Wearable-Firmware + Hardware-Assets |
| Omi Glass | Omi-Glass-Firmware/Hardware/App |
| Mobile | Flutter-Begleit-App |
| Backend | FastAPI-Backend-Services |
| Web | Omi-Hauptfrontend + Personas |
| Ökosystem | Plugin-/Integrations-Ökosystem |
| SDKs | Python, React Native, Swift |
| Agent-Infrastruktur | MCP-Server |
| Docs | Dokumentationsquelle |

Der Quick Start im root README ist bewusst auf Endnutzer und Entwickler-Onboarding fokussiert. Das vollständige, komponentenspezifische Setup findest du in den READMEs der jeweiligen Teilprojekte und in der Omi-Dokumentation.

## Funktionen

- ⚡ Echtzeit-AI-Audioverarbeitung und Transkriptionsabläufe
- 🔋 Low-Power-Bluetooth-Wearable-Workflows
- 🧩 Open-Source-Software-Stack über Firmware, Apps, Backend, Web und SDKs hinweg
- 🎙️ Wearable-first-UX für Meetings, Chats und Sprachnotizen
- 🔗 Webhook-/App-Ökosystem zum Auslösen benutzerdefinierter Aktionen
- 🛠️ Plugin-/Integrationsarchitektur zur Erweiterung der Funktionen

## Schnellstart (2 min)

### 1) omi-App herunterladen

[<img src='https://upload.wikimedia.org/wikipedia/commons/7/78/Google_Play_Store_badge_EN.svg' alt='Get it on Google Play' height="50px" width="180px">](https://play.google.com/store/apps/details?id=com.friend.ios)
[<img src='https://upload.wikimedia.org/wikipedia/commons/3/3c/Download_on_the_App_Store_Badge.svg' alt="Download on the App Store" height="50px" width="180px">](https://apps.apple.com/us/app/friend-ai-wearable/id6502156163)
[<img src='https://github.com/user-attachments/assets/59c47ec7-3da0-47d7-be2f-7467e4189499' alt="Download MacOS app" height="50px" width="180px">](https://apps.apple.com/us/app/omi-ai-smart-meeting-notes/id6502156163)

### 2) Einen Webhook erstellen

Erstelle einen Webhook mit [webhook.site](https://webhook.site) und kopiere diese URL.

<img src="https://github.com/user-attachments/assets/083a6ec4-4694-4c7a-843a-4a1a0c254453" width="500">

### 3) In der omi-App

| Explore => Create an App                                                                                  | Select Capability                                                                                       | Paste Webhook URL                                                                                         | Install App                                                                                             |
| --------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------- |
| <img src="https://github.com/user-attachments/assets/31809b81-7de2-4381-b5fc-5c9714972211" width="200"> | <img src="https://github.com/user-attachments/assets/59cfbe8e-7e3b-437f-81f7-25eb50ccdd7d" width="200"> | <img src="https://github.com/user-attachments/assets/3d864ee8-555f-4ded-b4db-87ff78128323" width = "200"> | <img src="https://github.com/user-attachments/assets/58cf6da6-e245-415e-92e7-dc1f46583cfc" width="200"> |

### 4) Sprechen und Events verifizieren

Beginne zu sprechen, und du siehst das Echtzeit-Transkript auf [webhook.site](https://webhook.site).

## Projektstruktur

### In diesem Repository

- [omi device](https://github.com/BasedHardware/omi/tree/main/omi)
- [omi glass](https://github.com/BasedHardware/omi/tree/main/omiGlass)
- [omi app](https://github.com/BasedHardware/omi/tree/main/app)
- [ai personas (web)](https://github.com/BasedHardware/omi/tree/main/web/personas-open-source)
- [SDKs](./sdks)

Hinweis: Ältere Verweise können `personas-open-source` im Repository-Root nennen; in diesem Repository liegt es derzeit unter `web/personas-open-source`.

### Übersicht auf hoher Ebene

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

## Voraussetzungen

Verwende die Anforderungen, die für deine Zielkomponente relevant sind.

| Tooling | Verwendet für |
| --- | --- |
| Git | Versionsverwaltung |
| Node.js 18+ und npm | web, personas, einige Plugin-Workflows |
| Python 3.10+ | backend, MCP, Python SDK |
| Flutter SDK | Mobile App |
| Xcode/CocoaPods | iOS-Entwicklung |
| Android Studio + Android SDK | Android-Entwicklung |
| `ffmpeg` + `opus` | backend/audio workflows |
| Docker (optional) | MCP/web deployments |
| Google Cloud + Firebase | backend/app workflows |

## Installation

Da dies ein Monorepo ist, installiere pro Komponente.

### Repository klonen

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

### Hauptfrontend (Next.js)

```bash
cd web/frontend
npm install
cp .env.template .env.local
npm run dev
```

### Personas-Web-App (Next.js)

```bash
cd web/personas-open-source
npm install
npm run dev
```

### MCP-Server

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

## Verwendung

### Endnutzer-App-Flow

1. Installiere die Omi-App über die Store-Links oben.
2. Kopple/verwende dein Omi-Gerät.
3. Erstelle eine App über den Webhook-Quick-Start-Flow.
4. Sprich und beobachte Echtzeit-Transkript-Events an deinem Webhook-Endpunkt.

### Lokales Backend mit App

1. Starte das Backend lokal auf Port `8000`.
2. Exponiere das lokale Backend über eine statische ngrok-Domain.
3. Setze `BASE_API_URL` in der App auf deine ngrok-URL.
4. Verwende die Omi-App gegen dein lokales Backend.

### SDK-Workflows

- Python SDK: nach BLE-Geräten mit `omi-scan` suchen, Opus-Pakete dekodieren und über Deepgram transkribieren.
- React Native SDK: verbinden, Audio-Bytes streamen, Codec/Batterie prüfen.
- Swift SDK (`omi-lib`): scannen/verbinden/transkribieren mit `OmiManager`-APIs.

## Konfiguration

Die Konfiguration ist je Komponente verteilt. Verwende die Templates/READMEs der jeweiligen Teilprojekte als Source of Truth.

- `backend/.env.template` -> backend API keys/infrastructure config
- `web/frontend/.env.template` -> web frontend env vars
- `app` environment values -> mobile app runtime configuration
- `mcp` env vars -> `OMI_API_KEY` and optional `OMI_API_BASE_URL`
- SDK-specific keys:
  - Python SDK uses `DEEPGRAM_API_KEY`
  - Personas uses Firebase/OpenRouter/RapidAPI/Mixpanel env vars

Wenn du unsicher bist, welche Variablen erforderlich sind, belasse die Standardwerte und folge der jeweiligen README dieser Komponente, bevor du Werte entfernst/änderst.

## Beispiele

### Webhook-Quick-Start (aus dem Root-Flow)

Nutze [webhook.site](https://webhook.site), installiere deine benutzerdefinierte App in Omi und prüfe dann, ob Transkript-Events in Echtzeit erscheinen.

### Backend-Startbefehl

```bash
cd backend
uvicorn main:app --reload --env-file .env
```

### Frontend-Startbefehl

```bash
cd web/frontend
npm run dev
```

### Python-SDK-Scan

```bash
cd sdks/python
omi-scan
```

## Hinweise zur Entwicklung

- CI/CD- und Deployment-Automatisierung sind konfiguriert in:
  - `.github/workflows/`
  - `codemagic.yaml`
- Root `scripts/pre-commit` formatiert gestagte Dateien für:
  - Dart in `app/`
  - Python in `backend/`
  - C/C++ in `omi/` und `omiGlass/`
- `Package.swift` im Repository-Root veröffentlicht das Swift-Paket `omi-lib` aus `sdks/swift`.
- Das Verzeichnis `i18n/` existiert und ist für mehrsprachige README-/Content-Varianten reserviert.

## Fehlerbehebung

- Backend-Modell-/Netzwerkproblem bei lokalem Setup: Wenn das bekannte SSL-Download-Problem auftritt, wende den in `backend/README.md` dokumentierten `ssl`-Workaround an und versuche es erneut.
- App kann lokales Backend nicht erreichen: Prüfe, ob die ngrok-Domain läuft und `BASE_API_URL` auf genau diese öffentliche URL zeigt.
- BLE-Erkennungsprobleme: Stelle sicher, dass Bluetooth-Berechtigungen auf der jeweiligen Plattform erteilt wurden (Terminal/Xcode/Android-App je nach Anwendungsfall).
- Pfadabweichungen in älteren Docs: Manche Legacy-Dokumente/Referenztexte können veraltete Pfade zeigen (z. B. `personas-open-source` im Root oder `omi/OmiGlass`-Schreibweise). In diesem Repository gilt das oben gezeigte aktuelle Verzeichnislayout.

## Roadmap

Dieser Abschnitt spiegelt aktuelle Signale aus dem Repository wider und kann sich weiterentwickeln:

- Firmware-/Hardware-Workflows für Omi und OmiGlass weiter verbessern
- App-/Plugin-Ökosystem und Entwickler-Tooling ausbauen
- Web-Erlebnisse für Memories/Apps/Personas verbessern
- MCP- und SDK-Integrationen für externe Agent-Ökosysteme stärken
- Mehrsprachige README-Varianten in `i18n/` hinzufügen und pflegen

## Dokumentation

- [Introduction](https://docs.omi.me/)
- [omi App setup](https://docs.omi.me/doc/developer/AppSetup)
- [Buying Guide](https://docs.omi.me/doc/assembly/Buying_Guide/)
- [Build the device](https://docs.omi.me/doc/assembly/Build_the_device/)
- [Install firmware](https://docs.omi.me/doc/get_started/Flash_device/)
- [Create your own app in 1 minute](https://docs.omi.me/doc/developer/apps/Introduction)

## Beiträge

- Sieh dir unseren [contributions guide](https://docs.omi.me/doc/developer/Contribution/) an.
- Verdiene mit Beiträgen! Schau dir die [paid bounties 🤑](https://omi.me/bounties) an.
- Prüfe die [aktuellen Issues](https://github.com/BasedHardware/Omi/issues).
- Tritt dem [Discord](http://discord.omi.me) bei.
- Entwickle deine eigenen [Plugins/Integrations](https://docs.omi.me/doc/developer/apps/Introduction).

## Support und Community

- Hauptseite: [omi.me](https://omi.me/)
- Downloads: [omi.me/download](https://omi.me/download)
- Docs: [docs.omi.me](https://docs.omi.me/)
- Community-Chat: [discord.omi.me](http://discord.omi.me)
- Folge Updates: [x.com/kodjima33](https://x.com/kodjima33)
- Hardware-/Dev-Kits:
  - [Buy omi Dev Kit](https://www.omi.me/products/omi-dev-kit-2)
  - [Buy Omi Glass Dev Kit](https://www.omi.me/glass)

## Lizenz

Omi ist unter der <a href="https://github.com/BasedHardware/omi/blob/main/LICENSE">MIT License</a> verfügbar.
