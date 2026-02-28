[English](../README.md) · [العربية](README.ar.md) · [Español](README.es.md) · [Français](README.fr.md) · [日本語](README.ja.md) · [한국어](README.ko.md) · [Tiếng Việt](README.vi.md) · [中文 (简体)](README.zh-Hans.md) · [中文（繁體）](README.zh-Hant.md) · [Deutsch](README.de.md) · [Русский](README.ru.md)



<p align="center">
  <img src="https://raw.githubusercontent.com/lachlanchen/lachlanchen/main/logos/banner.png" alt="LazyingArt banner" />
</p>

<div align="center">

# **omi**

Conoce Omi, el wearable de IA de código abierto líder en el mundo, que captura conversaciones, genera resúmenes, tareas accionables y realiza acciones por ti. Solo conecta Omi a tu dispositivo móvil y disfruta transcripciones automáticas y de alta calidad de reuniones, chats y notas de voz dondequiera que estés.

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

## Tabla de Contenidos

- [Resumen](#resumen)
- [Características](#características)
- [Inicio Rápido (2 min)](#inicio-rápido-2-min)
- [Estructura del Proyecto](#estructura-del-proyecto)
- [Requisitos Previos](#requisitos-previos)
- [Instalación](#instalación)
- [Uso](#uso)
- [Configuración](#configuración)
- [Ejemplos](#ejemplos)
- [Notas de Desarrollo](#notas-de-desarrollo)
- [Solución de Problemas](#solución-de-problemas)
- [Hoja de Ruta](#hoja-de-ruta)
- [Documentación](#documentación)
- [Contribuciones](#contribuciones)
- [Soporte y Comunidad](#soporte-y-comunidad)
- [Licencia](#licencia)

## Resumen

Este repositorio es el monorepo del ecosistema Omi de código abierto.

| Incluye | Detalles |
| --- | --- |
| Hardware/Firmware | Firmware del wearable Omi + recursos de hardware |
| Omi Glass | Firmware/hardware/app de Omi Glass |
| Mobile | App complementaria en Flutter |
| Backend | Servicios backend en FastAPI |
| Web | Frontend principal de Omi + Personas |
| Ecosystem | Ecosistema de plugins/integraciones |
| SDKs | Python, React Native, Swift |
| Agent Infra | Servidor MCP |
| Docs | Fuente de la documentación |

El inicio rápido del README raíz está intencionalmente orientado al onboarding de usuarios finales y desarrolladores. La configuración completa específica de cada componente está en el README de cada subproyecto y en la documentación de Omi.

## Características

- ⚡ Flujos de procesamiento y transcripción de audio con IA en tiempo real
- 🔋 Flujos de trabajo para wearables Bluetooth de bajo consumo
- 🧩 Stack de software de código abierto en firmware, apps, backend, web y SDKs
- 🎙️ UX centrada en wearable para reuniones, chats y notas de voz
- 🔗 Ecosistema de webhook/apps para activar acciones personalizadas
- 🛠️ Arquitectura de plugins/integraciones para ampliar capacidades

## Inicio Rápido (2 min)

### 1) Descargar la app de omi

[<img src='https://upload.wikimedia.org/wikipedia/commons/7/78/Google_Play_Store_badge_EN.svg' alt='Get it on Google Play' height="50px" width="180px">](https://play.google.com/store/apps/details?id=com.friend.ios)
[<img src='https://upload.wikimedia.org/wikipedia/commons/3/3c/Download_on_the_App_Store_Badge.svg' alt="Download on the App Store" height="50px" width="180px">](https://apps.apple.com/us/app/friend-ai-wearable/id6502156163)
[<img src='https://github.com/user-attachments/assets/59c47ec7-3da0-47d7-be2f-7467e4189499' alt="Download MacOS app" height="50px" width="180px">](https://apps.apple.com/us/app/omi-ai-smart-meeting-notes/id6502156163)

### 2) Crear un webhook

Crea un webhook con [webhook.site](https://webhook.site) y copia esa URL.

<img src="https://github.com/user-attachments/assets/083a6ec4-4694-4c7a-843a-4a1a0c254453" width="500">

### 3) En la app de omi

| Explore => Create an App                                                                                  | Select Capability                                                                                       | Paste Webhook URL                                                                                         | Install App                                                                                             |
| --------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------- |
| <img src="https://github.com/user-attachments/assets/31809b81-7de2-4381-b5fc-5c9714972211" width="200"> | <img src="https://github.com/user-attachments/assets/59cfbe8e-7e3b-437f-81f7-25eb50ccdd7d" width="200"> | <img src="https://github.com/user-attachments/assets/3d864ee8-555f-4ded-b4db-87ff78128323" width = "200"> | <img src="https://github.com/user-attachments/assets/58cf6da6-e245-415e-92e7-dc1f46583cfc" width="200"> |

### 4) Habla y verifica eventos

Empieza a hablar y verás la transcripción en tiempo real en [webhook.site](https://webhook.site).

## Estructura del Proyecto

### En este repositorio

- [omi device](https://github.com/BasedHardware/omi/tree/main/omi)
- [omi glass](https://github.com/BasedHardware/omi/tree/main/omiGlass)
- [omi app](https://github.com/BasedHardware/omi/tree/main/app)
- [ai personas (web)](https://github.com/BasedHardware/omi/tree/main/web/personas-open-source)
- [SDKs](./sdks)

Nota: las referencias antiguas pueden mencionar `personas-open-source` en la raíz del repositorio; en este repositorio actualmente está en `web/personas-open-source`.

### Mapa de alto nivel

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

## Requisitos Previos

Usa los requisitos correspondientes al componente objetivo.

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

## Instalación

Como este es un monorepo, la instalación se realiza por componente.

### Clonar repositorio

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

### Frontend principal (Next.js)

```bash
cd web/frontend
npm install
cp .env.template .env.local
npm run dev
```

### App web de Personas (Next.js)

```bash
cd web/personas-open-source
npm install
npm run dev
```

### Servidor MCP

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

## Uso

### Flujo de la app para usuarios finales

1. Instala la app de Omi desde los enlaces de tienda de arriba.
2. Empareja/usa tu dispositivo Omi.
3. Crea una app mediante el flujo de inicio rápido con webhook.
4. Habla y observa eventos de transcripción en tiempo real en tu endpoint de webhook.

### Backend local con la app

1. Inicia el backend localmente en el puerto `8000`.
2. Expón el backend local mediante un dominio estático de ngrok.
3. Configura `BASE_API_URL` de la app con tu URL de ngrok.
4. Usa la app de Omi contra tu backend local.

### Flujos de trabajo con SDK

- Python SDK: escanea dispositivos BLE con `omi-scan`, decodifica paquetes Opus y transcribe mediante Deepgram.
- React Native SDK: conecta, transmite bytes de audio e inspecciona codec/batería.
- Swift SDK (`omi-lib`): escaneo/conexión/transcripción usando APIs de `OmiManager`.

## Configuración

La configuración está distribuida por componente. Usa la plantilla/readme de cada subproyecto como fuente de verdad.

- `backend/.env.template` -> API keys/configuración de infraestructura del backend
- `web/frontend/.env.template` -> variables de entorno del frontend web
- valores de entorno de `app` -> configuración runtime de la app móvil
- variables de entorno de `mcp` -> `OMI_API_KEY` y opcional `OMI_API_BASE_URL`
- claves específicas de SDK:
  - Python SDK usa `DEEPGRAM_API_KEY`
  - Personas usa variables de entorno de Firebase/OpenRouter/RapidAPI/Mixpanel

Si no estás seguro de qué variables son obligatorias, conserva los valores por defecto y sigue primero el README específico de ese componente antes de eliminar/cambiar valores.

## Ejemplos

### Inicio rápido con webhook (desde el flujo raíz)

Usa [webhook.site](https://webhook.site), instala tu app personalizada en Omi y luego verifica que los eventos de transcripción aparezcan en tiempo real.

### Comando para ejecutar backend

```bash
cd backend
uvicorn main:app --reload --env-file .env
```

### Comando para ejecutar frontend

```bash
cd web/frontend
npm run dev
```

### Escaneo con Python SDK

```bash
cd sdks/python
omi-scan
```

## Notas de Desarrollo

- La automatización de CI/CD y despliegues está configurada en:
  - `.github/workflows/`
  - `codemagic.yaml`
- `scripts/pre-commit` en la raíz formatea archivos staged para:
  - Dart en `app/`
  - Python en `backend/`
  - C/C++ en `omi/` y `omiGlass/`
- `Package.swift` en la raíz del repositorio publica el paquete Swift `omi-lib` desde `sdks/swift`.
- El directorio `i18n/` existe y está reservado para variantes multilingües de README/contenido.

## Solución de Problemas

- Problema de modelo/red del backend en entorno local: si te encuentras con el problema conocido de descarga SSL, aplica el workaround de `ssl` documentado en `backend/README.md` y vuelve a intentarlo.
- La app no puede llegar al backend local: verifica que el dominio de ngrok esté activo y que `BASE_API_URL` apunte a esa URL pública exacta.
- Problemas de descubrimiento BLE: confirma que los permisos de Bluetooth de la plataforma estén otorgados (Terminal/Xcode/app de Android, según corresponda).
- Incompatibilidad de rutas en documentación antigua: algunos textos heredados de docs/referencias pueden mostrar rutas desactualizadas (por ejemplo la ruta raíz de `personas-open-source` o mayúsculas/minúsculas de `omi/OmiGlass`). En este repositorio usa la estructura de directorios actual mostrada arriba.

## Hoja de Ruta

Esta sección refleja señales actuales del repositorio y puede evolucionar:

- Seguir mejorando flujos de firmware/hardware para Omi y OmiGlass
- Expandir el ecosistema de app/plugins y tooling para desarrolladores
- Mejorar experiencias web para memorias/apps/personas
- Fortalecer integraciones de MCP + SDK para ecosistemas externos de agentes
- Añadir y mantener variantes multilingües del README en `i18n/`

## Documentación

- [Introduction](https://docs.omi.me/)
- [omi App setup](https://docs.omi.me/doc/developer/AppSetup)
- [Buying Guide](https://docs.omi.me/doc/assembly/Buying_Guide/)
- [Build the device](https://docs.omi.me/doc/assembly/Build_the_device/)
- [Install firmware](https://docs.omi.me/doc/get_started/Flash_device/)
- [Create your own app in 1 minute](https://docs.omi.me/doc/developer/apps/Introduction)

## Contribuciones

- Revisa nuestra [guía de contribuciones](https://docs.omi.me/doc/developer/Contribution/).
- Gana contribuyendo. Consulta las [recompensas pagadas 🤑](https://omi.me/bounties).
- Revisa los [issues actuales](https://github.com/BasedHardware/Omi/issues).
- Únete a [Discord](http://discord.omi.me).
- Crea tus propios [Plugins/Integrations](https://docs.omi.me/doc/developer/apps/Introduction).

## Soporte y Comunidad

- Sitio principal: [omi.me](https://omi.me/)
- Descargas: [omi.me/download](https://omi.me/download)
- Docs: [docs.omi.me](https://docs.omi.me/)
- Chat de la comunidad: [discord.omi.me](http://discord.omi.me)
- Sigue las novedades: [x.com/kodjima33](https://x.com/kodjima33)
- Hardware/dev kits:
  - [Buy omi Dev Kit](https://www.omi.me/products/omi-dev-kit-2)
  - [Buy Omi Glass Dev Kit](https://www.omi.me/glass)

## Licencia

Omi está disponible bajo la <a href="https://github.com/BasedHardware/omi/blob/main/LICENSE">Licencia MIT</a>
