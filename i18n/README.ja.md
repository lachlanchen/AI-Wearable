[English](../README.md) · [العربية](README.ar.md) · [Español](README.es.md) · [Français](README.fr.md) · [日本語](README.ja.md) · [한국어](README.ko.md) · [Tiếng Việt](README.vi.md) · [中文 (简体)](README.zh-Hans.md) · [中文（繁體）](README.zh-Hant.md) · [Deutsch](README.de.md) · [Русский](README.ru.md)


[![LazyingArt banner](https://github.com/lachlanchen/lachlanchen/raw/main/figs/banner.png)](https://github.com/lachlanchen/lachlanchen/blob/main/figs/banner.png)

<div align="center">

# **omi**

_AI-powered wearable for instant meetings and chats: capture, summarize, and act—hands-free._

会議やチャットをその場でサポートする AI ウェアラブルです。会話を取り込み、要約し、必要な操作まで自動で実行します。

世界最高水準のオープンソース AI ウェアラブルとして Omi は会話の記録、要約、実行可能なアクション生成までを行います。Omi をモバイルデバイスに接続するだけで、どこにいても高品質な会議・チャット・音声メモの文字起こしを自動取得できます。

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

## ⚡ クイックリンク

| リソース | リンク |
| --- | --- |
| 🌐 プロジェクトサイト | [omi.me](https://omi.me/) |
| ⬇️ ダウンロードセンター | [omi.me/download](https://omi.me/download) |
| 📚 ドキュメント | [docs.omi.me](https://docs.omi.me/) |
| 🛠️ Omi Dev Kit | [Omi Dev Kit を購入](https://www.omi.me/products/omi-dev-kit-2) |
| 👓 Omi Glass Dev Kit | [Omi Glass を購入](https://www.omi.me/glass) |

---

## 目次

- [📌 概要](#%E6%A6%82%E8%A6%81)
- [⚡️ 特徴](#%E7%89%B9%E5%BE%B4)
- [🚀 クイックスタート (2 分)](#%E3%82%AF%E3%82%A4%E3%83%83%E3%82%AF%E3%82%B9%E3%82%BF%E3%83%BC%E3%83%88-2-%E5%88%86)
- [🏗️ プロジェクト構造](#%E3%83%97%E3%83%AD%E3%82%B8%E3%82%A7%E3%82%AF%E3%83%88%E6%A7%8B%E9%80%A0)
- [🧰 前提条件](#%E5%89%8D%E6%8F%90%E6%9D%A1%E4%BB%B6)
- [🛠️ インストール](#%E3%82%A4%E3%83%B3%E3%82%B9%E3%83%88%E3%83%BC%E3%83%AB)
- [🧪 利用方法](#%E5%88%A9%E7%94%A8%E6%96%B9%E6%B3%95)
- [⚙️ 設定](#%E8%A8%AD%E5%AE%9A)
- [🧾 例](#%E4%BE%8B)
- [🧭 開発ノート](#%E9%96%8B%E7%99%BA%E3%83%8E%E3%83%BC%E3%83%88)
- [🐞 トラブルシューティング](#%E3%83%88%E3%83%A9%E3%83%96%E3%83%AB%E3%82%B7%E3%83%A5%E3%83%BC%E3%83%86%E3%82%A3%E3%83%B3%E3%82%B0)
- [🗺️ ロードマップ](#%E3%83%AD%E3%83%BC%E3%83%89%E3%83%9E%E3%83%83%E3%83%97)
- [📚 ドキュメント](#%E3%83%89%E3%82%AD%E3%83%A5%E3%83%A1%E3%83%B3%E3%83%88)
- [🤝 貢献](#%E8%B2%A2%E7%8C%AE)
- [❤️ Support](#%E2%9D%A4%EF%B8%8F-support)
- [💬 お問い合わせとコミュニティ](#%E3%81%8A%E5%95%8F%E5%90%88%E3%81%9B%E3%81%A8%E3%82%B3%E3%83%9F%E3%83%A5%E3%83%8B%E3%83%86%E3%82%A3)
- [📜 ライセンス](#%E3%83%A9%E3%82%A4%E3%82%BB%E3%83%B3%E3%82%B9)

## 概要

このリポジトリは Omi エコシステムのオープンソースモノレポです。

| 含まれる内容 | 詳細 |
| --- | --- |
| 🧠 Omi Hardware | Omi ウェアラブルのファームウェア + ハードウェア資産 |
| 🥽 Omi Glass | Omi Glass のファームウェア/ハードウェア/アプリ |
| 📱 Mobile | Flutter 連携アプリ |
| 🌐 Backend | FastAPI バックエンドサービス |
| 🕸️ Web | Omi メインフロントエンド + Personas |
| 🧩 エコシステム | プラグイン・インテグレーションエコシステム |
| 📦 SDKs | Python, React Native, Swift |
| 🔗 Agent Infra | MCP サーバー |
| 📘 Docs | ドキュメントのソース |

ルートの README は、オンボーディングと日常的な開発ワークフローに焦点を当てています。各コンポーネント固有のセットアップや運用メモは、各サブプロジェクトの README と `docs/` に記載されています。

## 特徴

- ⚡ リアルタイムの AI 音声処理と文字起こしフロー
- 🔋 低電力 Bluetooth ウェアラブルデバイスのワークフロー
- 🧩 ファームウェア、アプリ、バックエンド、Web、SDK を横断するオープンソース技術スタック
- 🎙️ 会議・チャット・音声メモ向けのウェアラブルファースト UX
- 🔗 カスタムアクションを起動できる Webhook / アプリエコシステム
- 🛠️ 機能拡張のためのプラグインおよび統合アーキテクチャ

## クイックスタート (2 分)

### 1) omi アプリをダウンロード

[<img src='https://upload.wikimedia.org/wikipedia/commons/7/78/Google_Play_Store_badge_EN.svg' alt='Get it on Google Play' height="50px" width="180px">](https://play.google.com/store/apps/details?id=com.friend.ios)
[<img src='https://upload.wikimedia.org/wikipedia/commons/3/3c/Download_on_the_App_Store_Badge.svg' alt="Download on the App Store" height="50px" width="180px">](https://apps.apple.com/us/app/friend-ai-wearable/id6502156163)
[<img src='https://github.com/user-attachments/assets/59c47ec7-3da0-47d7-be2f-7467e4189499' alt="Download MacOS app" height="50px" width="180px">](https://apps.apple.com/us/app/omi-ai-smart-meeting-notes/id6502156163)

### 2) Webhook を作成

[webhook.site](https://webhook.site) で webhook を作成し、この URL をコピーします。

<img src="https://github.com/user-attachments/assets/083a6ec4-4694-4c7a-843a-4a1a0c254453" width="500">

### 3) Omi アプリ内での設定

| Explore => Create an App                                                                                  | Select Capability                                                                                       | Paste Webhook URL                                                                                         | Install App                                                                                             |
| --------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------- |
| <img src="https://github.com/user-attachments/assets/31809b81-7de2-4381-b5fc-5c9714972211" width="200"> | <img src="https://github.com/user-attachments/assets/59cfbe8e-7e3b-437f-81f7-25eb50ccdd7d" width="200"> | <img src="https://github.com/user-attachments/assets/3d864ee8-555f-4ded-b4db-87ff78128323" width="200"> | <img src="https://github.com/user-attachments/assets/58cf6da6-e245-415e-92e7-dc1f46583cfc" width="200"> |

### 4) 話してイベントを確認

話しかけると、[webhook.site](https://webhook.site) 上でリアルタイム文字起こしイベントが表示されます。

## プロジェクト構造

### このリポジトリ内

| コンポーネント | 目的 |
| --- | --- |
| [omi device](https://github.com/BasedHardware/omi/tree/main/omi) | Omi ハードウェア + ファームウェア |
| [omi glass](https://github.com/BasedHardware/omi/tree/main/omiGlass) | Omi Glass ハードウェア + ファームウェア |
| [omi app](https://github.com/BasedHardware/omi/tree/main/app) | Flutter 連携アプリ |
| [ai personas (web)](https://github.com/BasedHardware/omi/tree/main/web/personas-open-source) | Personas Web アプリ |
| [SDKs](./sdks) | Python、React Native、Swift SDK |

注: 以前の資料には `personas-open-source` がリポジトリのルートにあると記載されている場合がありますが、このリポジトリでは現在 `web/personas-open-source` 配下にあります。

### 全体構成図

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

## 前提条件

対象コンポーネントに応じて必要な要件を用意してください。

| ツール | 用途 |
| --- | --- |
| Git | ソース管理 |
| Node.js 18+ と npm | Web、personas、一部のプラグインワークフロー |
| Python 3.10+ | Backend、MCP、Python SDK |
| Flutter SDK | モバイルアプリ |
| Xcode/CocoaPods | iOS 開発 |
| Android Studio + Android SDK | Android 開発 |
| `ffmpeg` + `opus` | Backend/音声フロー |
| Docker（任意） | MCP/web のデプロイ |
| Google Cloud + Firebase | Backend/app のワークフロー |

### 構成時の前提

- 一部のコマンドは外部クレデンシャル（Firebase、OpenAI/Deepgram/API プロバイダなど）に依存します。通常は対象コンポーネントの `.env` テンプレートで設定します。値が不明な場合は、各コンポーネントの README を確認してください。
- 1 つの画面だけが必要な場合は、そのコンポーネントのみインストール・ビルドして開発を速めます。

## インストール

本リポジトリはモノレポ構成のため、コンポーネントごとにインストールします。

### リポジトリをクローン

```bash
git clone https://github.com/BasedHardware/omi.git
cd omi
```

### アプリ（Flutter）

```bash
cd app
bash setup.sh ios
# または
bash setup.sh android

flutter run --flavor dev
```

### バックエンド（FastAPI）

```bash
cd backend
cp .env.template .env
pip install -r requirements.txt
uvicorn main:app --reload --env-file .env
```

### メインフロントエンド（Next.js）

```bash
cd web/frontend
npm install
cp .env.template .env.local
npm run dev
```

### Personas Web アプリ（Next.js）

```bash
cd web/personas-open-source
npm install
npm run dev
```

### MCP サーバー

```bash
cd mcp
# Docker ベースの Claude Desktop 設定については mcp/README.md を参照してください
```

### SDKs

```bash
cd sdks/python && pip install -e .
cd ../react-native && npm install
# Swift パッケージはルートの Package.swift で `omi-lib` として公開されています
```

## 利用方法

### エンドユーザー向けアプリの流れ

1. 上記のリンクから Omi アプリをインストールします。
2. Omi デバイスをペアリングして使用します。
3. Webhook クイックスタートでアプリを作成します。
4. 話しかけて、webhook エンドポイントでリアルタイム文字起こしイベントを確認します。

### ローカル backend とアプリの利用

1. ローカル backend をポート `8000` で起動します。
2. ngrok の固定ドメインでローカル backend を公開します。
3. アプリの `BASE_API_URL` を ngrok の URL に設定します。
4. Omi アプリをローカル backend に向けます。

### SDK のワークフロー

- Python SDK: `omi-scan` で BLE デバイスをスキャンし、Opus パケットをデコードして Deepgram で文字起こしします。
- React Native SDK: 接続、オーディオバイトのストリーミング、codec とバッテリー状態の確認
- Swift SDK（`omi-lib`）: `OmiManager` API を使ったスキャン、接続、文字起こし

## 設定

設定はコンポーネントごとに分かれています。各サブプロジェクトのテンプレート/README を真の情報源として参照してください。

- `backend/.env.template` -> backend API キー・インフラ設定
- `web/frontend/.env.template` -> Web フロントエンドの環境変数
- `app` の環境値 -> モバイルアプリの実行時設定
- `mcp` の環境変数 -> `OMI_API_KEY` と任意の `OMI_API_BASE_URL`
- SDK 固有のキー:
  - Python SDK は `DEEPGRAM_API_KEY`
  - Personas は Firebase/OpenRouter/RapidAPI/Mixpanel の環境変数

必要な変数が不明な場合は、既定値を保持し、値の削除や変更は対象コンポーネントの README を確認してから行ってください。

## 例

### Webhook クイックスタート（ルートフロー）

[webhook.site](https://webhook.site) を使い、Omi にカスタムアプリをインストールして文字起こしイベントがリアルタイムで反映されることを確認します。

### バックエンド起動コマンド

```bash
cd backend
uvicorn main:app --reload --env-file .env
```

### フロントエンド起動コマンド

```bash
cd web/frontend
npm run dev
```

### Python SDK スキャン

```bash
cd sdks/python
omi-scan
```

## 開発ノート

- CI/CD とデプロイ自動化は次に設定されています。
  - `.github/workflows/`
  - `codemagic.yaml`
- ルートの `scripts/pre-commit` はステージング中のファイルを整形します。
  - `app/` の Dart
  - `backend/` の Python
  - `omi/` と `omiGlass/` の C/C++
- リポジトリルートの `Package.swift` は、`sdks/swift` から Swift パッケージ `omi-lib` を公開します。
- `i18n/` ディレクトリは、多言語 README/コンテンツのために用意されています。

## トラブルシューティング

- ローカルセットアップで backend のモデル/ネットワーク問題が出た場合、既知の SSL ダウンロード問題に対する `ssl` 回避策を `backend/README.md` で確認して再実行してください。
- アプリがローカル backend に接続できない場合: ngrok ドメインが起動中で、`BASE_API_URL` がその公開 URL を正確に指しているか確認してください。
- BLE の検出問題: プラットフォームに応じて Bluetooth 権限（Terminal/Xcode/Android アプリ）が付与されているか確認します。
- 旧ドキュメントのパス不一致: 過去の資料では古いパスが残ることがあります（例: ルートの `personas-open-source` や `omi/OmiGlass` の大文字小文字）。このリポジトリでは上記の現在の構成を使用します。

## ロードマップ

このセクションは現時点でのリポジトリ情報を反映しており、更新される可能性があります。

- Omi と OmiGlass の firmware/hardware ワークフローを継続的に改善
- アプリ/プラグインエコシステムおよび開発者向けツールを拡張
- memories/apps/personas 向け Web 体験の改善
- 外部エージェントエコシステム向けに MCP + SDK 連携を強化
- `i18n/` の多言語 README バリアントを追加・維持

## ドキュメント

- [イントロダクション](https://docs.omi.me/)
- [Omi アプリのセットアップ](https://docs.omi.me/doc/developer/AppSetup)
- [購入ガイド](https://docs.omi.me/doc/assembly/Buying_Guide/)
- [デバイスの組み立て](https://docs.omi.me/doc/assembly/Build_the_device/)
- [ファームウェアのインストール](https://docs.omi.me/doc/get_started/Flash_device/)
- [1 分でアプリを作成](https://docs.omi.me/doc/developer/apps/Introduction)

## 貢献

- [contribution ガイド](https://docs.omi.me/doc/developer/Contribution/) を確認してください。
- 貢献して報酬を得られる可能性のある [有給バウンティ 🤑](https://omi.me/bounties) を参照。
- [現在の課題](https://github.com/BasedHardware/Omi/issues) を確認してください。
- [Discord](http://discord.omi.me) に参加。
- 独自の [Plugins/Integrations](https://docs.omi.me/doc/developer/apps/Introduction) を作成してください。

## お問い合わせとコミュニティ

- メインサイト: [omi.me](https://omi.me/)
- ダウンロード: [omi.me/download](https://omi.me/download)
- ドキュメント: [docs.omi.me](https://docs.omi.me/)
- コミュニティチャット: [discord.omi.me](http://discord.omi.me)
- 更新情報: [x.com/kodjima33](https://x.com/kodjima33)
- ハードウェア / 開発キット:
  - [Omi Dev Kit を購入](https://www.omi.me/products/omi-dev-kit-2)
  - [Omi Glass Dev Kit を購入](https://www.omi.me/glass)

## ライセンス

Omi は <a href="https://github.com/BasedHardware/omi/blob/main/LICENSE">MIT License</a> の下で公開されています。


## ❤️ Support

| Donate | PayPal | Stripe |
| --- | --- | --- |
| [![Donate](https://camo.githubusercontent.com/24a4914f0b42c6f435f9e101621f1e52535b02c225764b2f6cc99416926004b7/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f446f6e6174652d4c617a79696e674172742d3045413545393f7374796c653d666f722d7468652d6261646765266c6f676f3d6b6f2d6669266c6f676f436f6c6f723d7768697465)](https://chat.lazying.art/donate) | [![PayPal](https://camo.githubusercontent.com/d0f57e8b016517a4b06961b24d0ca87d62fdba16e18bbdb6aba28e978dc0ea21/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f50617950616c2d526f6e677a686f754368656e2d3030343537433f7374796c653d666f722d7468652d6261646765266c6f676f3d70617970616c266c6f676f436f6c6f723d7768697465)](https://paypal.me/RongzhouChen) | [![Stripe](https://camo.githubusercontent.com/1152dfe04b6943afe3a8d2953676749603fb9f95e24088c92c97a01a897b4942/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f5374726970652d446f6e6174652d3633354246463f7374796c653d666f722d7468652d6261646765266c6f676f3d737472697065266c6f676f436f6c6f723d7768697465)](https://buy.stripe.com/aFadR8gIaflgfQV6T4fw400) |
