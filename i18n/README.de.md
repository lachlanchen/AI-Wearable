[English](../README.md) · [العربية](README.ar.md) · [Español](README.es.md) · [Français](README.fr.md) · [日本語](README.ja.md) · [한국어](README.ko.md) · [Tiếng Việt](README.vi.md) · [中文 (简体)](README.zh-Hans.md) · [中文（繁體）](README.zh-Hant.md) · [Deutsch](README.de.md) · [Русский](README.ru.md)


[![LazyingArt banner](https://github.com/lachlanchen/lachlanchen/raw/main/figs/banner.png)](https://github.com/lachlanchen/lachlanchen/blob/main/figs/banner.png)

<div align="center">

# **omi**

_AI-gestütztes Wearable für spontane Meetings und Chats: mitschneiden, zusammenfassen und direkt handeln — freihändig._

Meet Omi, das weltweit führende Open-Source-KI-Wearable, das Gespräche aufzeichnet, Zusammenfassungen, Action Items erstellt und Aktionen für dich übernimmt. Verbinde Omi einfach mit deinem Mobilgerät und nutze automatisch hochwertige Transkriptionen von Meetings, Chats und Sprachnachrichten – wo immer du bist.

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

## ⚡ Schnellzugriff

| Ressource | Link |
| --- | --- |
| 🌐 Projektseite | [omi.me](https://omi.me/) |
| ⬇️ Download-Center | [omi.me/download](https://omi.me/download) |
| 📚 Dokumentation | [docs.omi.me](https://docs.omi.me/) |
| 🛠️ Omi Dev Kit | [Kaufe Omi Dev Kit](https://www.omi.me/products/omi-dev-kit-2) |
| 👓 Omi Glass Dev Kit | [Kaufe Omi Glass](https://www.omi.me/glass) |

---

## Inhaltsverzeichnis

- [📌 Überblick](#überblick)
- [⚡️ Funktionen](#funktionen)
- [🚀 Schnellstart (2 min)](#schnellstart-2-min)
- [🏗️ Projektstruktur](#projektstruktur)
- [🧰 Voraussetzungen](#voraussetzungen)
- [🛠️ Installation](#installation)
- [🧪 Verwendung](#verwendung)
- [⚙️ Konfiguration](#konfiguration)
- [🧾 Beispiele](#beispiele)
- [🧭 Entwicklungsnotizen](#entwicklungsnotizen)
- [🐞 Fehlerbehebung](#fehlerbehebung)
- [🗺️ Roadmap](#roadmap)
- [📚 Dokumentation](#dokumentation)
- [🤝 Beitrag](#beitrag)
- [❤️ Support](#%E2%9D%A4%EF%B8%8F-support)
- [💬 Kontakt & Community](#kontakt--community)
- [📜 Lizenz](#lizenz)

## Überblick

Dieses Repository ist das Open-Source-Monorepo des Omi-Ökosystems.

| Enthalten | Details |
| --- | --- |
| 🧠 Omi Hardware | Omi-Wearable-Firmware + Hardware-Dateien |
| 🥽 Omi Glass | Omi Glass Firmware/Hardware/App |
| 📱 Mobile | Flutter Companion App |
| 🌐 Backend | FastAPI Backend-Services |
| 🕸️ Web | Haupt-Omi-Frontend + Personas |
| 🧩 Ökosystem | Plugins- und Integrations-Ökosystem |
| 📦 SDKs | Python, React Native, Swift |
| 🔗 Agent-Infrastruktur | MCP-Server |
| 📘 Docs | Dokumentationsquellen |

Das Root-README ist auf Onboarding und tägliche Entwickler-Workflows ausgerichtet. Komponenten-spezifische Setups sowie tiefere Betriebsnotizen findest du in den jeweiligen Teilprojekten-README-Dateien und in `docs/`.

## Funktionen

- ⚡ KI-basierte Echtzeit-Audioverarbeitung und Transkriptionsabläufe
- 🔋 Energieeffiziente Wearable-Workflows mit Bluetooth
- 🧩 Open-Source-Software-Stack über Firmware, Apps, Backend, Web und SDKs
- 🎙️ Wearable-first UX für Meetings, Chats und Sprachnotizen
- 🔗 Webhook-/App-Ökosystem zum Auslösen benutzerdefinierter Aktionen
- 🛠️ Plugin- und Integrations-Architektur zur Erweiterung der Fähigkeiten

## Schnellstart (2 min)

### 1) Omi App herunterladen

[<img src='https://upload.wikimedia.org/wikipedia/commons/7/78/Google_Play_Store_badge_EN.svg' alt='Get it on Google Play' height="50px" width="180px">](https://play.google.com/store/apps/details?id=com.friend.ios)
[<img src='https://upload.wikimedia.org/wikipedia/commons/3/3c/Download_on_the_App_Store_Badge.svg' alt="Download on the App Store" height="50px" width="180px">](https://apps.apple.com/us/app/friend-ai-wearable/id6502156163)
[<img src='https://github.com/user-attachments/assets/59c47ec7-3da0-47d7-be2f-7467e4189499' alt="Download MacOS app" height="50px" width="180px">](https://apps.apple.com/us/app/omi-ai-smart-meeting-notes/id6502156163)

### 2) Webhook erstellen

Erstelle einen Webhook über [webhook.site](https://webhook.site) und kopiere diese URL.

<img src="https://github.com/user-attachments/assets/083a6ec4-4694-4c7a-843a-4a1a0c254453" width="500">

### 3) In der Omi-App

| Erkunden => App erstellen                                                                                | Fähigkeit auswählen                                                                                      | Webhook-URL einfügen                                                                                     | App installieren                                                                                        |
| --------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------- |
| <img src="https://github.com/user-attachments/assets/31809b81-7de2-4381-b5fc-5c9714972211" width="200"> | <img src="https://github.com/user-attachments/assets/59cfbe8e-7e3b-437f-81f7-25eb50ccdd7d" width="200"> | <img src="https://github.com/user-attachments/assets/3d864ee8-555f-4ded-b4db-87ff78128323" width="200"> | <img src="https://github.com/user-attachments/assets/58cf6da6-e245-415e-92e7-dc1f46583cfc" width="200"> |

### 4) Sprechen und Ereignisse prüfen

Starte die Spracheingabe und du siehst das Echtzeit-Transkript auf [webhook.site](https://webhook.site).

## Projektstruktur

### In diesem Repository

| Komponente | Zweck |
| --- | --- |
| [omi device](https://github.com/BasedHardware/omi/tree/main/omi) | Omi Hardware + Firmware |
| [omi glass](https://github.com/BasedHardware/omi/tree/main/omiGlass) | Omi Glass Hardware + Firmware |
| [omi app](https://github.com/BasedHardware/omi/tree/main/app) | Flutter Companion App |
| [ai personas (web)](https://github.com/BasedHardware/omi/tree/main/web/personas-open-source) | Personas-Web-App |
| [SDKs](./sdks) | Python-, React Native- und Swift-SDKs |

Hinweis: Ältere Referenzen können `personas-open-source` im Repository-Root erwähnen; in diesem Repository liegt es aktuell unter `web/personas-open-source`.

### Oberflächliche Karte

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

## Voraussetzungen

Nutze die Anforderungen, die für deine Zielkomponente relevant sind.

| Tooling | Verwendet für |
| --- | --- |
| Git | Versionsverwaltung |
| Node.js 18+ und npm | Web, Personas, einige Plugin-Workflows |
| Python 3.10+ | Backend, MCP, Python SDK |
| Flutter SDK | Mobile App |
| Xcode/CocoaPods | iOS-Entwicklung |
| Android Studio + Android SDK | Android-Entwicklung |
| `ffmpeg` + `opus` | Backend-/Audio-Workflows |
| Docker (optional) | MCP-/Web-Deployments |
| Google Cloud + Firebase | Backend-/App-Workflows |

### Voraussetzungen für die Einrichtung

- Einige Befehle benötigen externe Zugangsdaten (Firebase, OpenAI/Deepgram/API-Anbieter), die du typischerweise pro Komponente über deren `.env`-Vorlage konfigurierst. Falls Werte in der lokalen Doku fehlen, prüfe die README-Dateien der Komponenten.
- Wenn du nur eine Oberfläche benötigst, installiere und baue nur diese Komponente, um den Entwicklungszyklus kurz zu halten.

## Installation

Da es sich um ein Monorepo handelt, installiere pro Komponente.

### Repository klonen

```bash
git clone https://github.com/BasedHardware/omi.git
cd omi
```

### App (Flutter)

```bash
cd app
bash setup.sh ios
# oder
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
# Siehe mcp/README.md für die Docker-basierte Claude-Desktop-Konfiguration
```

### SDKs

```bash
cd sdks/python && pip install -e .
cd ../react-native && npm install
# Das Swift-Paket wird über `Package.swift` im Root als `omi-lib` bereitgestellt
```

## Verwendung

### Endnutzer-App-Flow

1. Installiere die Omi-App über die Store-Links oben.
2. Koppel/verwende dein Omi-Gerät.
3. Erstelle eine App über den Webhook-Schnellstart-Flow.
4. Sprich und beobachte die Echtzeit-Transkript-Ereignisse an deinem Webhook-Endpunkt.

### Lokales Backend mit App

1. Starte das Backend lokal auf Port `8000`.
2. Exponiere das lokale Backend über eine statische ngrok-Domain.
3. Setze in der App `BASE_API_URL` auf deine ngrok-URL.
4. Nutze die Omi-App mit deinem lokalen Backend.

### SDK-Workflows

- Python SDK: Suche nach BLE-Geräten mit `omi-scan`, dekodiere Opus-Pakete und transkribiere via Deepgram.
- React Native SDK: verbinde dich, streame Audiobytes und prüfe Codec/Akku.
- Swift SDK (`omi-lib`): scanne/verbinde/transkribiere mit den `OmiManager`-APIs.

## Konfiguration

Die Konfiguration ist komponentenbasiert verteilt. Nutze die jeweiligen Templates/README-Dateien als alleinige Referenz.

- `backend/.env.template` -> Backend-API-Keys/Infrastructure-Konfiguration
- `web/frontend/.env.template` -> Umgebungsvariablen für das Web-Frontend
- `app` Environment values -> Laufzeitkonfiguration der mobilen App
- `mcp` Umgebungsvariablen -> `OMI_API_KEY` und optional `OMI_API_BASE_URL`
- SDK-spezifische Schlüssel:
  - Python SDK nutzt `DEEPGRAM_API_KEY`
  - Personas nutzt Firebase/OpenRouter/RapidAPI/Mixpanel-Umgebungsvariablen

Wenn du unsicher bist, welche Variablen erforderlich sind, behalte die Standardwerte und prüfe die jeweilige Komponenten-README, bevor du Werte entfernst oder änderst.

## Beispiele

### Webhook-Quickstart (aus dem Hauptablauf)

Nutze [webhook.site](https://webhook.site), installiere deine eigene App in Omi und verifiziere dann die Transkript-Ereignisse in Echtzeit.

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

### Python SDK Scan

```bash
cd sdks/python
omi-scan
```

## Entwicklungsnotizen

- CI/CD und Deployment-Automatisierung sind in folgenden Dateien konfiguriert:
  - `.github/workflows/`
  - `codemagic.yaml`
- Das Root-`scripts/pre-commit` formatiert vorgemerkte Dateien für:
  - Dart in `app/`
  - Python in `backend/`
  - C/C++ in `omi/` und `omiGlass/`
- Das Root-`Package.swift` stellt das Swift-Paket `omi-lib` aus `sdks/swift` bereit.
- Das Verzeichnis `i18n/` ist für mehrsprachige README-/Content-Varianten reserviert.

## Fehlerbehebung

- Backend-Modell-/Netzwerkproblem beim lokalen Setup: Wenn du auf ein bekanntes SSL-Download-Problem stößt, wende den in `backend/README.md` dokumentierten `ssl`-Workaround an und versuche es erneut.
- App erreicht kein lokales Backend: Prüfe, dass die ngrok-Domain läuft und `BASE_API_URL` genau auf diese öffentliche URL zeigt.
- BLE-Erkennungsprobleme: Stelle sicher, dass Bluetooth-Berechtigungen der jeweiligen Plattform erteilt sind (Terminal/Xcode/Android-App je nach Plattform).
- Pfadabweichung in älteren Docs: Einige veraltete Docs/Referenztexte können alte Pfade enthalten (z. B. `personas-open-source` im Root-Pfad oder Groß-/Kleinschreibung bei `omi/OmiGlass`). In diesem Repository gilt das oben gezeigte Verzeichnislayout.

## Roadmap

Dieser Abschnitt spiegelt aktuelle Repository-Hinweise wider und kann sich ändern:

- Verbesserung der Firmware-/Hardware-Workflows für Omi und OmiGlass fortsetzen
- Ausbau von App-/Plugin-Ökosystem und Entwickler-Tooling
- Web-Erlebnisse für Memories/Apps/Personas verbessern
- MCP + SDK-Integrationen für externe Agenten-Ökosysteme stärken
- Mehrsprachige README-Varianten in `i18n/` ergänzen und pflegen

## Dokumentation

- [Einführung](https://docs.omi.me/)
- [omi App Setup](https://docs.omi.me/doc/developer/AppSetup)
- [Kaufanleitung](https://docs.omi.me/doc/assembly/Buying_Guide/)
- [Gerät bauen](https://docs.omi.me/doc/assembly/Build_the_device/)
- [Firmware installieren](https://docs.omi.me/doc/get_started/Flash_device/)
- [Erstelle deine eigene App in 1 Minute](https://docs.omi.me/doc/developer/apps/Introduction)

## Beitrag

- Sieh dir unsere [Contribution-Guide](https://docs.omi.me/doc/developer/Contribution/)-Anleitung an.
- Verdiene mit Beiträgen mit! Siehe die [Paid Bounties 🤑](https://omi.me/bounties).
- Sieh dir die [aktuellen Issues](https://github.com/BasedHardware/Omi/issues) an.
- Tritt unserem [Discord](http://discord.omi.me) bei.
- Baue eigene [Plugins/Integrationen](https://docs.omi.me/doc/developer/apps/Introduction).

## Kontakt & Community

- Hauptseite: [omi.me](https://omi.me/)
- Downloads: [omi.me/download](https://omi.me/download)
- Dokumentation: [docs.omi.me](https://docs.omi.me/)
- Community-Chat: [discord.omi.me](http://discord.omi.me)
- Aktualisierungen verfolgen: [x.com/kodjima33](https://x.com/kodjima33)
- Hardware/Developer-Kits:
  - [Omi Dev Kit kaufen](https://www.omi.me/products/omi-dev-kit-2)
  - [Omi Glass Dev Kit kaufen](https://www.omi.me/glass)

## Lizenz

Omi ist verfügbar unter der <a href="https://github.com/BasedHardware/omi/blob/main/LICENSE">MIT-Lizenz</a>


## ❤️ Support

| Donate | PayPal | Stripe |
| --- | --- | --- |
| [![Donate](https://camo.githubusercontent.com/24a4914f0b42c6f435f9e101621f1e52535b02c225764b2f6cc99416926004b7/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f446f6e6174652d4c617a79696e674172742d3045413545393f7374796c653d666f722d7468652d6261646765266c6f676f3d6b6f2d6669266c6f676f436f6c6f723d7768697465)](https://chat.lazying.art/donate) | [![PayPal](https://camo.githubusercontent.com/d0f57e8b016517a4b06961b24d0ca87d62fdba16e18bbdb6aba28e978dc0ea21/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f50617950616c2d526f6e677a686f754368656e2d3030343537433f7374796c653d666f722d7468652d6261646765266c6f676f3d70617970616c266c6f676f436f6c6f723d7768697465)](https://paypal.me/RongzhouChen) | [![Stripe](https://camo.githubusercontent.com/1152dfe04b6943afe3a8d2953676749603fb9f95e24088c92c97a01a897b4942/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f5374726970652d446f6e6174652d3633354246463f7374796c653d666f722d7468652d6261646765266c6f676f3d737472697065266c6f676f436f6c6f723d7768697465)](https://buy.stripe.com/aFadR8gIaflgfQV6T4fw400) |
