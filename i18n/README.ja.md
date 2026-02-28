[English](../README.md) · [العربية](README.ar.md) · [Español](README.es.md) · [Français](README.fr.md) · [日本語](README.ja.md) · [한국어](README.ko.md) · [Tiếng Việt](README.vi.md) · [中文 (简体)](README.zh-Hans.md) · [中文（繁體）](README.zh-Hant.md) · [Deutsch](README.de.md) · [Русский](README.ru.md)


<p align="center">
  <img src="https://raw.githubusercontent.com/lachlanchen/lachlanchen/main/logos/banner.png" alt="LazyingArt banner" />
</p>

<div align="center">

# **omi**

Omi は、会話を記録し、要約やアクション項目を生成し、実際のアクション実行まで支援する、世界をリードするオープンソース AI ウェアラブルです。モバイルデバイスに接続するだけで、会議・チャット・ボイスメモを場所を問わず自動で高品質に文字起こしできます。

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

このリポジトリは、Omi エコシステム全体を収めたオープンソースのモノレポです。

| 含まれるもの | 詳細 |
| --- | --- |
| Hardware/Firmware | Omi ウェアラブルのファームウェア + ハードウェア資産 |
| Omi Glass | Omi Glass のファームウェア/ハードウェア/アプリ |
| Mobile | Flutter コンパニオンアプリ |
| Backend | FastAPI バックエンドサービス |
| Web | Omi メインフロントエンド + Personas |
| Ecosystem | プラグイン/連携エコシステム |
| SDKs | Python, React Native, Swift |
| Agent Infra | MCP サーバー |
| Docs | ドキュメントソース |

ルート README のクイックスタートは、エンドユーザーと開発者のオンボーディングに意図的にフォーカスしています。各コンポーネント固有の詳細セットアップは、各サブプロジェクトの README と Omi ドキュメントを参照してください。

## Features

- ⚡ リアルタイム AI 音声処理と文字起こしフロー
- 🔋 低消費電力 Bluetooth ウェアラブル向けワークフロー
- 🧩 ファームウェア、アプリ、バックエンド、Web、SDK にまたがるオープンソーススタック
- 🎙️ 会議・チャット・ボイスメモを中心に設計されたウェアラブルファースト UX
- 🔗 カスタムアクションをトリガーできる Webhook/アプリ連携エコシステム
- 🛠️ 機能拡張のためのプラグイン/インテグレーションアーキテクチャ

## Quick Start (2 min)

### 1) omi App をダウンロード

