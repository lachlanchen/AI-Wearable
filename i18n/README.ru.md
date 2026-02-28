[English](../README.md) · [العربية](README.ar.md) · [Español](README.es.md) · [Français](README.fr.md) · [日本語](README.ja.md) · [한국어](README.ko.md) · [Tiếng Việt](README.vi.md) · [中文 (简体)](README.zh-Hans.md) · [中文（繁體）](README.zh-Hant.md) · [Deutsch](README.de.md) · [Русский](README.ru.md)



<p align="center">
  <img src="https://raw.githubusercontent.com/lachlanchen/lachlanchen/main/logos/banner.png" alt="LazyingArt banner" />
</p>

<div align="center">

# **omi**

Знакомьтесь: Omi — ведущий в мире open-source AI-носимый девайс, который записывает разговоры, делает сводки, формирует action items и может выполнять действия за вас. Просто подключите Omi к мобильному устройству и получайте автоматические качественные транскрипции встреч, бесед и голосовых заметок где угодно.

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

## Содержание

- [Обзор](#обзор)
- [Возможности](#возможности)
- [Быстрый старт (2 мин)](#быстрый-старт-2-мин)
- [Структура проекта](#структура-проекта)
- [Предварительные требования](#предварительные-требования)
- [Установка](#установка)
- [Использование](#использование)
- [Конфигурация](#конфигурация)
- [Примеры](#примеры)
- [Заметки по разработке](#заметки-по-разработке)
- [Устранение неполадок](#устранение-неполадок)
- [План развития](#план-развития)
- [Документация](#документация)
- [Вклад в проект](#вклад-в-проект)
- [Поддержка и сообщество](#поддержка-и-сообщество)
- [Лицензия](#лицензия)

## Обзор

Этот репозиторий — open-source монорепозиторий экосистемы Omi.

| Включает | Подробности |
| --- | --- |
| Hardware/Firmware | Прошивка Omi wearable + аппаратные ресурсы |
| Omi Glass | Прошивка/железо/приложение Omi Glass |
| Mobile | Компаньон-приложение на Flutter |
| Backend | Backend-сервисы на FastAPI |
| Web | Основной фронтенд Omi + Personas |
| Ecosystem | Экосистема плагинов/интеграций |
| SDKs | Python, React Native, Swift |
| Agent Infra | MCP server |
| Docs | Исходники документации |

Корневой quick-start в README намеренно ориентирован на onboarding конечных пользователей и разработчиков. Полная настройка для каждого компонента находится в README соответствующих подпроектов и в документации Omi.

## Возможности

- ⚡ Потоки обработки аудио и транскрибации на базе AI в реальном времени
- 🔋 Low-power workflow для носимого Bluetooth-устройства
- 🧩 Open-source стек: от прошивки до приложений, backend, web и SDK
- 🎙️ Wearable-first UX для встреч, бесед и голосовых заметок
- 🔗 Экосистема webhook/app для запуска пользовательских действий
- 🛠️ Архитектура плагинов/интеграций для расширения возможностей

## Быстрый старт (2 мин)

### 1) Скачайте приложение omi

[<img src='https://upload.wikimedia.org/wikipedia/commons/7/78/Google_Play_Store_badge_EN.svg' alt='Get it on Google Play' height="50px" width="180px">](https://play.google.com/store/apps/details?id=com.friend.ios)
[<img src='https://upload.wikimedia.org/wikipedia/commons/3/3c/Download_on_the_App_Store_Badge.svg' alt="Download on the App Store" height="50px" width="180px">](https://apps.apple.com/us/app/friend-ai-wearable/id6502156163)
[<img src='https://github.com/user-attachments/assets/59c47ec7-3da0-47d7-be2f-7467e4189499' alt="Download MacOS app" height="50px" width="180px">](https://apps.apple.com/us/app/omi-ai-smart-meeting-notes/id6502156163)

### 2) Создайте webhook

Создайте webhook через [webhook.site](https://webhook.site) и скопируйте этот URL.

<img src="https://github.com/user-attachments/assets/083a6ec4-4694-4c7a-843a-4a1a0c254453" width="500">

### 3) В приложении omi

| Explore => Create an App                                                                                  | Select Capability                                                                                       | Paste Webhook URL                                                                                         | Install App                                                                                             |
| --------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------- |
| <img src="https://github.com/user-attachments/assets/31809b81-7de2-4381-b5fc-5c9714972211" width="200"> | <img src="https://github.com/user-attachments/assets/59cfbe8e-7e3b-437f-81f7-25eb50ccdd7d" width="200"> | <img src="https://github.com/user-attachments/assets/3d864ee8-555f-4ded-b4db-87ff78128323" width = "200"> | <img src="https://github.com/user-attachments/assets/58cf6da6-e245-415e-92e7-dc1f46583cfc" width="200"> |

### 4) Говорите и проверяйте события

Начните говорить: вы увидите транскрипцию в реальном времени на [webhook.site](https://webhook.site).

## Структура проекта

### В этом репозитории

- [omi device](https://github.com/BasedHardware/omi/tree/main/omi)
- [omi glass](https://github.com/BasedHardware/omi/tree/main/omiGlass)
- [omi app](https://github.com/BasedHardware/omi/tree/main/app)
- [ai personas (web)](https://github.com/BasedHardware/omi/tree/main/web/personas-open-source)
- [SDKs](./sdks)

Примечание: в старых ссылках `personas-open-source` может упоминаться в корне репозитория; в этом репозитории он сейчас расположен в `web/personas-open-source`.

### Карта верхнего уровня

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

## Предварительные требования

Используйте требования, соответствующие целевому компоненту.

| Инструменты | Используется для |
| --- | --- |
| Git | Контроль версий |
| Node.js 18+ and npm | web, personas, некоторые workflow плагинов |
| Python 3.10+ | backend, MCP, Python SDK |
| Flutter SDK | мобильное приложение |
| Xcode/CocoaPods | разработка под iOS |
| Android Studio + Android SDK | разработка под Android |
| `ffmpeg` + `opus` | workflow backend/аудио |
| Docker (optional) | деплой MCP/web |
| Google Cloud + Firebase | workflow backend/app |

## Установка

Так как это монорепозиторий, установка выполняется по компонентам.

### Клонирование репозитория

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

## Использование

### Поток для конечного пользователя

1. Установите приложение Omi по ссылкам на магазины выше.
2. Подключите и используйте ваше устройство Omi.
3. Создайте приложение через quick-start с webhook.
4. Говорите и наблюдайте события транскрипции в реальном времени на endpoint вашего webhook.

### Локальный backend с приложением

1. Запустите backend локально на порту `8000`.
2. Опубликуйте локальный backend через статический домен ngrok.
3. Установите `BASE_API_URL` в приложении на ваш URL ngrok.
4. Используйте приложение Omi с локальным backend.

### Workflow SDK

- Python SDK: сканируйте BLE-устройства с `omi-scan`, декодируйте Opus-пакеты и транскрибируйте через Deepgram.
- React Native SDK: подключайтесь, стримьте аудиобайты, проверяйте кодек/батарею.
- Swift SDK (`omi-lib`): сканирование/подключение/транскрибация через API `OmiManager`.

## Конфигурация

Конфигурация распределена по компонентам. Используйте шаблон/readme каждого подпроекта как источник истины.

- `backend/.env.template` -> ключи API backend/конфигурация инфраструктуры
- `web/frontend/.env.template` -> переменные окружения web frontend
- значения окружения `app` -> runtime-конфигурация мобильного приложения
- переменные окружения `mcp` -> `OMI_API_KEY` и опционально `OMI_API_BASE_URL`
- ключи для конкретных SDK:
  - Python SDK использует `DEEPGRAM_API_KEY`
  - Personas использует переменные окружения Firebase/OpenRouter/RapidAPI/Mixpanel

Если вы не уверены, какие переменные обязательны, сохраните значения по умолчанию и сначала следуйте README конкретного компонента, прежде чем удалять/менять значения.

## Примеры

### Webhook quick-start (из корневого потока)

Используйте [webhook.site](https://webhook.site), установите свое кастомное приложение в Omi, затем проверьте, что события транскрипции появляются в реальном времени.

### Команда запуска backend

```bash
cd backend
uvicorn main:app --reload --env-file .env
```

### Команда запуска frontend

```bash
cd web/frontend
npm run dev
```

### Сканирование в Python SDK

```bash
cd sdks/python
omi-scan
```

## Заметки по разработке

- Автоматизация CI/CD и деплоя настроена в:
  - `.github/workflows/`
  - `codemagic.yaml`
- Корневой `scripts/pre-commit` форматирует staged-файлы для:
  - Dart в `app/`
  - Python в `backend/`
  - C/C++ в `omi/` и `omiGlass/`
- `Package.swift` в корне репозитория публикует Swift-пакет `omi-lib` из `sdks/swift`.
- Директория `i18n/` существует и зарезервирована для многоязычных вариантов README/контента.

## Устранение неполадок

- Проблема с моделью/сетью backend при локальной настройке: если возникла известная проблема загрузки SSL, примените обходной путь `ssl`, описанный в `backend/README.md`, и повторите попытку.
- Приложение не может достучаться до локального backend: проверьте, что домен ngrok запущен и `BASE_API_URL` указывает на этот точный публичный URL.
- Проблемы обнаружения BLE: убедитесь, что выданы разрешения Bluetooth для соответствующей платформы (Terminal/Xcode/Android app).
- Несоответствие путей в старой документации: в некоторых legacy-документах/справках могут быть устаревшие пути (например, корневой путь `personas-open-source` или регистр `omi/OmiGlass`). В этом репозитории используйте актуальную структуру директорий, показанную выше.

## План развития

Этот раздел отражает текущие сигналы репозитория и может меняться:

- Продолжать улучшать workflow прошивки/железа для Omi и OmiGlass
- Расширять экосистему приложений/плагинов и инструменты для разработчиков
- Улучшать web-опыт для memories/apps/personas
- Усиливать интеграции MCP + SDK для внешних агентных экосистем
- Добавлять и поддерживать многоязычные варианты README в `i18n/`

## Документация

- [Introduction](https://docs.omi.me/)
- [omi App setup](https://docs.omi.me/doc/developer/AppSetup)
- [Buying Guide](https://docs.omi.me/doc/assembly/Buying_Guide/)
- [Build the device](https://docs.omi.me/doc/assembly/Build_the_device/)
- [Install firmware](https://docs.omi.me/doc/get_started/Flash_device/)
- [Create your own app in 1 minute](https://docs.omi.me/doc/developer/apps/Introduction)

## Вклад в проект

- Ознакомьтесь с нашим [руководством по вкладу](https://docs.omi.me/doc/developer/Contribution/).
- Зарабатывайте на участии! Посмотрите [оплачиваемые баунти 🤑](https://omi.me/bounties).
- Посмотрите [текущие issues](https://github.com/BasedHardware/Omi/issues).
- Присоединяйтесь к [Discord](http://discord.omi.me).
- Создавайте собственные [Plugins/Integrations](https://docs.omi.me/doc/developer/apps/Introduction).

## Поддержка и сообщество

- Основной сайт: [omi.me](https://omi.me/)
- Загрузки: [omi.me/download](https://omi.me/download)
- Документация: [docs.omi.me](https://docs.omi.me/)
- Чат сообщества: [discord.omi.me](http://discord.omi.me)
- Следите за обновлениями: [x.com/kodjima33](https://x.com/kodjima33)
- Hardware/dev kits:
  - [Buy omi Dev Kit](https://www.omi.me/products/omi-dev-kit-2)
  - [Buy Omi Glass Dev Kit](https://www.omi.me/glass)

## Лицензия

Omi доступен по лицензии <a href="https://github.com/BasedHardware/omi/blob/main/LICENSE">MIT License</a>
