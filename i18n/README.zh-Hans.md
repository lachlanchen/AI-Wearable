[English](../README.md) · [العربية](README.ar.md) · [Español](README.es.md) · [Français](README.fr.md) · [日本語](README.ja.md) · [한국어](README.ko.md) · [Tiếng Việt](README.vi.md) · [中文 (简体)](README.zh-Hans.md) · [中文（繁體）](README.zh-Hant.md) · [Deutsch](README.de.md) · [Русский](README.ru.md)


**语言：** 英文（当前） | i18n 变体将添加到 [`/i18n`](./i18n)

<p align="center">
  <img src="https://raw.githubusercontent.com/lachlanchen/lachlanchen/main/logos/banner.png" alt="LazyingArt banner" />
</p>

<div align="center">

# **omi**

认识 Omi：全球领先的开源 AI 可穿戴设备，可捕获对话、生成摘要、提炼行动项并为你执行操作。只需将 Omi 连接到移动设备，即可随时随地自动获得高质量的会议、聊天和语音备忘录转写。

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

## 目录

- [概览](#概览)
- [功能特性](#功能特性)
- [快速开始（2 分钟）](#快速开始2-分钟)
- [项目结构](#项目结构)
- [前置要求](#前置要求)
- [安装](#安装)
- [使用方式](#使用方式)
- [配置](#配置)
- [示例](#示例)
- [开发说明](#开发说明)
- [故障排查](#故障排查)
- [路线图](#路线图)
- [文档](#文档)
- [贡献](#贡献)
- [支持与社区](#支持与社区)
- [许可证](#许可证)

## 概览

本仓库是开源 Omi 生态系统的 monorepo。

| 包含内容 | 详情 |
| --- | --- |
| Hardware/Firmware | Omi 可穿戴设备固件 + 硬件资源 |
| Omi Glass | Omi Glass 固件/硬件/应用 |
| Mobile | Flutter 伴侣应用 |
| Backend | FastAPI 后端服务 |
| Web | Omi 主前端 + Personas |
| Ecosystem | 插件/集成生态 |
| SDKs | Python、React Native、Swift |
| Agent Infra | MCP server |
| Docs | 文档源码 |

根 README 的快速开始有意聚焦终端用户/开发者入门。完整的组件级配置请查看各子项目 README 与 Omi 文档。

## 功能特性

- ⚡ 实时 AI 音频处理与转写流程
- 🔋 低功耗蓝牙可穿戴设备工作流
- 🧩 覆盖固件、应用、后端、Web 与 SDK 的开源软件栈
- 🎙️ 面向可穿戴场景优先的会议、聊天与语音备忘录体验
- 🔗 支持通过 Webhook/应用生态触发自定义动作
- 🛠️ 通过插件/集成架构扩展能力

## 快速开始（2 分钟）

### 1) 下载 omi App

[<img src='https://upload.wikimedia.org/wikipedia/commons/7/78/Google_Play_Store_badge_EN.svg' alt='Get it on Google Play' height="50px" width="180px">](https://play.google.com/store/apps/details?id=com.friend.ios)
[<img src='https://upload.wikimedia.org/wikipedia/commons/3/3c/Download_on_the_App_Store_Badge.svg' alt="Download on the App Store" height="50px" width="180px">](https://apps.apple.com/us/app/friend-ai-wearable/id6502156163)
[<img src='https://github.com/user-attachments/assets/59c47ec7-3da0-47d7-be2f-7467e4189499' alt="Download MacOS app" height="50px" width="180px">](https://apps.apple.com/us/app/omi-ai-smart-meeting-notes/id6502156163)

### 2) 创建 webhook

使用 [webhook.site](https://webhook.site) 创建 webhook，并复制该 URL。

<img src="https://github.com/user-attachments/assets/083a6ec4-4694-4c7a-843a-4a1a0c254453" width="500">

### 3) 在 omi App 中

| Explore => Create an App                                                                                  | Select Capability                                                                                       | Paste Webhook URL                                                                                         | Install App                                                                                             |
| --------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------- |
| <img src="https://github.com/user-attachments/assets/31809b81-7de2-4381-b5fc-5c9714972211" width="200"> | <img src="https://github.com/user-attachments/assets/59cfbe8e-7e3b-437f-81f7-25eb50ccdd7d" width="200"> | <img src="https://github.com/user-attachments/assets/3d864ee8-555f-4ded-b4db-87ff78128323" width = "200"> | <img src="https://github.com/user-attachments/assets/58cf6da6-e245-415e-92e7-dc1f46583cfc" width="200"> |

### 4) 开始说话并验证事件

开始说话后，你将在 [webhook.site](https://webhook.site) 上看到实时转写。

## 项目结构

### 本仓库包含

- [omi device](https://github.com/BasedHardware/omi/tree/main/omi)
- [omi glass](https://github.com/BasedHardware/omi/tree/main/omiGlass)
- [omi app](https://github.com/BasedHardware/omi/tree/main/app)
- [ai personas (web)](https://github.com/BasedHardware/omi/tree/main/web/personas-open-source)
- [SDKs](./sdks)

注意：旧资料中可能会提到仓库根目录下的 `personas-open-source`；在本仓库中，它当前位于 `web/personas-open-source`。

### 高层目录图

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

## 前置要求

请根据你目标组件选择对应依赖。

| Tooling | 用途 |
| --- | --- |
| Git | 源码版本管理 |
| Node.js 18+ and npm | web、personas、部分插件工作流 |
| Python 3.10+ | backend、MCP、Python SDK |
| Flutter SDK | 移动端应用 |
| Xcode/CocoaPods | iOS 开发 |
| Android Studio + Android SDK | Android 开发 |
| `ffmpeg` + `opus` | backend/音频工作流 |
| Docker (optional) | MCP/web 部署 |
| Google Cloud + Firebase | backend/app 工作流 |

## 安装

由于这是 monorepo，请按组件分别安装。

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

### 终端用户 App 流程

1. 从上方商店链接安装 Omi app。
2. 配对并使用你的 Omi 设备。
3. 通过 webhook 快速开始流程创建应用。
4. 在你的 webhook 端点观察实时转写事件。

### 本地后端配合 App

1. 在本地 `8000` 端口启动 backend。
2. 通过 ngrok 静态域名暴露本地 backend。
3. 将 app 的 `BASE_API_URL` 设置为你的 ngrok URL。
4. 使用 Omi app 连接你的本地 backend。

### SDK 工作流

- Python SDK：使用 `omi-scan` 扫描 BLE 设备，解码 Opus 数据包，并通过 Deepgram 转写。
- React Native SDK：连接设备、流式传输音频字节、检查编解码器/电池状态。
- Swift SDK (`omi-lib`)：使用 `OmiManager` APIs 完成扫描/连接/转写。

## 配置

配置按组件分布。请以各子项目模板/README 为准。

- `backend/.env.template` -> backend API 密钥/基础设施配置
- `web/frontend/.env.template` -> web frontend 环境变量
- `app` environment values -> mobile app 运行时配置
- `mcp` env vars -> `OMI_API_KEY` 和可选的 `OMI_API_BASE_URL`
- SDK-specific keys:
  - Python SDK uses `DEEPGRAM_API_KEY`
  - Personas uses Firebase/OpenRouter/RapidAPI/Mixpanel env vars

如果你不确定哪些变量是必需的，请先保留默认值，并在删除/修改前先遵循该组件的 README。

## 示例

### Webhook quick-start (from root flow)

使用 [webhook.site](https://webhook.site)，在 Omi 中安装你的自定义应用，然后验证转写事件是否实时出现。

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

## 开发说明

- CI/CD 与部署自动化配置位于：
  - `.github/workflows/`
  - `codemagic.yaml`
- 根目录 `scripts/pre-commit` 会格式化以下已暂存文件：
  - `app/` 中的 Dart
  - `backend/` 中的 Python
  - `omi/` 与 `omiGlass/` 中的 C/C++
- 仓库根目录 `Package.swift` 从 `sdks/swift` 发布 Swift 包 `omi-lib`。
- `i18n/` 目录已存在，并保留用于多语言 README/内容变体。

## 故障排查

- 本地 backend 模型/网络问题：若遇到已知 SSL 下载问题，请应用 `backend/README.md` 中记录的 `ssl` 变通方案后重试。
- App 无法连接本地 backend：确认 ngrok 域名正在运行，且 `BASE_API_URL` 指向该精确公网 URL。
- BLE 发现问题：确认平台蓝牙权限已授予（按实际场景为 Terminal/Xcode/Android app）。
- 旧文档路径不一致：部分历史文档/参考文本可能显示过时路径（例如 `personas-open-source` 根路径或 `omi/OmiGlass` 大小写）。本仓库请使用上文展示的当前目录布局。

## 路线图

本节反映当前仓库信号，后续可能调整：

- 持续改进 Omi 与 OmiGlass 的固件/硬件工作流
- 扩展 app/plugin 生态与开发者工具链
- 提升 memories/apps/personas 的 web 体验
- 强化 MCP + SDK 与外部代理生态的集成
- 在 `i18n/` 中新增并维护多语言 README 变体

## 文档

- [Introduction](https://docs.omi.me/)
- [omi App setup](https://docs.omi.me/doc/developer/AppSetup)
- [Buying Guide](https://docs.omi.me/doc/assembly/Buying_Guide/)
- [Build the device](https://docs.omi.me/doc/assembly/Build_the_device/)
- [Install firmware](https://docs.omi.me/doc/get_started/Flash_device/)
- [Create your own app in 1 minute](https://docs.omi.me/doc/developer/apps/Introduction)

## 贡献

- 查看我们的[贡献指南](https://docs.omi.me/doc/developer/Contribution/)。
- 贡献还能获得收益！查看[付费赏金 🤑](https://omi.me/bounties)。
- 查看[当前 issues](https://github.com/BasedHardware/Omi/issues)。
- 加入 [Discord](http://discord.omi.me)。
- 构建你自己的[Plugins/Integrations](https://docs.omi.me/doc/developer/apps/Introduction)。

## 支持与社区

- 主站：[omi.me](https://omi.me/)
- 下载：[omi.me/download](https://omi.me/download)
- 文档：[docs.omi.me](https://docs.omi.me/)
- 社区聊天：[discord.omi.me](http://discord.omi.me)
- 动态关注：[x.com/kodjima33](https://x.com/kodjima33)
- 硬件/开发套件：
  - [Buy omi Dev Kit](https://www.omi.me/products/omi-dev-kit-2)
  - [Buy Omi Glass Dev Kit](https://www.omi.me/glass)

## 许可证

Omi 基于 <a href="https://github.com/BasedHardware/omi/blob/main/LICENSE">MIT License</a> 发布。