[<img src='https://upload.wikimedia.org/wikipedia/commons/7/78/Google_Play_Store_badge_EN.svg' alt='Get it on Google Play' height="50px" width="180px">](https://play.google.com/store/apps/details?id=com.friend.ios)
[<img src='https://upload.wikimedia.org/wikipedia/commons/3/3c/Download_on_the_App_Store_Badge.svg' alt="Download on the App Store" height="50px" width="180px">](https://apps.apple.com/us/app/friend-ai-wearable/id6502156163)
[<img src='https://github.com/user-attachments/assets/59c47ec7-3da0-47d7-be2f-7467e4189499' alt="Download MacOS app" height="50px" width="180px">](https://apps.apple.com/us/app/omi-ai-smart-meeting-notes/id6502156163)

### 2) webhook を作成

[webhook.site](https://webhook.site) で webhook を作成し、この URL をコピーします。

<img src="https://github.com/user-attachments/assets/083a6ec4-4694-4c7a-843a-4a1a0c254453" width="500">

### 3) omi App で設定

| Explore => Create an App                                                                                  | Select Capability                                                                                       | Paste Webhook URL                                                                                         | Install App                                                                                             |
| --------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------- |
| <img src="https://github.com/user-attachments/assets/31809b81-7de2-4381-b5fc-5c9714972211" width="200"> | <img src="https://github.com/user-attachments/assets/59cfbe8e-7e3b-437f-81f7-25eb50ccdd7d" width="200"> | <img src="https://github.com/user-attachments/assets/3d864ee8-555f-4ded-b4db-87ff78128323" width = "200"> | <img src="https://github.com/user-attachments/assets/58cf6da6-e245-415e-92e7-dc1f46583cfc" width="200"> |

### 4) 話してイベントを確認

話し始めると、[webhook.site](https://webhook.site) でリアルタイム文字起こしを確認できます。

## Project Structure

### このリポジトリに含まれるもの

- [omi device](https://github.com/BasedHardware/omi/tree/main/omi)
- [omi glass](https://github.com/BasedHardware/omi/tree/main/omiGlass)
- [omi app](https://github.com/BasedHardware/omi/tree/main/app)
- [ai personas (web)](https://github.com/BasedHardware/omi/tree/main/web/personas-open-source)
- [SDKs](./sdks)

注記: 古い参照では `personas-open-source` がリポジトリ直下にある前提で書かれている場合がありますが、このリポジトリでは現在 `web/personas-open-source` 配下にあります。

### 全体マップ

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

対象コンポーネントに応じた要件を使用してください。

| Tooling | Used for |
| --- | --- |
| Git | ソース管理 |
| Node.js 18+ and npm | web、personas、一部プラグインワークフロー |
| Python 3.10+ | backend、MCP、Python SDK |
| Flutter SDK | モバイルアプリ |
| Xcode/CocoaPods | iOS 開発 |
| Android Studio + Android SDK | Android 開発 |
| `ffmpeg` + `opus` | backend/音声ワークフロー |
| Docker (optional) | MCP/web デプロイ |
| Google Cloud + Firebase | backend/app ワークフロー |

## Installation

このリポジトリはモノレポのため、コンポーネントごとにインストールします。

### リポジトリをクローン

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

### エンドユーザー向けアプリフロー

1. 上記ストアリンクから Omi アプリをインストールします。
2. Omi デバイスをペアリングして使用します。
3. webhook クイックスタートに沿ってアプリを作成します。
4. webhook エンドポイントでリアルタイム文字起こしイベントを確認します。

### アプリとローカル backend を接続

1. backend をローカルの `8000` ポートで起動します。
2. ngrok の static domain でローカル backend を公開します。
3. アプリの `BASE_API_URL` を ngrok URL に設定します。
4. ローカル backend に対して Omi アプリを使用します。

### SDK ワークフロー

- Python SDK: `omi-scan` で BLE デバイスを検出し、Opus パケットをデコードして Deepgram で文字起こしします。
- React Native SDK: 接続して音声バイト列をストリーミングし、コーデック/バッテリー状態を確認します。
- Swift SDK (`omi-lib`): `OmiManager` API でスキャン/接続/文字起こしを実行します。

## Configuration

設定はコンポーネントごとに分散しています。各サブプロジェクトのテンプレート/README を正として参照してください。

- `backend/.env.template` -> backend の API キー/インフラ設定
- `web/frontend/.env.template` -> web frontend の環境変数
- `app` environment values -> モバイルアプリのランタイム設定
- `mcp` env vars -> `OMI_API_KEY` と任意の `OMI_API_BASE_URL`
- SDK 固有のキー:
  - Python SDK は `DEEPGRAM_API_KEY` を使用
  - Personas は Firebase/OpenRouter/RapidAPI/Mixpanel の環境変数を使用

必要な変数が不明な場合はデフォルト値を維持し、値を削除・変更する前に該当コンポーネントの README を確認してください。

## Examples

### Webhook quick-start (ルートフロー)

[webhook.site](https://webhook.site) を使って Omi にカスタムアプリをインストールし、文字起こしイベントがリアルタイムで表示されることを確認します。

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

- CI/CD とデプロイ自動化の設定:
  - `.github/workflows/`
  - `codemagic.yaml`
- ルートの `scripts/pre-commit` は、ステージ済みファイルに対して次を整形します:
  - `app/` の Dart
  - `backend/` の Python
  - `omi/` と `omiGlass/` の C/C++
- リポジトリルートの `Package.swift` は、`sdks/swift` から Swift パッケージ `omi-lib` を公開します。
- `i18n/` ディレクトリは存在しており、多言語 README/コンテンツの配置先として予約されています。

## Troubleshooting

- ローカル環境で backend のモデル/ネットワーク問題が出る場合: 既知の SSL ダウンロード問題に遭遇したら、`backend/README.md` に記載の `ssl` 回避策を適用して再試行してください。
- アプリがローカル backend に到達できない場合: ngrok ドメインが稼働しているか、`BASE_API_URL` がその公開 URL と完全一致しているかを確認してください。
- BLE 検出の問題: プラットフォームごとの Bluetooth 権限（Terminal/Xcode/Android アプリ）を確認してください。
- 古いドキュメントとのパス不一致: 一部の旧ドキュメントや参照テキストでは古いパス（例: `personas-open-source` のルート配置、`omi/OmiGlass` の大文字小文字）を示すことがあります。このリポジトリでは上記の現在のディレクトリ構成を使用してください。

## Roadmap

このセクションは現在のリポジトリ状況を反映しており、今後更新される可能性があります。

- Omi および OmiGlass の firmware/hardware ワークフロー改善を継続
- アプリ/プラグインのエコシステムと開発者向けツールを拡充
- memories/apps/personas 向け Web 体験を改善
- 外部エージェントエコシステム向けに MCP + SDK 連携を強化
- `i18n/` に多言語 README バリアントを追加・維持

## Documentation

- [Introduction](https://docs.omi.me/)
- [omi App setup](https://docs.omi.me/doc/developer/AppSetup)
- [Buying Guide](https://docs.omi.me/doc/assembly/Buying_Guide/)
- [Build the device](https://docs.omi.me/doc/assembly/Build_the_device/)
- [Install firmware](https://docs.omi.me/doc/get_started/Flash_device/)
- [Create your own app in 1 minute](https://docs.omi.me/doc/developer/apps/Introduction)

## Contributions

- [contributions guide](https://docs.omi.me/doc/developer/Contribution/) を確認してください。
- 貢献で収益化できます。[paid bounties 🤑](https://omi.me/bounties) を確認してください。
- [current issues](https://github.com/BasedHardware/Omi/issues) を確認してください。
- [Discord](http://discord.omi.me) に参加してください。
- 独自の [Plugins/Integrations](https://docs.omi.me/doc/developer/apps/Introduction) を開発してください。

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

Omi is available under <a href="https://github.com/BasedHardware/omi/blob/main/LICENSE">MIT License</a>
