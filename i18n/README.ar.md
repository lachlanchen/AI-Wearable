[English](../README.md) · [العربية](README.ar.md) · [Español](README.es.md) · [Français](README.fr.md) · [日本語](README.ja.md) · [한국어](README.ko.md) · [Tiếng Việt](README.vi.md) · [中文 (简体)](README.zh-Hans.md) · [中文（繁體）](README.zh-Hant.md) · [Deutsch](README.de.md) · [Русский](README.ru.md)


<p align="center">
  <img src="https://raw.githubusercontent.com/lachlanchen/lachlanchen/main/logos/banner.png" alt="LazyingArt banner" />
</p>

<div align="center">

# **omi**

تعرّف على Omi، جهاز الذكاء الاصطناعي القابل للارتداء مفتوح المصدر الرائد عالميًا، والذي يلتقط المحادثات، ويقدّم الملخصات وعناصر العمل، وينفّذ الإجراءات نيابةً عنك. ما عليك سوى توصيل Omi بجهازك المحمول للاستمتاع بتفريغ تلقائي عالي الجودة للاجتماعات والدردشات والمذكرات الصوتية أينما كنت.

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

## جدول المحتويات

- [نظرة عامة](#نظرة-عامة)
- [الميزات](#الميزات)
- [البدء السريع (دقيقتان)](#البدء-السريع-دقيقتان)
- [بنية المشروع](#بنية-المشروع)
- [المتطلبات المسبقة](#المتطلبات-المسبقة)
- [التثبيت](#التثبيت)
- [الاستخدام](#الاستخدام)
- [الإعداد](#الإعداد)
- [أمثلة](#أمثلة)
- [ملاحظات التطوير](#ملاحظات-التطوير)
- [استكشاف الأخطاء وإصلاحها](#استكشاف-الأخطاء-وإصلاحها)
- [خارطة الطريق](#خارطة-الطريق)
- [التوثيق](#التوثيق)
- [المساهمات](#المساهمات)
- [الدعم والمجتمع](#الدعم-والمجتمع)
- [الترخيص](#الترخيص)

## نظرة عامة

هذا المستودع هو monorepo مفتوح المصدر لمنظومة Omi.

| يتضمن | التفاصيل |
| --- | --- |
| Hardware/Firmware | برمجيات Omi القابلة للارتداء الثابتة + أصول العتاد |
| Omi Glass | البرمجيات الثابتة/العتاد/التطبيق لـ Omi Glass |
| Mobile | تطبيق مرافق مبني بـ Flutter |
| Backend | خدمات خلفية مبنية بـ FastAPI |
| Web | الواجهة الأمامية الرئيسية لـ Omi + Personas |
| Ecosystem | منظومة الإضافات/التكاملات |
| SDKs | Python وReact Native وSwift |
| Agent Infra | خادم MCP |
| Docs | مصدر التوثيق |

تم تصميم البدء السريع في README الجذر ليركّز على تهيئة المستخدم النهائي والمطور. إعداد كل مكوّن بالتفصيل موجود في README الخاص بكل مشروع فرعي وفي توثيق Omi.

## الميزات

- ⚡ تدفقات معالجة صوتية وتفريغ نصي بالذكاء الاصطناعي في الزمن الحقيقي
- 🔋 سير عمل لأجهزة قابلة للارتداء منخفضة استهلاك الطاقة عبر Bluetooth
- 🧩 حزمة برمجية مفتوحة المصدر عبر البرمجيات الثابتة والتطبيقات والخلفية والويب وSDKs
- 🎙️ تجربة استخدام موجّهة للأجهزة القابلة للارتداء للاجتماعات والدردشات والمذكرات الصوتية
- 🔗 منظومة webhook/تطبيقات لتشغيل إجراءات مخصصة
- 🛠️ بنية إضافات/تكاملات لتوسيع الإمكانات

## البدء السريع (دقيقتان)

### 1) تنزيل تطبيق omi

[<img src='https://upload.wikimedia.org/wikipedia/commons/7/78/Google_Play_Store_badge_EN.svg' alt='Get it on Google Play' height="50px" width="180px">](https://play.google.com/store/apps/details?id=com.friend.ios)
[<img src='https://upload.wikimedia.org/wikipedia/commons/3/3c/Download_on_the_App_Store_Badge.svg' alt="Download on the App Store" height="50px" width="180px">](https://apps.apple.com/us/app/friend-ai-wearable/id6502156163)
[<img src='https://github.com/user-attachments/assets/59c47ec7-3da0-47d7-be2f-7467e4189499' alt="Download MacOS app" height="50px" width="180px">](https://apps.apple.com/us/app/omi-ai-smart-meeting-notes/id6502156163)

### 2) إنشاء webhook

أنشئ webhook باستخدام [webhook.site](https://webhook.site) ثم انسخ هذا الرابط.

<img src="https://github.com/user-attachments/assets/083a6ec4-4694-4c7a-843a-4a1a0c254453" width="500">

### 3) داخل تطبيق omi

| Explore => Create an App                                                                                  | Select Capability                                                                                       | Paste Webhook URL                                                                                         | Install App                                                                                             |
| --------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------- |
| <img src="https://github.com/user-attachments/assets/31809b81-7de2-4381-b5fc-5c9714972211" width="200"> | <img src="https://github.com/user-attachments/assets/59cfbe8e-7e3b-437f-81f7-25eb50ccdd7d" width="200"> | <img src="https://github.com/user-attachments/assets/3d864ee8-555f-4ded-b4db-87ff78128323" width = "200"> | <img src="https://github.com/user-attachments/assets/58cf6da6-e245-415e-92e7-dc1f46583cfc" width="200"> |

### 4) تحدّث وتحقّق من الأحداث

ابدأ بالتحدث، وسترى التفريغ النصي الفوري على [webhook.site](https://webhook.site).

## بنية المشروع

### في هذا المستودع

- [omi device](https://github.com/BasedHardware/omi/tree/main/omi)
- [omi glass](https://github.com/BasedHardware/omi/tree/main/omiGlass)
- [omi app](https://github.com/BasedHardware/omi/tree/main/app)
- [ai personas (web)](https://github.com/BasedHardware/omi/tree/main/web/personas-open-source)
- [SDKs](./sdks)

ملاحظة: قد تشير المراجع الأقدم إلى `personas-open-source` في جذر المستودع؛ في هذا المستودع يوجد حاليًا تحت `web/personas-open-source`.

### خريطة عالية المستوى

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

## المتطلبات المسبقة

استخدم المتطلبات المناسبة للمكوّن الذي تعمل عليه.

| الأدوات | الاستخدام |
| --- | --- |
| Git | التحكم بالإصدار المصدري |
| Node.js 18+ and npm | الويب وpersonas وبعض تدفقات plugins |
| Python 3.10+ | الخلفية وMCP وPython SDK |
| Flutter SDK | تطبيق الهاتف المحمول |
| Xcode/CocoaPods | تطوير iOS |
| Android Studio + Android SDK | تطوير Android |
| `ffmpeg` + `opus` | تدفقات الخلفية/الصوت |
| Docker (optional) | نشر MCP/الويب |
| Google Cloud + Firebase | تدفقات الخلفية/التطبيق |

## التثبيت

لأن هذا المستودع من نوع monorepo، قم بالتثبيت لكل مكوّن على حدة.

### استنساخ المستودع

```bash
git clone https://github.com/BasedHardware/omi.git
cd omi
```

### التطبيق (Flutter)

```bash
cd app
bash setup.sh ios
# or
bash setup.sh android

flutter run --flavor dev
```

### الخلفية (FastAPI)

```bash
cd backend
cp .env.template .env
pip install -r requirements.txt
uvicorn main:app --reload --env-file .env
```

### الواجهة الأمامية الرئيسية (Next.js)

```bash
cd web/frontend
npm install
cp .env.template .env.local
npm run dev
```

### تطبيق Personas للويب (Next.js)

```bash
cd web/personas-open-source
npm install
npm run dev
```

### خادم MCP

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

## الاستخدام

### تدفق استخدام التطبيق للمستخدم النهائي

1. ثبّت تطبيق Omi من روابط المتجر أعلاه.
2. قم بإقران/استخدام جهاز Omi الخاص بك.
3. أنشئ تطبيقًا عبر تدفق البدء السريع لـ webhook.
4. تحدّث وراقب أحداث التفريغ النصي الفوري على نقطة نهاية webhook الخاصة بك.

### تشغيل الخلفية محليًا مع التطبيق

1. شغّل الخلفية محليًا على المنفذ `8000`.
2. اكشف الخلفية المحلية عبر نطاق ngrok ثابت.
3. اضبط `BASE_API_URL` في التطبيق ليشير إلى رابط ngrok الخاص بك.
4. استخدم تطبيق Omi مع الخلفية المحلية.

### تدفقات SDK

- Python SDK: افحص أجهزة BLE عبر `omi-scan`، وفك ترميز حزم Opus، ثم نفّذ التفريغ عبر Deepgram.
- React Native SDK: اتصل، وابث بايتات الصوت، وافحص codec/البطارية.
- Swift SDK (`omi-lib`): امسح/اتصل/فرّغ باستخدام واجهات `OmiManager`.

## الإعداد

الإعداد موزّع حسب المكوّن. استخدم قالب/README كل مشروع فرعي كمصدر الحقيقة.

- `backend/.env.template` -> مفاتيح API للبنية الخلفية وإعدادات البنية التحتية
- `web/frontend/.env.template` -> متغيرات البيئة للواجهة الأمامية
- قيم البيئة في `app` -> إعدادات وقت التشغيل لتطبيق الهاتف
- متغيرات بيئة `mcp` -> `OMI_API_KEY` و`OMI_API_BASE_URL` (اختياري)
- مفاتيح خاصة بـ SDK:
  - Python SDK يستخدم `DEEPGRAM_API_KEY`
  - Personas يستخدم متغيرات Firebase/OpenRouter/RapidAPI/Mixpanel

إذا لم تكن متأكدًا من المتغيرات المطلوبة، حافظ على القيم الافتراضية واتبع README الخاص بذلك المكوّن قبل إزالة/تغيير أي قيمة.

## أمثلة

### بدء سريع عبر Webhook (من التدفق الجذري)

استخدم [webhook.site](https://webhook.site)، وثبّت تطبيقك المخصص داخل Omi، ثم تحقّق من ظهور أحداث التفريغ النصي في الزمن الحقيقي.

### أمر تشغيل الخلفية

```bash
cd backend
uvicorn main:app --reload --env-file .env
```

### أمر تشغيل الواجهة الأمامية

```bash
cd web/frontend
npm run dev
```

### فحص Python SDK

```bash
cd sdks/python
omi-scan
```

## ملاحظات التطوير

- تمت تهيئة أتمتة CI/CD والنشر في:
  - `.github/workflows/`
  - `codemagic.yaml`
- يقوم `scripts/pre-commit` في الجذر بتنسيق الملفات staged لـ:
  - Dart في `app/`
  - Python في `backend/`
  - C/C++ في `omi/` و`omiGlass/`
- ملف `Package.swift` في جذر المستودع ينشر حزمة Swift باسم `omi-lib` من `sdks/swift`.
- دليل `i18n/` موجود ومخصص لنسخ README/المحتوى متعددة اللغات.

## استكشاف الأخطاء وإصلاحها

- مشكلة نموذج/شبكة في الخلفية أثناء الإعداد المحلي: إذا واجهت مشكلة SSL المعروفة عند التنزيل، طبّق حل `ssl` الموثق في `backend/README.md` ثم أعد المحاولة.
- التطبيق لا يصل إلى الخلفية المحلية: تحقّق من أن نطاق ngrok يعمل وأن `BASE_API_URL` يشير إلى نفس الرابط العام تمامًا.
- مشكلات اكتشاف BLE: تأكد من منح أذونات Bluetooth على المنصة المعنية (Terminal/Xcode/تطبيق Android حسب الحالة).
- عدم تطابق المسارات في التوثيق القديم: قد تعرض بعض المستندات/المراجع القديمة مسارات غير محدثة (مثل مسار الجذر `personas-open-source` أو حالة الأحرف `omi/OmiGlass`). في هذا المستودع استخدم تخطيط الأدلة الحالي الموضّح أعلاه.

## خارطة الطريق

يعكس هذا القسم الإشارات الحالية في المستودع وقد يتطور لاحقًا:

- الاستمرار في تحسين تدفقات البرمجيات الثابتة/العتاد لـ Omi وOmiGlass
- توسيع منظومة التطبيق/الإضافات وأدوات المطور
- تحسين تجارب الويب للذكريات/التطبيقات/personas
- تعزيز تكامل MCP + SDK لمنظومات الوكلاء الخارجية
- إضافة وصيانة نسخ README متعددة اللغات في `i18n/`

## التوثيق

- [Introduction](https://docs.omi.me/)
- [omi App setup](https://docs.omi.me/doc/developer/AppSetup)
- [Buying Guide](https://docs.omi.me/doc/assembly/Buying_Guide/)
- [Build the device](https://docs.omi.me/doc/assembly/Build_the_device/)
- [Install firmware](https://docs.omi.me/doc/get_started/Flash_device/)
- [Create your own app in 1 minute](https://docs.omi.me/doc/developer/apps/Introduction)

## المساهمات

- اطّلع على [دليل المساهمات](https://docs.omi.me/doc/developer/Contribution/).
- اربح من المساهمة! راجع [المهام المدفوعة 🤑](https://omi.me/bounties).
- اطّلع على [القضايا الحالية](https://github.com/BasedHardware/Omi/issues).
- انضم إلى [Discord](http://discord.omi.me).
- ابنِ [Plugins/Integrations](https://docs.omi.me/doc/developer/apps/Introduction) الخاصة بك.

## الدعم والمجتمع

- الموقع الرئيسي: [omi.me](https://omi.me/)
- التنزيلات: [omi.me/download](https://omi.me/download)
- التوثيق: [docs.omi.me](https://docs.omi.me/)
- دردشة المجتمع: [discord.omi.me](http://discord.omi.me)
- تابع التحديثات: [x.com/kodjima33](https://x.com/kodjima33)
- العتاد/حِزم المطور:
  - [Buy omi Dev Kit](https://www.omi.me/products/omi-dev-kit-2)
  - [Buy Omi Glass Dev Kit](https://www.omi.me/glass)

## الترخيص

يتوفر Omi بموجب <a href="https://github.com/BasedHardware/omi/blob/main/LICENSE">MIT License</a>
