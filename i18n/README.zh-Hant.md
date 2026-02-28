[English](../README.md) · [العربية](README.ar.md) · [Español](README.es.md) · [Français](README.fr.md) · [日本語](README.ja.md) · [한국어](README.ko.md) · [Tiếng Việt](README.vi.md) · [中文 (简体)](README.zh-Hans.md) · [中文（繁體）](README.zh-Hant.md) · [Deutsch](README.de.md) · [Русский](README.ru.md)


[![LazyingArt banner](https://github.com/lachlanchen/lachlanchen/raw/main/figs/banner.png)](https://github.com/lachlanchen/lachlanchen/blob/main/figs/banner.png)

<div align="center">

# **omi**

_AI 驅動的可穿戴裝置，適用於即時會議與聊天：隨時擷取、總結，並可自動採取行動——完全免手。

認識 Omi，全球領先的開源 AI 可穿戴裝置，能記錄對話、整理摘要、列出待辦，並幫你代為執行後續步驟。只要將 Omi 連接到行動裝置，即可在任何場景下自動產生高品質的會議、聊天與語音記事逐字稿。

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

## ⚡ 快速連結

| 資源 | 連結 |
| --- | --- |
| 🌐 專案網站 | [omi.me](https://omi.me/) |
| ⬇️ 下載中心 | [omi.me/download](https://omi.me/download) |
| 📚 文件 | [docs.omi.me](https://docs.omi.me/) |
| 🛠️ Omi Dev Kit | [購買 Omi Dev Kit](https://www.omi.me/products/omi-dev-kit-2) |
| 👓 Omi Glass Dev Kit | [購買 Omi Glass](https://www.omi.me/glass) |

---

## 目錄

- [📌 概覽](#概覽)
- [⚡️ 功能](#功能)
- [🚀 快速開始（2 分鐘）](#快速開始2-分鐘)
- [🏗️ 專案結構](#專案結構)
- [🧰 前置需求](#前置需求)
- [🛠️ 安裝](#安裝)
- [🧪 使用方式](#使用方式)
- [⚙️ 設定](#設定)
- [🧾 範例](#範例)
- [🧭 開發說明](#開發說明)
- [🐞 疑難排解](#疑難排解)
- [🗺️ 路線圖](#路線圖)
- [📚 文件](#文件)
- [🤝 貢獻](#貢獻)
- [❤️ Support](#%E2%9D%A4%EF%B8%8F-support)
- [💬 聯絡與社群](#聯絡與社群)
- [📜 授權](#授權)

## 概覽

此儲存庫是開源 Omi 生態系統的 monorepo。

| 含項 | 說明 |
| --- | --- |
| 🧠 Omi 硬體 | Omi 可穿戴設備韌體 + 硬體資源 |
| 🥽 Omi Glass | Omi Glass 韌體/硬體/應用程式 |
| 📱 行動端 | Flutter 配套應用 |
| 🌐 後端 | FastAPI 後端服務 |
| 🕸️ 網頁 | Omi 主前端 + Personas |
| 🧩 生態系統 | 外掛/整合生態 |
| 📦 SDK | Python、React Native、Swift |
| 🔗 Agent 基礎設施 | MCP 伺服器 |
| 📘 文件 | 文件原始資料 |

根 README 主要聚焦於導覽與日常開發流程。各元件的完整安裝與更深入的操作說明位於各子專案 README 及 `docs/`。

## 功能

- ⚡ 即時 AI 音訊處理與轉錄流程
- 🔋 低耗電 Bluetooth 可穿戴設備工作流程
- 🧩 跨韌體、應用、後端、網頁與 SDK 的開源軟體堆疊
- 🎙️ 以穿戴為先的會議、聊天與語音記事體驗
- 🔗 透過 Webhook/應用生態觸發自訂動作
- 🛠️ 外掛與整合架構，方便擴充能力

## 快速開始（2 分鐘）

### 1) 下載 Omi 應用

[<img src='https://upload.wikimedia.org/wikipedia/commons/7/78/Google_Play_Store_badge_EN.svg' alt='Get it on Google Play' height="50px" width="180px">](https://play.google.com/store/apps/details?id=com.friend.ios)
[<img src='https://upload.wikimedia.org/wikipedia/commons/3/3c/Download_on_the_App_Store_Badge.svg' alt="Download on the App Store" height="50px" width="180px">](https://apps.apple.com/us/app/friend-ai-wearable/id6502156163)
[<img src='https://github.com/user-attachments/assets/59c47ec7-3da0-47d7-be2f-7467e4189499' alt="Download MacOS app" height="50px" width="180px">](https://apps.apple.com/us/app/omi-ai-smart-meeting-notes/id6502156163)

### 2) 建立 webhook

使用 [webhook.site](https://webhook.site) 建立 webhook，並複製該 URL。

<img src="https://github.com/user-attachments/assets/083a6ec4-4694-4c7a-843a-4a1a0c254453" width="500">

### 3) 在 Omi 應用內

| 探索 => 建立應用 | 選擇能力 | 貼上 Webhook URL | 安裝應用 |
| --- | --- | --- | --- |
| <img src="https://github.com/user-attachments/assets/31809b81-7de2-4381-b5fc-5c9714972211" width="200"> | <img src="https://github.com/user-attachments/assets/59cfbe8e-7e3b-437f-81f7-25eb50ccdd7d" width="200"> | <img src="https://github.com/user-attachments/assets/3d864ee8-555f-4ded-b4db-87ff78128323" width="200"> | <img src="https://github.com/user-attachments/assets/58cf6da6-e245-415e-92e7-dc1f46583cfc" width="200"> |

### 4) 開始發聲並驗證事件

開始發聲後，你會在 [webhook.site](https://webhook.site) 上看到即時逐字稿事件。

## 專案結構

### 此儲存庫

| 元件 | 用途 |
| --- | --- |
| [omi device](https://github.com/BasedHardware/omi/tree/main/omi) | Omi 硬體 + 韌體 |
| [omi glass](https://github.com/BasedHardware/omi/tree/main/omiGlass) | Omi Glass 硬體 + 韌體 |
| [omi app](https://github.com/BasedHardware/omi/tree/main/app) | Flutter 配套應用 |
| [ai personas (web)](https://github.com/BasedHardware/omi/tree/main/web/personas-open-source) | Personas 網頁應用 |
| [SDKs](./sdks) | Python、React Native、Swift SDK |

注意：舊文件可能仍提及在儲存庫根目錄中的 `personas-open-source`，但本專案目前位於 `web/personas-open-source`。

### 高階架構圖

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

## 前置需求

依你要處理的目標元件，安裝對應需求。

| 工具 | 用途 |
| --- | --- |
| Git | 版本控制 |
| Node.js 18+ 與 npm | Web、Personas、部分外掛工作流 |
| Python 3.10+ | 後端、MCP、Python SDK |
| Flutter SDK | 行動應用 |
| Xcode/CocoaPods | iOS 開發 |
| Android Studio + Android SDK | Android 開發 |
| `ffmpeg` + `opus` | 後端/音訊流程 |
| Docker（選用） | MCP/web 部署 |
| Google Cloud + Firebase | 後端/應用流程 |

### 安裝前假設

- 部分指令會依賴外部憑證（Firebase、OpenAI/Deepgram/API 提供者），通常以各元件的 `.env` 範本個別設定。若本機文件缺欄位，請參考該元件 README。
- 如果你只需要某個介面，請只安裝與建置該元件，讓迭代更快。

## 安裝

因為這是 monorepo，請按元件分開安裝。

### 複製儲存庫

```bash
git clone https://github.com/BasedHardware/omi.git
cd omi
```

### 應用程式（Flutter）

```bash
cd app
bash setup.sh ios
# 或
bash setup.sh android

flutter run --flavor dev
```

### 後端（FastAPI）

```bash
cd backend
cp .env.template .env
pip install -r requirements.txt
uvicorn main:app --reload --env-file .env
```

### 主前端（Next.js）

```bash
cd web/frontend
npm install
cp .env.template .env.local
npm run dev
```

### Personas 網頁應用（Next.js）

```bash
cd web/personas-open-source
npm install
npm run dev
```

### MCP 伺服器

```bash
cd mcp
# 請參考 mcp/README.md 了解以 Docker 為基礎的 Claude Desktop 設定
```

### SDKs

```bash
cd sdks/python && pip install -e .
cd ../react-native && npm install
# Swift 套件由根目錄的 Package.swift 以 `omi-lib` 方式提供
```

## 使用方式

### 一般使用者 App 流程

1. 透過上方商店連結安裝 Omi 應用。
2. 配對並使用你的 Omi 裝置。
3. 依 webhook 快速上手流程建立應用。
4. 開始說話，並在你的 webhook 端點即時查看逐字稿事件。

### 本地後端 + App 搭配

1. 在本機啟動後端，埠號為 `8000`。
2. 使用 ngrok 靜態網域公開本地後端。
3. 將應用的 `BASE_API_URL` 設定為你的 ngrok URL。
4. 使用 Omi 應用連接本地後端。

### SDK 工作流程

- Python SDK：使用 `omi-scan` 掃描 BLE 裝置、解碼 Opus 封包，並透過 Deepgram 進行轉錄。
- React Native SDK：連線、串流音訊位元組、檢查 codec 與電池狀態。
- Swift SDK（`omi-lib`）：使用 `OmiManager` API 掃描、連線與轉錄。

## 配置

配置按元件分佈。各子專案的 template/readme 為權威依據。

- `backend/.env.template` -> 後端 API 金鑰與基礎架構設定
- `web/frontend/.env.template` -> 網頁前端環境變數
- `app` 環境值 -> 行動應用執行時設定
- `mcp` 環境變數 -> `OMI_API_KEY` 與可選 `OMI_API_BASE_URL`
- SDK 特定變數：
  - Python SDK 使用 `DEEPGRAM_API_KEY`
  - Personas 使用 Firebase/OpenRouter/RapidAPI/Mixpanel 的環境變數

如果不確定哪些變數必填，請保留預設值，並在刪除/變更前先依該元件 README 確認。

## 範例

### Webhook 快速開始（根目錄流程）

使用 [webhook.site](https://webhook.site)，在 Omi 安裝你的自訂應用，然後確認逐字稿事件是否即時出現。

### 後端執行指令

```bash
cd backend
uvicorn main:app --reload --env-file .env
```

### 前端執行指令

```bash
cd web/frontend
npm run dev
```

### Python SDK 掃描

```bash
cd sdks/python
omi-scan
```

## 開發說明

- CI/CD 與部署自動化設定在：
  - `.github/workflows/`
  - `codemagic.yaml`
- 根目錄 `scripts/pre-commit` 會格式化以下內容：
  - `app/` 下的 Dart
  - `backend/` 下的 Python
  - `omi/` 和 `omiGlass/` 下的 C/C++
- 根目錄 `Package.swift` 從 `sdks/swift` 公佈 Swift 套件 `omi-lib`。
- `i18n/` 目錄存在並保留多語言 README/內容變體。

## 疑難排解

- 本地端後端模型/網路問題：若遇到已知的 SSL 下載問題，請套用 `backend/README.md` 中的 `ssl` 臨時解法後重試。
- App 無法連上本地後端：請確認 ngrok 網域已啟動，且 `BASE_API_URL` 指向完全相同的公開 URL。
- BLE 發現問題：確認對應平台藍牙權限已授權（依情境在 Terminal/Xcode/Android 應用）。
- 路徑不一致：某些舊文件可能仍使用舊路徑（如根目錄中的 `personas-open-source`、`omi/OmiGlass` 大小寫）。本庫請使用上方顯示的目前目錄結構。

## 路線圖

此區段依據目前儲存庫訊號彙整，未來可能調整：

- 持續改進 Omi 與 OmiGlass 的韌體/硬體流程
- 擴充 App/外掛生態與開發者工具鏈
- 改善 memories/apps/personas 的網站體驗
- 加強 MCP + SDK 與外部智能代理生態的整合
- 在 `i18n/` 中新增並維護多語言 README 變體

## 文件

- [Introduction](https://docs.omi.me/)
- [omi App setup](https://docs.omi.me/doc/developer/AppSetup)
- [Buying Guide](https://docs.omi.me/doc/assembly/Buying_Guide/)
- [Build the device](https://docs.omi.me/doc/assembly/Build_the_device/)
- [Install firmware](https://docs.omi.me/doc/get_started/Flash_device/)
- [Create your own app in 1 minute](https://docs.omi.me/doc/developer/apps/Introduction)

## 貢獻

- 查看我們的 [contribution guide](https://docs.omi.me/doc/developer/Contribution/)。
- 從貢獻中獲得酬勞！查看 [有償賞金 🤑](https://omi.me/bounties)。
- 查看 [目前 issue](https://github.com/BasedHardware/Omi/issues)。
- 加入 [Discord](http://discord.omi.me)。
- 建置你自己的 [Plugins/Integrations](https://docs.omi.me/doc/developer/apps/Introduction)。

## 聯絡與社群

- 官方網站：[omi.me](https://omi.me/)
- 下載： [omi.me/download](https://omi.me/download)
- 文件：[docs.omi.me](https://docs.omi.me/)
- 社群聊天室：[discord.omi.me](http://discord.omi.me)
- 追蹤更新：[x.com/kodjima33](https://x.com/kodjima33)
- 硬體/開發套件：
  - [購買 Omi Dev Kit](https://www.omi.me/products/omi-dev-kit-2)
  - [購買 Omi Glass Dev Kit](https://www.omi.me/glass)

## 授權

Omi 採用 <a href="https://github.com/BasedHardware/omi/blob/main/LICENSE">MIT 授權條款</a>


## ❤️ Support

| Donate | PayPal | Stripe |
| --- | --- | --- |
| [![Donate](https://camo.githubusercontent.com/24a4914f0b42c6f435f9e101621f1e52535b02c225764b2f6cc99416926004b7/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f446f6e6174652d4c617a79696e674172742d3045413545393f7374796c653d666f722d7468652d6261646765266c6f676f3d6b6f2d6669266c6f676f436f6c6f723d7768697465)](https://chat.lazying.art/donate) | [![PayPal](https://camo.githubusercontent.com/d0f57e8b016517a4b06961b24d0ca87d62fdba16e18bbdb6aba28e978dc0ea21/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f50617950616c2d526f6e677a686f754368656e2d3030343537433f7374796c653d666f722d7468652d6261646765266c6f676f3d70617970616c266c6f676f436f6c6f723d7768697465)](https://paypal.me/RongzhouChen) | [![Stripe](https://camo.githubusercontent.com/1152dfe04b6943afe3a8d2953676749603fb9f95e24088c92c97a01a897b4942/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f5374726970652d446f6e6174652d3633354246463f7374796c653d666f722d7468652d6261646765266c6f676f3d737472697065266c6f676f436f6c6f723d7768697465)](https://buy.stripe.com/aFadR8gIaflgfQV6T4fw400) |
