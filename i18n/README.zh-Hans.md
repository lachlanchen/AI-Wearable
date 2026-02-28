[English](../README.md) · [العربية](README.ar.md) · [Español](README.es.md) · [Français](README.fr.md) · [日本語](README.ja.md) · [한국어](README.ko.md) · [Tiếng Việt](README.vi.md) · [中文 (简体)](README.zh-Hans.md) · [中文（繁體）](README.zh-Hant.md) · [Deutsch](README.de.md) · [Русский](README.ru.md)


[![LazyingArt banner](https://github.com/lachlanchen/lachlanchen/raw/main/figs/banner.png)](https://github.com/lachlanchen/lachlanchen/blob/main/figs/banner.png)

<div align="center">

# **omi**

_AI 驱动的可穿戴设备，适用于即时会议和聊天：随时采集、总结，并可自动执行操作——免提操作。_

Meet Omi，世界领先的开源 AI 可穿戴设备，能够记录对话、生成摘要和待办事项，并可为你执行后续操作。只需将 Omi 连接到移动设备，就能在任何场景下自动获得高质量的会议、聊天和语音备忘录转录。

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

## ⚡️ 快速链接

| 资源 | 链接 |
| --- | --- |
| 🌐 项目网站 | [omi.me](https://omi.me/) |
| ⬇️ 下载中心 | [omi.me/download](https://omi.me/download) |
| 📚 文档 | [docs.omi.me](https://docs.omi.me/) |
| 🛠️ Omi 开发者套件 | [购买 Omi Dev Kit](https://www.omi.me/products/omi-dev-kit-2) |
| 👓 Omi Glass 开发套件 | [购买 Omi Glass](https://www.omi.me/glass) |

---

## 目录

- [📌 概览](#概览)
- [⚡️ 特性](#特性)
- [🚀 快速开始（2 分钟）](#快速开始2-分钟)
- [🏗️ 项目结构](#项目结构)
- [🧰 前置要求](#前置要求)
- [🛠️ 安装](#安装)
- [🧪 使用](#使用)
- [⚙️ 配置](#配置)
- [🧾 示例](#示例)
- [🧭 开发说明](#开发说明)
- [🐞 故障排查](#故障排查)
- [🗺️ 路线图](#路线图)
- [📚 文档](#文档)
- [🤝 贡献](#贡献)
- [❤️ Support](#%E2%9D%A4%EF%B8%8F-support)
- [💬 联系与社区](#联系与社区)
- [📜 许可协议](#许可协议)

## 概览

此仓库是开源 Omi 生态系统 monorepo。

| 包含 | 详情 |
| --- | --- |
| 🧠 Omi 硬件 | Omi 可穿戴设备固件 + 硬件资产 |
| 🥽 Omi Glass | Omi Glass 固件/硬件/应用 |
| 📱 移动端 | Flutter 配套应用 |
| 🌐 后端 | FastAPI 后端服务 |
| 🕸️ 网站 | Omi 主前端 + Personas |
| 🧩 生态系统 | 插件/集成生态 |
| 📦 SDK | Python、React Native、Swift |
| 🔗 Agent 基础设施 | MCP 服务器 |
| 📘 文档 | 文档源文件 |

根 README 重点关注项目入门与日常开发流程。各组件的完整配置说明和更深入的运行细节位于各子项目 README 和 `docs/`。

## 特性

- ⚡ 实时 AI 音频处理与转录流程
- 🔋 低功耗蓝牙可穿戴设备工作流
- 🧩 覆盖固件、应用、后端、网站和 SDK 的开源软件栈
- 🎙️ 面向可穿戴的会议、聊天与语音备忘录体验
- 🔗 基于 Webhook/应用生态触发自定义动作
- 🛠️ 插件与集成架构，便于扩展能力

## 快速开始（2 分钟）

### 1) 下载 Omi 应用

[<img src='https://upload.wikimedia.org/wikipedia/commons/7/78/Google_Play_Store_badge_EN.svg' alt='Get it on Google Play' height="50px" width="180px">](https://play.google.com/store/apps/details?id=com.friend.ios)
[<img src='https://upload.wikimedia.org/wikipedia/commons/3/3c/Download_on_the_App_Store_Badge.svg' alt="Download on the App Store" height="50px" width="180px">](https://apps.apple.com/us/app/friend-ai-wearable/id6502156163)
[<img src='https://github.com/user-attachments/assets/59c47ec7-3da0-47d7-be2f-7467e4189499' alt="Download MacOS app" height="50px" width="180px">](https://apps.apple.com/us/app/omi-ai-smart-meeting-notes/id6502156163)

### 2) 创建 Webhook

使用 [webhook.site](https://webhook.site) 创建 Webhook，并复制该 URL。

<img src="https://github.com/user-attachments/assets/083a6ec4-4694-4c7a-843a-4a1a0c254453" width="500">

### 3) 在 Omi 应用内

| 探索 => 创建应用 | 选择能力 | 粘贴 Webhook URL | 安装应用 |
| --- | --- | --- | --- |
| <img src="https://github.com/user-attachments/assets/31809b81-7de2-4381-b5fc-5c9714972211" width="200"> | <img src="https://github.com/user-attachments/assets/59cfbe8e-7e3b-437f-81f7-25eb50ccdd7d" width="200"> | <img src="https://github.com/user-attachments/assets/3d864ee8-555f-4ded-b4db-87ff78128323" width="200"> | <img src="https://github.com/user-attachments/assets/58cf6da6-e245-415e-92e7-dc1f46583cfc" width="200"> |

### 4) 开始说话并校验事件

开始说话后，你会在 [webhook.site](https://webhook.site) 上看到实时转录事件。

## 项目结构

### 本仓库

| 组件 | 用途 |
| --- | --- |
| [omi device](https://github.com/BasedHardware/omi/tree/main/omi) | Omi 硬件 + 固件 |
| [omi glass](https://github.com/BasedHardware/omi/tree/main/omiGlass) | Omi Glass 硬件 + 固件 |
| [omi app](https://github.com/BasedHardware/omi/tree/main/app) | Flutter 配套应用 |
| [ai personas (web)](https://github.com/BasedHardware/omi/tree/main/web/personas-open-source) | Personas web 应用 |
| [SDKs](./sdks) | Python、React Native、Swift SDK |

注意：旧文档可能仍会提到仓库根目录中的 `personas-open-source`，但当前仓库该目录在 `web/personas-open-source`。

### 高层结构

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

## 前置要求

根据你要处理的目标组件选择所需内容。

| 工具 | 用途 |
| --- | --- |
| Git | 源码版本控制 |
| Node.js 18+ 与 npm | web、Personas、部分插件工作流 |
| Python 3.10+ | 后端、MCP、Python SDK |
| Flutter SDK | 移动应用 |
| Xcode/CocoaPods | iOS 开发 |
| Android Studio + Android SDK | Android 开发 |
| `ffmpeg` + `opus` | 后端/音频流程 |
| Docker（可选） | MCP/web 部署 |
| Google Cloud + Firebase | 后端/应用流程 |

### 安装前置假设

- 部分命令依赖外部凭据（Firebase、OpenAI/Deepgram/API 提供商），通常在各组件内使用其 `.env` 模板单独配置。若本地文档缺少字段，请参考对应组件的 README。
- 如果你只需要单一端，尽量只安装并构建该组件，以加快迭代。

## 安装

本仓库为 monorepo，按组件分别安装。

### 克隆仓库

```bash
git clone https://github.com/BasedHardware/omi.git
cd omi
```

### App（Flutter）

```bash
cd app
bash setup.sh ios
# or
bash setup.sh android

flutter run --flavor dev
```

### 后端（FastAPI）

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

### Personas web 应用（Next.js）

```bash
cd web/personas-open-source
npm install
npm run dev
```

### MCP 服务器

```bash
cd mcp
# 请参阅 mcp/README.md 获取基于 Docker 的 Claude Desktop 配置
```

### SDKs

```bash
cd sdks/python && pip install -e .
cd ../react-native && npm install
# Swift 包通过仓库根目录的 Package.swift 以 `omi-lib` 形式暴露
```

## 使用

### 终端用户 App 流程

1. 从上方商店链接安装 Omi 应用。
2. 配对并使用你的 Omi 设备。
3. 按照 Webhook 快速上手流程创建应用。
4. 开始说话，并在你的 webhook 端点查看实时转录事件。

### 本地后端 + App 联合使用

1. 在本地启动后端，端口 `8000`。
2. 使用 ngrok 静态域名公开本地后端。
3. 将应用的 `BASE_API_URL` 配置为你的 ngrok URL。
4. 使用 Omi 应用对接该本地后端。

### SDK 流程

- Python SDK：通过 `omi-scan` 扫描 BLE 设备、解码 Opus 数据包，并使用 Deepgram 转录。
- React Native SDK：连接设备、流式传输音频字节、检查 codec 与电量。
- Swift SDK（`omi-lib`）：通过 `OmiManager` API 扫描、连接和转录。

## 配置

配置按组件拆分。请以各子项目模板/README 为准。

- `backend/.env.template` -> 后端 API 密钥与基础设施配置
- `web/frontend/.env.template` -> 网站前端环境变量
- `app` 中的环境值 -> 移动应用运行时配置
- `mcp` 环境变量 -> `OMI_API_KEY` 与可选 `OMI_API_BASE_URL`
- SDK 特定变量：
  - Python SDK 使用 `DEEPGRAM_API_KEY`
  - Personas 使用 Firebase/OpenRouter/RapidAPI/Mixpanel 环境变量

如果你不确定哪些变量是必需项，请保留默认值，并在移除或修改前查阅该组件对应 README。

## 示例

### Webhook 快速上手（根目录流程）

使用 [webhook.site](https://webhook.site) 创建并在 Omi 中安装自定义应用，然后确认转录事件是否实时出现。

### 后端运行命令

```bash
cd backend
uvicorn main:app --reload --env-file .env
```

### 前端运行命令

```bash
cd web/frontend
npm run dev
```

### Python SDK 扫描

```bash
cd sdks/python
omi-scan
```

## 开发说明

- CI/CD 与部署自动化配置在：
  - `.github/workflows/`
  - `codemagic.yaml`
- 根目录 `scripts/pre-commit` 会对以下内容执行格式化：
  - `app/` 下的 Dart
  - `backend/` 下的 Python
  - `omi/` 和 `omiGlass/` 下的 C/C++
- 根目录 `Package.swift` 通过 `sdks/swift` 发布 Swift 包 `omi-lib`。
- `i18n/` 目录用于存放多语言 README 与内容变体。

## 故障排查

- 本地后端的模型/网络问题：若遇到已知的 SSL 下载问题，请按 `backend/README.md` 中记录的 `ssl` 变通方案处理后重试。
- App 无法访问本地后端：确认 ngrok 域名已运行，并且 `BASE_API_URL` 指向该公网 URL。
- BLE 发现问题：确认对应平台已授予蓝牙权限（按场景为 Terminal/Xcode/Android App）。
- 旧文档路径不一致：部分历史文档可能仍保留旧路径（例如根目录的 `personas-open-source` 或 `omi/OmiGlass` 的大小写）。请使用上文展示的当前目录结构。

## 路线图

本节反映仓库当前状态，后续可能调整：

- 持续改进 Omi 与 OmiGlass 的固件/硬件工作流
- 扩展 App/插件生态和开发者工具链
- 改进 memories/apps/personas 的网站体验
- 强化 MCP + SDK 与外部智能体生态的集成
- 在 `i18n/` 中新增并维护更多多语言 README 变体

## 文档

- [Introduction](https://docs.omi.me/)
- [omi App setup](https://docs.omi.me/doc/developer/AppSetup)
- [Buying Guide](https://docs.omi.me/doc/assembly/Buying_Guide/)
- [Build the device](https://docs.omi.me/doc/assembly/Build_the_device/)
- [Install firmware](https://docs.omi.me/doc/get_started/Flash_device/)
- [Create your own app in 1 minute](https://docs.omi.me/doc/developer/apps/Introduction)

## 贡献

- 查看我们的[贡献指南](https://docs.omi.me/doc/developer/Contribution/)。
- 参与贡献还能获得报酬：查看[有偿赏金 🤑](https://omi.me/bounties)。
- 查看[当前问题单](https://github.com/BasedHardware/Omi/issues)。
- 加入 [Discord](http://discord.omi.me)。
- 构建你自己的[插件/集成](https://docs.omi.me/doc/developer/apps/Introduction)。

## 联系与社区

- 官网：[omi.me](https://omi.me/)
- 下载：[omi.me/download](https://omi.me/download)
- 文档：[docs.omi.me](https://docs.omi.me/)
- 社区聊天：[discord.omi.me](http://discord.omi.me)
- 更新动态：[x.com/kodjima33](https://x.com/kodjima33)
- 硬件/开发套件：
  - [购买 Omi Dev Kit](https://www.omi.me/products/omi-dev-kit-2)
  - [购买 Omi Glass Dev Kit](https://www.omi.me/glass)

## 许可协议

Omi 采用 <a href="https://github.com/BasedHardware/omi/blob/main/LICENSE">MIT 许可协议</a>。


## ❤️ Support

| Donate | PayPal | Stripe |
| --- | --- | --- |
| [![Donate](https://camo.githubusercontent.com/24a4914f0b42c6f435f9e101621f1e52535b02c225764b2f6cc99416926004b7/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f446f6e6174652d4c617a79696e674172742d3045413545393f7374796c653d666f722d7468652d6261646765266c6f676f3d6b6f2d6669266c6f676f436f6c6f723d7768697465)](https://chat.lazying.art/donate) | [![PayPal](https://camo.githubusercontent.com/d0f57e8b016517a4b06961b24d0ca87d62fdba16e18bbdb6aba28e978dc0ea21/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f50617950616c2d526f6e677a686f754368656e2d3030343537433f7374796c653d666f722d7468652d6261646765266c6f676f3d70617970616c266c6f676f436f6c6f723d7768697465)](https://paypal.me/RongzhouChen) | [![Stripe](https://camo.githubusercontent.com/1152dfe04b6943afe3a8d2953676749603fb9f95e24088c92c97a01a897b4942/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f5374726970652d446f6e6174652d3633354246463f7374796c653d666f722d7468652d6261646765266c6f676f3d737472697065266c6f676f436f6c6f723d7768697465)](https://buy.stripe.com/aFadR8gIaflgfQV6T4fw400) |
