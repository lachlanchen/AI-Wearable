[English](../README.md) · [العربية](README.ar.md) · [Español](README.es.md) · [Français](README.fr.md) · [日本語](README.ja.md) · [한국어](README.ko.md) · [Tiếng Việt](README.vi.md) · [中文 (简体)](README.zh-Hans.md) · [中文（繁體）](README.zh-Hant.md) · [Deutsch](README.de.md) · [Русский](README.ru.md)


[![LazyingArt banner](https://github.com/lachlanchen/lachlanchen/raw/main/figs/banner.png)](https://github.com/lachlanchen/lachlanchen/blob/main/figs/banner.png)

<div align="center">

# **omi**

_AI-powered wearable for instant meetings and chats: capture, summarize, and act—hands-free._

즉시 회의와 채팅을 지원하는 AI 웨어러블로, 대화를 캡처하고 요약한 뒤 손을 뗀 채로 바로 실행까지 이어줍니다.

회의, 채팅, 음성 메모를 어디에서나 자동으로 고품질 기록으로 남겨주며, Omi는 대화를 요약하고 실행 가능한 액션을 생성하는 세계적인 오픈소스 AI 웨어러블입니다. Omi를 모바일 기기에 연결하기만 하면 바로 고품질 실시간 전사를 사용할 수 있습니다.

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

## ⚡ 빠른 링크

| 리소스 | 링크 |
| --- | --- |
| 🌐 프로젝트 사이트 | [omi.me](https://omi.me/) |
| ⬇️ 다운로드 센터 | [omi.me/download](https://omi.me/download) |
| 📚 문서 | [docs.omi.me](https://docs.omi.me/) |
| 🛠️ Omi Dev Kit | [Omi Dev Kit 구매](https://www.omi.me/products/omi-dev-kit-2) |
| 👓 Omi Glass Dev Kit | [Omi Glass 구매](https://www.omi.me/glass) |

## 목차

- [📌 개요](#개요)
- [⚡️ 기능](#기능)
- [🚀 빠른 시작 (2분)](#빠른-시작-2분)
- [🏗️ 프로젝트 구조](#프로젝트-구조)
- [🧰 필수 조건](#필수-조건)
- [🛠️ 설치](#설치)
- [🧪 사용법](#사용법)
- [⚙️ 설정](#설정)
- [🧾 예시](#예시)
- [🧭 개발 노트](#개발-노트)
- [🐞 문제 해결](#문제-해결)
- [🗺️ 로드맵](#로드맵)
- [📚 문서](#문서)
- [🤝 기여](#기여)
- [❤️ Support](#%E2%9D%A4%EF%B8%8F-support)
- [💬 문의 및 커뮤니티](#문의-및-커뮤니티)
- [📜 라이선스](#라이선스)

## 개요

이 저장소는 Omi 생태계의 오픈소스 모노레포입니다.

| 포함 항목 | 상세 설명 |
| --- | --- |
| 🧠 Omi Hardware | Omi 웨어러블 펌웨어 + 하드웨어 자산 |
| 🥽 Omi Glass | Omi Glass 펌웨어/하드웨어/앱 |
| 📱 Mobile | Flutter 동반 앱 |
| 🌐 Backend | FastAPI 백엔드 서비스 |
| 🕸️ Web | 메인 Omi 프론트엔드 + Personas |
| 🧩 Ecosystem | 플러그인/통합 생태계 |
| 📦 SDKs | Python, React Native, Swift |
| 🔗 Agent Infra | MCP 서버 |
| 📘 Docs | 문서 소스 |

루트 README는 온보딩과 일상적인 개발자 워크플로우에 초점을 둡니다. 컴포넌트별 상세 설정과 운영 노트는 각 하위 프로젝트 README와 `docs/`에 존재합니다.

## 기능

- ⚡ 실시간 AI 오디오 처리 및 전사 플로우
- 🔋 저전력 Bluetooth 웨어러블 디바이스 워크플로우
- 🧩 펌웨어, 앱, 백엔드, 웹, SDK 전 영역의 오픈소스 스택
- 🎙️ 회의, 채팅, 음성 메모에 맞춘 웨어러블 퍼스트 UX
- 🔗 사용자 맞춤 액션을 실행할 수 있는 Webhook/앱 생태계
- 🛠️ 기능 확장을 위한 플러그인 및 통합 아키텍처

## 🚀 빠른 시작 (2분)

### 1) Omi 앱 다운로드

[<img src='https://upload.wikimedia.org/wikipedia/commons/7/78/Google_Play_Store_badge_EN.svg' alt='Get it on Google Play' height="50px" width="180px">](https://play.google.com/store/apps/details?id=com.friend.ios)
[<img src='https://upload.wikimedia.org/wikipedia/commons/3/3c/Download_on_the_App_Store_Badge.svg' alt="Download on the App Store" height="50px" width="180px">](https://apps.apple.com/us/app/friend-ai-wearable/id6502156163)
[<img src='https://github.com/user-attachments/assets/59c47ec7-3da0-47d7-be2f-7467e4189499' alt="Download MacOS app" height="50px" width="180px">](https://apps.apple.com/us/app/omi-ai-smart-meeting-notes/id6502156163)

### 2) Webhook 만들기

[webhook.site](https://webhook.site)에서 webhook을 생성한 뒤 URL을 복사하세요.

<img src="https://github.com/user-attachments/assets/083a6ec4-4694-4c7a-843a-4a1a0c254453" width="500">

### 3) Omi 앱에서 설정

| 탐색 => 앱 생성 | 기능 선택 | Webhook URL 붙여넣기 | 앱 설치 |
| --- | --- | --- | --- |
| <img src="https://github.com/user-attachments/assets/31809b81-7de2-4381-b5fc-5c9714972211" width="200"> | <img src="https://github.com/user-attachments/assets/59cfbe8e-7e3b-437f-81f7-25eb50ccdd7d" width="200"> | <img src="https://github.com/user-attachments/assets/3d864ee8-555f-4ded-b4db-87ff78128323" width="200"> | <img src="https://github.com/user-attachments/assets/58cf6da6-e245-415e-92e7-dc1f46583cfc" width="200"> |

### 4) 말하기 및 이벤트 확인

말하기를 시작하면 [webhook.site](https://webhook.site)에서 실시간 전사 이벤트를 확인할 수 있습니다.

## 프로젝트 구조

### 이 저장소 안에서

| 구성 요소 | 용도 |
| --- | --- |
| [omi device](https://github.com/BasedHardware/omi/tree/main/omi) | Omi 하드웨어 + 펌웨어 |
| [omi glass](https://github.com/BasedHardware/omi/tree/main/omiGlass) | Omi Glass 하드웨어 + 펌웨어 |
| [omi app](https://github.com/BasedHardware/omi/tree/main/app) | Flutter 동반 애플리케이션 |
| [ai personas (web)](https://github.com/BasedHardware/omi/tree/main/web/personas-open-source) | Personas 웹 앱 |
| [SDKs](./sdks) | Python, React Native, Swift SDK |

참고: 이전 문서에는 리포지토리 루트에 `personas-open-source`가 있다고 되어 있을 수 있습니다. 현재는 `web/personas-open-source` 아래에 있습니다.

### 전체 구성도

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

## 필수 조건

대상 컴포넌트에 맞는 요구사항을 준비합니다.

| 도구 | 용도 |
| --- | --- |
| Git | 소스 제어 |
| Node.js 18+ 및 npm | 웹, personas, 일부 플러그인 워크플로 |
| Python 3.10+ | 백엔드, MCP, Python SDK |
| Flutter SDK | 모바일 앱 |
| Xcode/CocoaPods | iOS 개발 |
| Android Studio + Android SDK | Android 개발 |
| `ffmpeg` + `opus` | 백엔드/오디오 워크플로 |
| Docker (선택) | MCP/web 배포 |
| Google Cloud + Firebase | 백엔드/앱 워크플로 |

### 설치 전 가정 조건

- 일부 명령은 외부 자격 증명(Firebase, OpenAI/Deepgram/API 제공자)에 의존합니다. 보통 각 컴포넌트의 `.env` 템플릿에서 구성합니다. 값이 누락된 경우 해당 컴포넌트 README를 확인하세요.
- 특정 인터페이스만 필요하면 해당 컴포넌트만 설치/빌드해 반복 속도를 빠르게 유지하세요.

## 설치

이 저장소는 모노레포이므로 컴포넌트별로 설치합니다.

### 저장소 클론

```bash
git clone https://github.com/BasedHardware/omi.git
cd omi
```

### 앱 (Flutter)

```bash
cd app
bash setup.sh ios
# 또는
bash setup.sh android

flutter run --flavor dev
```

### 백엔드 (FastAPI)

```bash
cd backend
cp .env.template .env
pip install -r requirements.txt
uvicorn main:app --reload --env-file .env
```

### 메인 프론트엔드 (Next.js)

```bash
cd web/frontend
npm install
cp .env.template .env.local
npm run dev
```

### Personas 웹 앱 (Next.js)

```bash
cd web/personas-open-source
npm install
npm run dev
```

### MCP 서버

```bash
cd mcp
# Docker 기반 Claude Desktop 설정은 mcp/README.md를 참고하세요
```

### SDKs

```bash
cd sdks/python && pip install -e .
cd ../react-native && npm install
# Swift 패키지는 루트의 Package.swift에서 `omi-lib`로 노출됩니다
```

## 사용법

### 최종 사용자 앱 흐름

1. 위의 스토어 링크에서 Omi 앱을 설치합니다.
2. Omi 장치를 페어링하고 사용합니다.
3. webhook 빠른 시작 흐름으로 앱을 생성합니다.
4. 말하기를 시작하고 webhook 엔드포인트에서 실시간 전사 이벤트가 표시되는지 확인합니다.

### 로컬 백엔드 + 앱 사용

1. 로컬에서 백엔드를 `8000` 포트로 시작합니다.
2. ngrok 고정 도메인으로 로컬 백엔드를 노출합니다.
3. 앱의 `BASE_API_URL`을 ngrok URL로 설정합니다.
4. Omi 앱에서 로컬 백엔드를 사용합니다.

### SDK 워크플로우

- Python SDK: `omi-scan`으로 BLE 디바이스를 스캔하고 Opus 패킷을 디코드해 Deepgram으로 전사합니다.
- React Native SDK: 연결, 오디오 바이트 스트리밍, codec/배터리 상태 점검
- Swift SDK (`omi-lib`): `OmiManager` API를 사용해 스캔/연결/전사 수행

## 설정

설정은 컴포넌트별로 분리되어 있습니다. 각 하위 프로젝트의 템플릿/README를 기준으로 확인하세요.

- `backend/.env.template` -> backend API 키/인프라 설정
- `web/frontend/.env.template` -> 웹 프론트엔드 환경 변수
- `app` 환경 값 -> 모바일 앱 런타임 설정
- `mcp` 환경 변수 -> `OMI_API_KEY` 및 선택적 `OMI_API_BASE_URL`
- SDK별 키:
  - Python SDK는 `DEEPGRAM_API_KEY`
  - Personas는 Firebase/OpenRouter/RapidAPI/Mixpanel 환경 변수

필요한 변수가 무엇인지 불분명할 때는 기본값을 유지하고, 값을 삭제하거나 변경하기 전 대상 컴포넌트 README를 먼저 확인하세요.

## 예시

### Webhook 빠른 시작 (루트 플로우)

[webhook.site](https://webhook.site)를 사용해 Omi에 맞춤 앱을 설치한 다음, 전사 이벤트가 실시간으로 나타나는지 확인하세요.

### 백엔드 실행 명령

```bash
cd backend
uvicorn main:app --reload --env-file .env
```

### 프론트엔드 실행 명령

```bash
cd web/frontend
npm run dev
```

### Python SDK 스캔

```bash
cd sdks/python
omi-scan
```

## 개발 노트

- CI/CD 및 배포 자동화는 다음에서 설정됩니다.
  - `.github/workflows/`
  - `codemagic.yaml`
- 루트 `scripts/pre-commit`은 스테이징된 파일을 다음 대상으로 포맷합니다.
  - `app/`의 Dart
  - `backend/`의 Python
  - `omi/`와 `omiGlass/`의 C/C++
- 저장소 루트의 `Package.swift`는 `sdks/swift`의 Swift 패키지 `omi-lib`를 배포합니다.
- `i18n/` 디렉터리는 다국어 README/콘텐츠 변형을 위한 위치입니다.

## 문제 해결

- 로컬 설정에서 백엔드 모델/네트워크 문제가 발생하면: 알려진 SSL 다운로드 문제의 경우 `backend/README.md`에 문서화된 `ssl` 우회 절차를 적용한 뒤 재시도하세요.
- 앱이 로컬 백엔드에 연결되지 않으면: ngrok 도메인이 실행 중인지, `BASE_API_URL`이 해당 공개 URL을 정확히 가리키는지 확인하세요.
- BLE 검색 문제: 플랫폼별 Bluetooth 권한이 허용되었는지 확인하세요(터미널/Xcode/Android 앱).
- 기존 문서의 경로 불일치: 레거시 문서에는 오래된 경로가 남아 있을 수 있습니다(예: 루트 경로의 `personas-open-source`, `omi/OmiGlass` 대소문자). 이 저장소는 위의 현재 디렉터리 구조를 사용합니다.

## 로드맵

이 섹션은 현재 저장소 기준으로 작성되었으며, 변경될 수 있습니다.

- Omi와 OmiGlass의 펌웨어/하드웨어 워크플로 개선 지속
- 앱/플러그인 생태계 및 개발자 도구 확장
- memories/apps/personas 대상 웹 경험 개선
- 외부 에이전트 생태계에서 MCP + SDK 연동 강화
- `i18n/`에서 다국어 README 변형 추가 및 유지 보수

## 문서

- [Introduction](https://docs.omi.me/)
- [omi 앱 설정](https://docs.omi.me/doc/developer/AppSetup)
- [구매 가이드](https://docs.omi.me/doc/assembly/Buying_Guide/)
- [디바이스 조립](https://docs.omi.me/doc/assembly/Build_the_device/)
- [펌웨어 설치](https://docs.omi.me/doc/get_started/Flash_device/)
- [1분 만에 내 앱 만들기](https://docs.omi.me/doc/developer/apps/Introduction)

## 기여

- [기여 가이드](https://docs.omi.me/doc/developer/Contribution/)를 확인하세요.
- 기여로 수익을 얻을 수 있는 [유료 바운티 🤑](https://omi.me/bounties)를 확인하세요.
- [현재 이슈](https://github.com/BasedHardware/Omi/issues)를 확인하세요.
- [Discord](http://discord.omi.me)에 참여하세요.
- 나만의 [Plugins/Integrations](https://docs.omi.me/doc/developer/apps/Introduction)을 만들어 보세요.

## 문의 및 커뮤니티

- 메인 사이트: [omi.me](https://omi.me/)
- 다운로드: [omi.me/download](https://omi.me/download)
- 문서: [docs.omi.me](https://docs.omi.me/)
- 커뮤니티 채팅: [discord.omi.me](http://discord.omi.me)
- 업데이트 확인: [x.com/kodjima33](https://x.com/kodjima33)
- 하드웨어/개발 키트:
  - [Omi Dev Kit 구매](https://www.omi.me/products/omi-dev-kit-2)
  - [Omi Glass Dev Kit 구매](https://www.omi.me/glass)

## 라이선스

Omi는 <a href="https://github.com/BasedHardware/omi/blob/main/LICENSE">MIT 라이선스</a>로 제공됩니다.


## ❤️ Support

| Donate | PayPal | Stripe |
| --- | --- | --- |
| [![Donate](https://camo.githubusercontent.com/24a4914f0b42c6f435f9e101621f1e52535b02c225764b2f6cc99416926004b7/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f446f6e6174652d4c617a79696e674172742d3045413545393f7374796c653d666f722d7468652d6261646765266c6f676f3d6b6f2d6669266c6f676f436f6c6f723d7768697465)](https://chat.lazying.art/donate) | [![PayPal](https://camo.githubusercontent.com/d0f57e8b016517a4b06961b24d0ca87d62fdba16e18bbdb6aba28e978dc0ea21/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f50617950616c2d526f6e677a686f754368656e2d3030343537433f7374796c653d666f722d7468652d6261646765266c6f676f3d70617970616c266c6f676f436f6c6f723d7768697465)](https://paypal.me/RongzhouChen) | [![Stripe](https://camo.githubusercontent.com/1152dfe04b6943afe3a8d2953676749603fb9f95e24088c92c97a01a897b4942/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f5374726970652d446f6e6174652d3633354246463f7374796c653d666f722d7468652d6261646765266c6f676f3d737472697065266c6f676f436f6c6f723d7768697465)](https://buy.stripe.com/aFadR8gIaflgfQV6T4fw400) |
