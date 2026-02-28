[English](../README.md) · [العربية](README.ar.md) · [Español](README.es.md) · [Français](README.fr.md) · [日本語](README.ja.md) · [한국어](README.ko.md) · [Tiếng Việt](README.vi.md) · [中文 (简体)](README.zh-Hans.md) · [中文（繁體）](README.zh-Hant.md) · [Deutsch](README.de.md) · [Русский](README.ru.md)


[![LazyingArt banner](https://github.com/lachlanchen/lachlanchen/raw/main/figs/banner.png)](https://github.com/lachlanchen/lachlanchen/blob/main/figs/banner.png)

<div align="center">

# **omi**

_Wearable con IA para reuniones y conversaciones instantáneas: captura, resume y ejecuta acciones, sin usar las manos._

Conoce Omi, el wearable de IA open source líder mundial que capta conversaciones, genera resúmenes y acciones, y ejecuta tareas por ti. Simplemente conecta Omi a tu dispositivo móvil y disfruta de transcripciones automáticas de alta calidad de reuniones, charlas y notas de voz desde donde estés.

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

## ⚡ Enlaces rápidos

| Recurso | Enlace |
| --- | --- |
| 🌐 Sitio del proyecto | [omi.me](https://omi.me/) |
| ⬇️ Centro de descargas | [omi.me/download](https://omi.me/download) |
| 📚 Documentación | [docs.omi.me](https://docs.omi.me/) |
| 🛠️ Kit de desarrollo Omi | [Comprar Omi Dev Kit](https://www.omi.me/products/omi-dev-kit-2) |
| 👓 Kit de desarrollo Omi Glass | [Comprar Omi Glass](https://www.omi.me/glass) |

---

## Tabla de contenidos

- [📌 Visión general](#visión-general)
- [⚡️ Características](#características)
- [🚀 Inicio rápido (2 min)](#inicio-rápido-2-min)
- [🏗️ Estructura del proyecto](#estructura-del-proyecto)
- [🧰 Prerrequisitos](#prerrequisitos)
- [🛠️ Instalación](#instalación)
- [🧪 Uso](#uso)
- [⚙️ Configuración](#configuración)
- [🧾 Ejemplos](#ejemplos)
- [🧭 Notas de desarrollo](#notas-de-desarrollo)
- [🐞 Solución de problemas](#solución-de-problemas)
- [🗺️ Hoja de ruta](#hoja-de-ruta)
- [📚 Documentación](#documentación)
- [🤝 Contribución](#contribución)
- [❤️ Support](#%E2%9D%A4%EF%B8%8F-support)
- [💬 Contacto y comunidad](#contacto-y-comunidad)
- [📜 Licencia](#licencia)

## Visión general

Este repositorio es el monorepo del ecosistema open source de Omi.

| Incluye | Detalles |
| --- | --- |
| 🧠 Omi Hardware | Firmware de Omi + activos de hardware |
| 🥽 Omi Glass | Firmware/hardware/app de Omi Glass |
| 📱 Mobile | Aplicación companion en Flutter |
| 🌐 Backend | Servicios backend con FastAPI |
| 🕸️ Web | Frontend principal de Omi + Personas |
| 🧩 Ecosistema | Ecosistema de plugins/integraciones |
| 📦 SDKs | Python, React Native, Swift |
| 🔗 Agent Infra | Servidor MCP |
| 📘 Docs | Fuente de documentación |

El README raíz está enfocado en onboarding y en el flujo de trabajo diario del desarrollo. La configuración completa por componente y notas operativas más profundas viven en los README de cada subproyecto y en `docs/`.

## Características

- ⚡ Procesamiento de audio y transcripción en tiempo real con IA
- 🔋 Flujos de trabajo para wearables con Bluetooth de bajo consumo
- 🧩 Stack software open source en firmware, apps, backend, web y SDKs
- 🎙️ UX centrada en wearables para reuniones, chats y notas de voz
- 🔗 Ecosistema webhook/app para disparar acciones personalizadas
- 🛠️ Arquitectura de plugins e integraciones para ampliar capacidades

## Inicio rápido (2 min)

### 1) Descargar la app de omi

[<img src='https://upload.wikimedia.org/wikipedia/commons/7/78/Google_Play_Store_badge_EN.svg' alt='Get it on Google Play' height="50px" width="180px">](https://play.google.com/store/apps/details?id=com.friend.ios)
[<img src='https://upload.wikimedia.org/wikipedia/commons/3/3c/Download_on_the_App_Store_Badge.svg' alt="Download on the App Store" height="50px" width="180px">](https://apps.apple.com/us/app/friend-ai-wearable/id6502156163)
[<img src='https://github.com/user-attachments/assets/59c47ec7-3da0-47d7-be2f-7467e4189499' alt="Download MacOS app" height="50px" width="180px">](https://apps.apple.com/us/app/omi-ai-smart-meeting-notes/id6502156163)

### 2) Crear un webhook

Crea un webhook en [webhook.site](https://webhook.site) y copia esta URL.

<img src="https://github.com/user-attachments/assets/083a6ec4-4694-4c7a-843a-4a1a0c254453" width="500">

### 3) En la app de omi

| Explorar => Crear app                                                                                  | Seleccionar capacidad                                                                                           | Pegar URL de webhook                                                                                         | Instalar app                                                                                             |
| ------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------- |
| <img src="https://github.com/user-attachments/assets/31809b81-7de2-4381-b5fc-5c9714972211" width="200"> | <img src="https://github.com/user-attachments/assets/59cfbe8e-7e3b-437f-81f7-25eb50ccdd7d" width="200"> | <img src="https://github.com/user-attachments/assets/3d864ee8-555f-4ded-b4db-87ff78128323" width="200"> | <img src="https://github.com/user-attachments/assets/58cf6da6-e245-415e-92e7-dc1f46583cfc" width="200"> |

### 4) Hablar y verificar eventos

Empieza a hablar; verás la transcripción en tiempo real en [webhook.site](https://webhook.site).

## Estructura del proyecto

### En este repositorio

| Componente | Propósito |
| --- | --- |
| [omi device](https://github.com/BasedHardware/omi/tree/main/omi) | Hardware + firmware de Omi |
| [omi glass](https://github.com/BasedHardware/omi/tree/main/omiGlass) | Hardware + firmware de Omi Glass |
| [omi app](https://github.com/BasedHardware/omi/tree/main/app) | Aplicación companion Flutter |
| [ai personas (web)](https://github.com/BasedHardware/omi/tree/main/web/personas-open-source) | App web de personas |
| [SDKs](./sdks) | SDKs de Python, React Native y Swift |

Nota: es posible que referencias antiguas mencionen `personas-open-source` en la raíz del repositorio; en este repositorio actualmente se encuentra bajo `web/personas-open-source`.

### Mapa de alto nivel

```text
.
├── app/                     # App companion Flutter
├── backend/                 # Backend FastAPI
├── docs/                    # Documentación Mintlify
├── mcp/                     # Servidor MCP para recuerdos/conversaciones
├── omi/                     # Hardware + firmware Omi
├── omiGlass/                # Hardware + firmware + app Omi Glass
├── plugins/                 # Integraciones/apps/plugins
├── sdks/                    # python / react-native / swift
├── web/frontend/            # Frontend Next.js principal
├── web/personas-open-source/ # App web Personas
├── scripts/                 # herramientas (format hooks, ayuda OTA)
└── i18n/                    # Contenido multilingüe y traducciones
```

## Prerrequisitos

Usa los requisitos relevantes para tu componente objetivo.

| Herramienta | Usado para |
| --- | --- |
| Git | Control de versiones |
| Node.js 18+ y npm | web, personas, algunos flujos de plugins |
| Python 3.10+ | backend, MCP, SDK Python |
| Flutter SDK | app móvil |
| Xcode/CocoaPods | desarrollo de iOS |
| Android Studio + Android SDK | desarrollo de Android |
| `ffmpeg` + `opus` | flujos de audio/backend |
| Docker (opcional) | despliegues MCP/web |
| Google Cloud + Firebase | flujos de backend/app |

### Supuestos para la configuración

- Algunos comandos dependen de credenciales externas (Firebase, OpenAI/Deepgram/proveedores de API), que normalmente configuras por componente usando su plantilla `.env`. Consulta los README de cada componente si faltan valores en la documentación local.
- Si solo necesitas una superficie, instala/compila solo ese componente para mantener rápida la iteración.

## Instalación

Dado que este es un monorepo, instala por componente.

### Clonar repositorio

```bash
git clone https://github.com/BasedHardware/omi.git
cd omi
```

### App (Flutter)

```bash
cd app
bash setup.sh ios
# o
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

### App web de personas (Next.js)

```bash
cd web/personas-open-source
npm install
npm run dev
```

### Servidor MCP

```bash
cd mcp
# Consulta mcp/README.md para configurar Claude Desktop con Docker
```

### SDKs

```bash
cd sdks/python && pip install -e .
cd ../react-native && npm install
# El paquete Swift se expone a través de Package.swift en la raíz como `omi-lib`
```

## Uso

### Flujo de app para usuario final

1. Instala la app Omi desde los enlaces de tienda de arriba.
2. Empareja/usa tu dispositivo Omi.
3. Crea una app a través del flujo de inicio rápido con webhook.
4. Habla y observa los eventos de transcripción en tiempo real en tu endpoint de webhook.

### Backend local con app

1. Inicia el backend localmente en el puerto `8000`.
2. Exponlo usando un dominio estático de ngrok.
3. Configura `BASE_API_URL` en la app con tu URL de ngrok.
4. Usa la app Omi contra tu backend local.

### Flujos de trabajo de SDK

- SDK de Python: escanea dispositivos BLE con `omi-scan`, decodifica paquetes Opus y transcribe con Deepgram.
- SDK de React Native: conecta, transmite bytes de audio y revisa códec/batería.
- SDK de Swift (`omi-lib`): escanea/conecta/transcribe usando APIs de `OmiManager`.

## Configuración

La configuración se distribuye por componente. Usa la plantilla/README de cada subproyecto como fuente de verdad.

- `backend/.env.template` -> claves de API/config de infraestructura de backend
- `web/frontend/.env.template` -> variables de entorno del frontend web
- valores de entorno de `app` -> configuración runtime de la app móvil
- variables de entorno de `mcp` -> `OMI_API_KEY` y `OMI_API_BASE_URL` opcional
- claves específicas por SDK:
  - El SDK de Python usa `DEEPGRAM_API_KEY`
  - Personas usa variables de Firebase/OpenRouter/RapidAPI/Mixpanel

Si no tienes claro qué variables son obligatorias, conserva los valores por defecto y sigue el README específico de ese componente antes de quitar o cambiar valores.

## Ejemplos

### Inicio rápido de webhook (desde el flujo raíz)

Usa [webhook.site](https://webhook.site), instala tu app personalizada en Omi y luego verifica que aparezcan eventos de transcripción en tiempo real.

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

### Escaneo con SDK de Python

```bash
cd sdks/python
omi-scan
```

## Notas de desarrollo

- CI/CD y automatización de despliegue están configurados en:
  - `.github/workflows/`
  - `codemagic.yaml`
- El script `scripts/pre-commit` de raíz da formato a archivos en staging para:
  - Dart en `app/`
  - Python en `backend/`
  - C/C++ en `omi/` y `omiGlass/`
- `Package.swift` en la raíz publica el paquete Swift `omi-lib` desde `sdks/swift`.
- El directorio `i18n/` existe y está reservado para variantes multilingües del README/contenido.

## Solución de problemas

- Problema de modelo/red en configuración local: si encuentras el problema conocido de SSL al descargar, aplica la solución `ssl` documentada en `backend/README.md` y vuelve a intentarlo.
- La app no puede llegar al backend local: verifica que el dominio de ngrok esté activo y que `BASE_API_URL` apunte a esa URL pública exacta.
- Problemas de descubrimiento BLE: confirma que los permisos de Bluetooth estén concedidos en la plataforma correspondiente (Terminal/Xcode/app de Android según aplique).
- Desajuste de rutas en docs antiguas: algunos textos antiguos pueden mostrar rutas obsoletas (por ejemplo, ruta raíz `personas-open-source` o mayúsculas de `omi/OmiGlass`). En este repositorio usa el layout actual que aparece arriba.

## Hoja de ruta

Esta sección refleja las señales actuales del repositorio y puede cambiar:

- Seguir mejorando flujos de firmware/hardware para Omi y OmiGlass
- Expandir el ecosistema de app/plugins y herramientas de desarrollo
- Mejorar experiencias web para recuerdos/apps/personas
- Fortalecer MCP + integraciones de SDK para ecosistemas externos de agentes
- Añadir y mantener variantes multilingües del README en `i18n/`

## Documentación

- [Introduction](https://docs.omi.me/)
- [Configuración de la app Omi](https://docs.omi.me/doc/developer/AppSetup)
- [Guía de compra](https://docs.omi.me/doc/assembly/Buying_Guide/)
- [Construye el dispositivo](https://docs.omi.me/doc/assembly/Build_the_device/)
- [Instalar firmware](https://docs.omi.me/doc/get_started/Flash_device/)
- [Crear tu propia app en 1 minuto](https://docs.omi.me/doc/developer/apps/Introduction)

## Contribución

- Consulta nuestra [guía de contribución](https://docs.omi.me/doc/developer/Contribution/).
- ¡Gana dinero contribuyendo! Consulta las [recompensas pagadas 🤑](https://omi.me/bounties).
- Revisa los [issues actuales](https://github.com/BasedHardware/Omi/issues).
- Únete a [Discord](http://discord.omi.me).
- Crea tus propios [Plugins/Integraciones](https://docs.omi.me/doc/developer/apps/Introduction).

## ❤️ Support

| Donate | PayPal | Stripe |
| --- | --- | --- |
| [![Donate](https://camo.githubusercontent.com/24a4914f0b42c6f435f9e101621f1e52535b02c225764b2f6cc99416926004b7/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f446f6e6174652d4c617a79696e674172742d3045413545393f7374796c653d666f722d7468652d6261646765266c6f676f3d6b6f2d6669266c6f676f436f6c6f723d7768697465)](https://chat.lazying.art/donate) | [![PayPal](https://camo.githubusercontent.com/d0f57e8b016517a4b06961b24d0ca87d62fdba16e18bbdb6aba28e978dc0ea21/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f50617950616c2d526f6e677a686f754368656e2d3030343537433f7374796c653d666f722d7468652d6261646765266c6f676f3d70617970616c266c6f676f436f6c6f723d7768697465)](https://paypal.me/RongzhouChen) | [![Stripe](https://camo.githubusercontent.com/1152dfe04b6943afe3a8d2953676749603fb9f95e24088c92c97a01a897b4942/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f5374726970652d446f6e6174652d3633354246463f7374796c653d666f722d7468652d6261646765266c6f676f3d737472697065266c6f676f436f6c6f723d7768697465)](https://buy.stripe.com/aFadR8gIaflgfQV6T4fw400) |

## Contacto y comunidad

- Sitio principal: [omi.me](https://omi.me/)
- Descargas: [omi.me/download](https://omi.me/download)
- Docs: [docs.omi.me](https://docs.omi.me/)
- Chat comunitario: [discord.omi.me](http://discord.omi.me)
- Seguir actualizaciones: [x.com/kodjima33](https://x.com/kodjima33)
- Kits de hardware:
  - [Comprar Omi Dev Kit](https://www.omi.me/products/omi-dev-kit-2)
  - [Comprar Omi Glass Dev Kit](https://www.omi.me/glass)

## Licencia

Omi está disponible bajo <a href="https://github.com/BasedHardware/omi/blob/main/LICENSE">licencia MIT</a>
