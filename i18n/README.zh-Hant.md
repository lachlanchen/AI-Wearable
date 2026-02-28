[English](../README.md) · [العربية](README.ar.md) · [Español](README.es.md) · [Français](README.fr.md) · [日本語](README.ja.md) · [한국어](README.ko.md) · [Tiếng Việt](README.vi.md) · [中文 (简体)](README.zh-Hans.md) · [中文（繁體）](README.zh-Hant.md) · [Deutsch](README.de.md) · [Русский](README.ru.md)


<p align="center">
  <img src="https://raw.githubusercontent.com/lachlanchen/lachlanchen/main/logos/banner.png" alt="LazyingArt banner" />
</p>

<div align="center">

# **omi**

認識 Omi：全球領先的開源 AI 穿戴裝置，可捕捉對話、產生摘要與行動項目，並替你執行動作。只要將 Omi 連接到你的行動裝置，即可在任何地方自動取得高品質逐字稿，適用於會議、聊天與語音備忘錄。

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

## 目錄

- [概覽](#概覽)
- [功能特色](#功能特色)
- [快速開始（2 分鐘）](#快速開始2-分鐘)
- [專案結構](#專案結構)
- [先決條件](#先決條件)
- [安裝](#安裝)
- [使用方式](#使用方式)
- [設定](#設定)
- [範例](#範例)
- [開發備註](#開發備註)
- [疑難排解](#疑難排解)
- [路線圖](#路線圖)
- [文件](#文件)
- [貢獻](#貢獻)
- [支援與社群](#支援與社群)
- [授權](#授權)

## 概覽

此儲存庫是開源 Omi 生態系的 monorepo。

| 包含項目 | 說明 |
| --- | --- |
| Hardware/Firmware | Omi 穿戴裝置韌體與硬體資產 |
| Omi Glass | Omi Glass 韌體/硬體/app |
| Mobile | Flutter 伴隨 app |
| Backend | FastAPI 後端服務 |
| Web | Omi 主前端 + Personas |
| Ecosystem | 外掛/整合生態 |
| SDKs | Python、React Native、Swift |
| Agent Infra | MCP server |
| Docs | 文件來源 |

根目錄 README 的快速開始刻意聚焦於終端使用者/開發者 onboarding。完整的元件級設定位於各子專案 README 與 Omi docs。

## 功能特色

- ⚡ 即時 AI 音訊處理與轉錄流程
- 🔋 低功耗藍牙穿戴裝置工作流程
- 🧩 涵蓋韌體、app、後端、web 與 SDK 的開源軟體堆疊
- 🎙️ 以穿戴裝置優先的 UX，適用於會議、聊天與語音備忘錄
- 🔗 可透過 webhook/app 生態觸發自訂動作
- 🛠️ 外掛/整合架構，便於擴充能力

## 快速開始（2 分鐘）

### 1) 下載 omi App

[<img src='https://upload.wikimedia.org/wikipedia/commons/7/78/Google_Play_Store_badge_EN.svg' alt='Get it on Google Play' height="50px" width="180px">](https://play.google.com/store/apps/details?id=com.friend.ios)
[<img src='https://upload.wikimedia.org/wikipedia/commons/3/3c/Download_on_the_App_Store_Badge.svg' alt="Download on the App Store" height="50px" width="180px">](https://apps.apple.com/us/app/friend-ai-wearable/id6502156163)
[<img src='https://github.com/user-attachments/assets/59c47ec7-3da0-47d7-be2f-7467e4189499' alt="Download MacOS app" height="50px" width="180px">](https://apps.apple.com/us/app/omi-ai-smart-meeting-notes/id6502156163)

### 2) 建立一個 webhook

使用 [webhook.site](https://webhook.site) 建立 webhook，並複製此 URL。

<img src="https://github.com/user-attachments/assets/083a6ec4-4694-4c7a-843a-4a1a0c254453" width="500">

### 3) 在 omi App 中

| Explore => Create an App                                                                                  | Select Capability                                                                                       | Paste Webhook URL                                                                                         | Install App                                                                                             |
| --------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------- |
| <img src="https://github.com/user-attachments/assets/31809b81-7de2-4381-b5fc-5c9714972211" width="200"> | <img src="https://github.com/user-attachments/assets/59cfbe8e-7e3b-437f-81f7-25eb50ccdd7d" width="200"> | <img src="https://github.com/user-attachments/assets/3d864ee8-555f-4ded-b4db-87ff78128323" width = "200"> | <img src="https://github.com/user-attachments/assets/58cf6da6-e245-415e-92e7-dc1f46583cfc" width="200"> |

### 4) 開始說話並驗證事件

開始說話後，你會在 [webhook.site](https://webhook.site) 看到即時逐字稿。

## 專案結構

### 此儲存庫內包含

- [omi device](https://github.com/BasedHardware/omi/tree/main/omi)
- [omi glass](https://github.com/BasedHardware/omi/tree/main/omiGlass)
- [omi app](https://github.com/BasedHardware/omi/tree/main/app)
- [ai personas (web)](https://github.com/BasedHardware/omi/tree/main/web/personas-open-source)
- [SDKs](./sdks)

Note: older references may mention `personas-open-source` at repository root; in this repository it is currently under `web/personas-open-source`.

### 高階結構圖

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

## 先決條件

請依你要開發/使用的元件採用對應需求。

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

## 安裝

由於此專案為 monorepo，請按元件分別安裝。

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

## 使用方式

### 終端使用者 app 流程

1. 從上方商店連結安裝 Omi app。
2. 配對/使用你的 Omi 裝置。
3. 透過 webhook 快速開始流程建立 app。
4. 在你的 webhook endpoint 觀察即時逐字稿事件。

### 使用 app 搭配本機 backend

1. 在本機 `8000` 埠啟動 backend。
2. 透過 ngrok 靜態網域對外暴露本機 backend。
3. 將 app `BASE_API_URL` 設為你的 ngrok URL。
4. 讓 Omi app 連到你的本機 backend。

### SDK 工作流程

- Python SDK：使用 `omi-scan` 掃描 BLE 裝置、解碼 Opus 封包，並透過 Deepgram 轉錄。
- React Native SDK：連線、串流音訊位元組、檢查 codec/電量。
- Swift SDK (`omi-lib`)：使用 `OmiManager` APIs 掃描/連線/轉錄。

## 設定

設定依元件分散管理。請以各子專案 template/readme 為準。

- `backend/.env.template` -> backend API keys/infrastructure config
- `web/frontend/.env.template` -> web frontend env vars
- `app` environment values -> mobile app runtime configuration
- `mcp` env vars -> `OMI_API_KEY` and optional `OMI_API_BASE_URL`
- SDK-specific keys:
  - Python SDK uses `DEEPGRAM_API_KEY`
  - Personas uses Firebase/OpenRouter/RapidAPI/Mixpanel env vars

若你不確定哪些變數為必要，請先保留預設值，並先依該元件的 README 操作，再調整或移除值。

## 範例

### Webhook quick-start（來自 root 流程）

使用 [webhook.site](https://webhook.site)，在 Omi 安裝你的自訂 app，接著確認逐字稿事件即時出現。

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

## 開發備註

- CI/CD 與部署自動化設定於：
  - `.github/workflows/`
  - `codemagic.yaml`
- 根目錄 `scripts/pre-commit` 會格式化已 staged 檔案，涵蓋：
  - `app/` 中的 Dart
  - `backend/` 中的 Python
  - `omi/` 與 `omiGlass/` 中的 C/C++
- 儲存庫根目錄的 `Package.swift` 會從 `sdks/swift` 發佈 Swift 套件 `omi-lib`。
- `i18n/` 目錄已存在，保留給多語 README/內容變體。

## 疑難排解

- 本機 setup 遇到 backend model/network 問題：若碰到已知 SSL 下載問題，請套用 `backend/README.md` 記錄的 `ssl` workaround 後重試。
- App 無法連到本機 backend：確認 ngrok 網域正在運行，且 `BASE_API_URL` 指向完全一致的公開 URL。
- BLE 掃描問題：確認已授與平台藍牙權限（依情境可能是 Terminal/Xcode/Android app）。
- 舊文件路徑不一致：部分舊版 docs/reference 文字可能顯示過期路徑（例如 `personas-open-source` root path 或 `omi/OmiGlass` 大小寫）。在本 repo 請以本文件上方目前目錄結構為準。

## 路線圖

此區反映目前儲存庫訊號，後續可能調整：

- 持續改進 Omi 與 OmiGlass 的韌體/硬體工作流程
- 擴展 app/plugin 生態與開發者工具
- 改善 memories/apps/personas 的 web 體驗
- 強化 MCP + SDK 與外部 agent 生態的整合
- 在 `i18n/` 新增並維護多語 README 變體

## 文件

- [Introduction](https://docs.omi.me/)
- [omi App setup](https://docs.omi.me/doc/developer/AppSetup)
- [Buying Guide](https://docs.omi.me/doc/assembly/Buying_Guide/)
- [Build the device](https://docs.omi.me/doc/assembly/Build_the_device/)
- [Install firmware](https://docs.omi.me/doc/get_started/Flash_device/)
- [Create your own app in 1 minute](https://docs.omi.me/doc/developer/apps/Introduction)

## 貢獻

- 查看我們的 [contributions guide](https://docs.omi.me/doc/developer/Contribution/)。
- 貢獻也能獲得報酬！請看 [paid bounties 🤑](https://omi.me/bounties)。
- 查看 [current issues](https://github.com/BasedHardware/Omi/issues)。
- 加入 [Discord](http://discord.omi.me)。
- 建立你自己的 [Plugins/Integrations](https://docs.omi.me/doc/developer/apps/Introduction)。

## 支援與社群

- Main site: [omi.me](https://omi.me/)
- Downloads: [omi.me/download](https://omi.me/download)
- Docs: [docs.omi.me](https://docs.omi.me/)
- Community chat: [discord.omi.me](http://discord.omi.me)
- Follow updates: [x.com/kodjima33](https://x.com/kodjima33)
- Hardware/dev kits:
  - [Buy omi Dev Kit](https://www.omi.me/products/omi-dev-kit-2)
  - [Buy Omi Glass Dev Kit](https://www.omi.me/glass)

## 授權

Omi is available under <a href="https://github.com/BasedHardware/omi/blob/main/LICENSE">MIT License</a>
