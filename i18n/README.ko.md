[English](../README.md) · [العربية](README.ar.md) · [Español](README.es.md) · [Français](README.fr.md) · [日本語](README.ja.md) · [한국어](README.ko.md) · [Tiếng Việt](README.vi.md) · [中文 (简体)](README.zh-Hans.md) · [中文（繁體）](README.zh-Hant.md) · [Deutsch](README.de.md) · [Русский](README.ru.md)


<p align="center">
  <img src="https://raw.githubusercontent.com/lachlanchen/lachlanchen/main/logos/banner.png" alt="LazyingArt banner" />
</p>

<div align="center">

# **omi**

Omi를 만나보세요. 대화를 기록하고, 요약과 액션 아이템을 제공하며, 실제 작업까지 수행해 주는 세계적인 오픈소스 AI 웨어러블입니다. Omi를 모바일 기기에 연결하면 어디서든 회의, 채팅, 음성 메모를 자동으로 고품질 전사로 받아볼 수 있습니다.

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

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Quick Start (2 min)](#quick-start-2-min)
- [Project Structure](#project-structure)
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Usage](#usage)
- [Configuration](#configuration)
- [Examples](#examples)
- [Development Notes](#development-notes)
- [Troubleshooting](#troubleshooting)
- [Roadmap](#roadmap)
- [Documentation](#documentation)
- [Contributions](#contributions)
- [Support and Community](#support-and-community)
- [License](#license)

## Overview

이 저장소는 오픈소스 Omi 생태계 모노레포입니다.

| Includes | Details |
| --- | --- |
| Hardware/Firmware | Omi 웨어러블 펌웨어 + 하드웨어 에셋 |
| Omi Glass | Omi Glass 펌웨어/하드웨어/앱 |
| Mobile | Flutter 컴패니언 앱 |
| Backend | FastAPI 백엔드 서비스 |
| Web | 메인 Omi 프론트엔드 + Personas |
| Ecosystem | 플러그인/통합 생태계 |
| SDKs | Python, React Native, Swift |
| Agent Infra | MCP 서버 |
| Docs | 문서 소스 |

루트 README의 빠른 시작은 최종 사용자/개발자 온보딩에 초점을 맞추고 있습니다. 컴포넌트별 상세 설정은 각 하위 프로젝트의 README와 Omi 문서를 참고하세요.

## Features

- ⚡ 실시간 AI 오디오 처리 및 전사 플로우
- 🔋 저전력 Bluetooth 웨어러블 디바이스 워크플로
- 🧩 펌웨어, 앱, 백엔드, 웹, SDK 전반을 아우르는 오픈소스 소프트웨어 스택
- 🎙️ 회의, 채팅, 음성 메모에 최적화된 웨어러블 중심 UX
- 🔗 커스텀 액션 트리거를 위한 웹훅/앱 생태계
- 🛠️ 기능 확장을 위한 플러그인/통합 아키텍처

## Quick Start (2 min)

### 1) omi App 다운로드

[<img src='https://upload.wikimedia.org/wikipedia/commons/7/78/Google_Play_Store_badge_EN.svg' alt='Get it on Google Play' height="50px" width="180px">](https://play.google.com/store/apps/details?id=com.friend.ios)
[<img src='https://upload.wikimedia.org/wikipedia/commons/3/3c/Download_on_the_App_Store_Badge.svg' alt="Download on the App Store" height="50px" width="180px">](https://apps.apple.com/us/app/friend-ai-wearable/id6502156163)
[<img src='https://github.com/user-attachments/assets/59c47ec7-3da0-47d7-be2f-7467e4189499' alt="Download MacOS app" height="50px" width="180px">](https://apps.apple.com/us/app/omi-ai-smart-meeting-notes/id6502156163)

### 2) 웹훅 만들기

[webhook.site](https://webhook.site)에서 웹훅을 생성하고 해당 URL을 복사하세요.

<img src="https://github.com/user-attachments/assets/083a6ec4-4694-4c7a-843a-4a1a0c254453" width="500">

### 3) omi App에서 설정

| Explore => Create an App                                                                                  | Select Capability                                                                                       | Paste Webhook URL                                                                                         | Install App                                                                                             |
| --------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------- |
| <img src="https://github.com/user-attachments/assets/31809b81-7de2-4381-b5fc-5c9714972211" width="200"> | <img src="https://github.com/user-attachments/assets/59cfbe8e-7e3b-437f-81f7-25eb50ccdd7d" width="200"> | <img src="https://github.com/user-attachments/assets/3d864ee8-555f-4ded-b4db-87ff78128323" width = "200"> | <img src="https://github.com/user-attachments/assets/58cf6da6-e245-415e-92e7-dc1f46583cfc" width="200"> |

### 4) 말하고 이벤트 확인하기

말하기를 시작하면 [webhook.site](https://webhook.site)에서 실시간 전사 결과를 확인할 수 있습니다.

## Project Structure

### 이 저장소에 포함된 항목

- [omi device](https://github.com/BasedHardware/omi/tree/main/omi)
- [omi glass](https://github.com/BasedHardware/omi/tree/main/omiGlass)
- [omi app](https://github.com/BasedHardware/omi/tree/main/app)
- [ai personas (web)](https://github.com/BasedHardware/omi/tree/main/web/personas-open-source)
- [SDKs](./sdks)

참고: 과거 문서에서는 `personas-open-source`가 저장소 루트에 있다고 언급할 수 있습니다. 현재 이 저장소에서는 `web/personas-open-source` 아래에 있습니다.

### 상위 구조 맵

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

## Prerequisites

대상 컴포넌트에 맞는 요구 사항만 준비하세요.

| Tooling | Used for |
| --- | --- |
| Git | 소스 제어 |
| Node.js 18+ and npm | web, personas, 일부 플러그인 워크플로 |
| Python 3.10+ | backend, MCP, Python SDK |
| Flutter SDK | 모바일 앱 |
| Xcode/CocoaPods | iOS 개발 |
| Android Studio + Android SDK | Android 개발 |
| `ffmpeg` + `opus` | backend/audio 워크플로 |
| Docker (optional) | MCP/web 배포 |
| Google Cloud + Firebase | backend/app 워크플로 |

## Installation

모노레포이므로 컴포넌트별로 설치합니다.

### 저장소 클론

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

### 최종 사용자 앱 흐름

1. 위 스토어 링크에서 Omi 앱을 설치합니다.
2. Omi 디바이스를 페어링하고 사용합니다.
3. 웹훅 빠른 시작 흐름을 통해 앱을 생성합니다.
4. 말하고 웹훅 엔드포인트에서 실시간 전사 이벤트를 확인합니다.

### 앱과 함께 로컬 백엔드 사용

1. 로컬에서 `8000` 포트로 백엔드를 실행합니다.
2. ngrok 정적 도메인으로 로컬 백엔드를 노출합니다.
3. 앱의 `BASE_API_URL`을 ngrok URL로 설정합니다.
4. 로컬 백엔드에 연결된 Omi 앱을 사용합니다.

### SDK 워크플로

- Python SDK: `omi-scan`으로 BLE 디바이스를 스캔하고, Opus 패킷을 디코드한 뒤, Deepgram으로 전사합니다.
- React Native SDK: 연결 후 오디오 바이트를 스트리밍하고 코덱/배터리 정보를 확인합니다.
- Swift SDK (`omi-lib`): `OmiManager` API를 사용해 스캔/연결/전사를 수행합니다.

## Configuration

설정은 컴포넌트별로 분산되어 있습니다. 각 하위 프로젝트의 템플릿/README를 기준으로 확인하세요.

- `backend/.env.template` -> backend API 키/인프라 설정
- `web/frontend/.env.template` -> web frontend 환경 변수
- `app` environment values -> 모바일 앱 런타임 설정
- `mcp` env vars -> `OMI_API_KEY` 및 선택적 `OMI_API_BASE_URL`
- SDK별 키:
  - Python SDK uses `DEEPGRAM_API_KEY`
  - Personas uses Firebase/OpenRouter/RapidAPI/Mixpanel env vars

필수 변수 판단이 어렵다면 기본값을 유지하고, 값을 삭제/변경하기 전에 해당 컴포넌트의 README를 먼저 따르세요.

## Examples

### 웹훅 빠른 시작(루트 플로우)

[webhook.site](https://webhook.site)를 사용해 커스텀 앱을 Omi에 설치한 뒤, 전사 이벤트가 실시간으로 표시되는지 확인하세요.

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

- CI/CD 및 배포 자동화는 다음에 구성되어 있습니다:
  - `.github/workflows/`
  - `codemagic.yaml`
- 루트 `scripts/pre-commit`은 다음 경로의 staged 파일 포맷팅을 수행합니다:
  - `app/`의 Dart
  - `backend/`의 Python
  - `omi/` 및 `omiGlass/`의 C/C++
- 저장소 루트의 `Package.swift`는 `sdks/swift`의 Swift 패키지 `omi-lib`를 배포합니다.
- `i18n/` 디렉터리는 다국어 README/콘텐츠 변형을 위해 존재하며 예약되어 있습니다.

## Troubleshooting

- 로컬 설정에서 백엔드 모델/네트워크 문제가 발생하는 경우: 알려진 SSL 다운로드 이슈가 나타나면 `backend/README.md`에 문서화된 `ssl` 우회 방법을 적용한 뒤 다시 시도하세요.
- 앱이 로컬 백엔드에 연결되지 않는 경우: ngrok 도메인이 실행 중인지, 그리고 `BASE_API_URL`이 해당 공개 URL과 정확히 일치하는지 확인하세요.
- BLE 검색 문제가 있는 경우: 플랫폼별 Bluetooth 권한(Terminal/Xcode/Android 앱)을 부여했는지 확인하세요.
- 오래된 문서의 경로 불일치: 일부 레거시 문서/참조 텍스트에는 구식 경로(예: `personas-open-source` 루트 경로, `omi/OmiGlass` 대소문자)가 표시될 수 있습니다. 이 저장소에서는 위에 제시된 현재 디렉터리 레이아웃을 기준으로 사용하세요.

## Roadmap

이 섹션은 현재 저장소 신호를 반영하며 향후 변경될 수 있습니다:

- Omi 및 OmiGlass의 펌웨어/하드웨어 워크플로 지속 개선
- 앱/플러그인 생태계와 개발자 도구 확장
- memories/apps/personas를 위한 웹 경험 개선
- 외부 에이전트 생태계를 위한 MCP + SDK 통합 강화
- `i18n/`의 다국어 README 변형 추가 및 유지

## Documentation

- [Introduction](https://docs.omi.me/)
- [omi App setup](https://docs.omi.me/doc/developer/AppSetup)
- [Buying Guide](https://docs.omi.me/doc/assembly/Buying_Guide/)
- [Build the device](https://docs.omi.me/doc/assembly/Build_the_device/)
- [Install firmware](https://docs.omi.me/doc/get_started/Flash_device/)
- [Create your own app in 1 minute](https://docs.omi.me/doc/developer/apps/Introduction)

## Contributions

- [contributions guide](https://docs.omi.me/doc/developer/Contribution/)를 확인하세요.
- 기여로 보상을 받을 수 있습니다. [paid bounties 🤑](https://omi.me/bounties)를 확인하세요.
- [current issues](https://github.com/BasedHardware/Omi/issues)를 확인하세요.
- [Discord](http://discord.omi.me)에 참여하세요.
- 직접 [Plugins/Integrations](https://docs.omi.me/doc/developer/apps/Introduction)를 만들어보세요.

## Support and Community

- Main site: [omi.me](https://omi.me/)
- Downloads: [omi.me/download](https://omi.me/download)
- Docs: [docs.omi.me](https://docs.omi.me/)
- Community chat: [discord.omi.me](http://discord.omi.me)
- Follow updates: [x.com/kodjima33](https://x.com/kodjima33)
- Hardware/dev kits:
  - [Buy omi Dev Kit](https://www.omi.me/products/omi-dev-kit-2)
  - [Buy Omi Glass Dev Kit](https://www.omi.me/glass)

## License

Omi는 <a href="https://github.com/BasedHardware/omi/blob/main/LICENSE">MIT License</a>로 제공됩니다.
