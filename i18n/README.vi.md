[English](../README.md) · [العربية](README.ar.md) · [Español](README.es.md) · [Français](README.fr.md) · [日本語](README.ja.md) · [한국어](README.ko.md) · [Tiếng Việt](README.vi.md) · [中文 (简体)](README.zh-Hans.md) · [中文（繁體）](README.zh-Hant.md) · [Deutsch](README.de.md) · [Русский](README.ru.md)



<p align="center">
  <img src="https://raw.githubusercontent.com/lachlanchen/lachlanchen/main/logos/banner.png" alt="LazyingArt banner" />
</p>

<div align="center">

# **omi**

Gặp Omi, thiết bị đeo AI mã nguồn mở hàng đầu thế giới có thể ghi lại hội thoại, tạo tóm tắt, liệt kê việc cần làm và tự động thực hiện hành động cho bạn. Chỉ cần kết nối Omi với thiết bị di động để có bản chép lời chất lượng cao, tự động cho cuộc họp, trò chuyện và ghi chú giọng nói ở bất kỳ đâu.

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

## Mục lục

- [Tổng quan](#tổng-quan)
- [Tính năng](#tính-năng)
- [Bắt đầu nhanh (2 phút)](#bắt-đầu-nhanh-2-phút)
- [Cấu trúc dự án](#cấu-trúc-dự-án)
- [Yêu cầu trước khi cài đặt](#yêu-cầu-trước-khi-cài-đặt)
- [Cài đặt](#cài-đặt)
- [Cách sử dụng](#cách-sử-dụng)
- [Cấu hình](#cấu-hình)
- [Ví dụ](#ví-dụ)
- [Ghi chú phát triển](#ghi-chú-phát-triển)
- [Khắc phục sự cố](#khắc-phục-sự-cố)
- [Lộ trình](#lộ-trình)
- [Tài liệu](#tài-liệu)
- [Đóng góp](#đóng-góp)
- [Hỗ trợ và cộng đồng](#hỗ-trợ-và-cộng-đồng)
- [Giấy phép](#giấy-phép)

## Tổng quan

Repository này là monorepo mã nguồn mở của toàn bộ hệ sinh thái Omi.

| Bao gồm | Chi tiết |
| --- | --- |
| Hardware/Firmware | Firmware thiết bị đeo Omi + tài nguyên phần cứng |
| Omi Glass | Firmware/phần cứng/app của Omi Glass |
| Mobile | Ứng dụng đồng hành Flutter |
| Backend | Dịch vụ backend FastAPI |
| Web | Frontend Omi chính + Personas |
| Ecosystem | Hệ sinh thái plugin/tích hợp |
| SDKs | Python, React Native, Swift |
| Agent Infra | MCP server |
| Docs | Mã nguồn tài liệu |

README ở thư mục gốc được tối ưu để onboard người dùng/nhà phát triển. Thiết lập chi tiết theo từng thành phần nằm trong README của từng subproject và tài liệu Omi.

## Tính năng

- ⚡ Luồng xử lý âm thanh AI và chép lời theo thời gian thực
- 🔋 Quy trình thiết bị đeo Bluetooth tiêu thụ điện năng thấp
- 🧩 Stack mã nguồn mở xuyên suốt firmware, app, backend, web và SDK
- 🎙️ UX ưu tiên thiết bị đeo cho họp, trò chuyện và ghi chú giọng nói
- 🔗 Hệ sinh thái webhook/app để kích hoạt hành động tùy chỉnh
- 🛠️ Kiến trúc plugin/integration để mở rộng khả năng

## Bắt đầu nhanh (2 phút)

### 1) Tải ứng dụng omi

[<img src='https://upload.wikimedia.org/wikipedia/commons/7/78/Google_Play_Store_badge_EN.svg' alt='Get it on Google Play' height="50px" width="180px">](https://play.google.com/store/apps/details?id=com.friend.ios)
[<img src='https://upload.wikimedia.org/wikipedia/commons/3/3c/Download_on_the_App_Store_Badge.svg' alt="Download on the App Store" height="50px" width="180px">](https://apps.apple.com/us/app/friend-ai-wearable/id6502156163)
[<img src='https://github.com/user-attachments/assets/59c47ec7-3da0-47d7-be2f-7467e4189499' alt="Download MacOS app" height="50px" width="180px">](https://apps.apple.com/us/app/omi-ai-smart-meeting-notes/id6502156163)

### 2) Tạo webhook

Tạo webhook bằng [webhook.site](https://webhook.site) và sao chép URL này.

<img src="https://github.com/user-attachments/assets/083a6ec4-4694-4c7a-843a-4a1a0c254453" width="500">

### 3) Trong ứng dụng omi

| Explore => Create an App                                                                                  | Select Capability                                                                                       | Paste Webhook URL                                                                                         | Install App                                                                                             |
| --------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------- |
| <img src="https://github.com/user-attachments/assets/31809b81-7de2-4381-b5fc-5c9714972211" width="200"> | <img src="https://github.com/user-attachments/assets/59cfbe8e-7e3b-437f-81f7-25eb50ccdd7d" width="200"> | <img src="https://github.com/user-attachments/assets/3d864ee8-555f-4ded-b4db-87ff78128323" width = "200"> | <img src="https://github.com/user-attachments/assets/58cf6da6-e245-415e-92e7-dc1f46583cfc" width="200"> |

### 4) Nói và xác minh sự kiện

Bắt đầu nói, bạn sẽ thấy bản chép lời theo thời gian thực trên [webhook.site](https://webhook.site).

## Cấu trúc dự án

### Trong repo này

- [omi device](https://github.com/BasedHardware/omi/tree/main/omi)
- [omi glass](https://github.com/BasedHardware/omi/tree/main/omiGlass)
- [omi app](https://github.com/BasedHardware/omi/tree/main/app)
- [ai personas (web)](https://github.com/BasedHardware/omi/tree/main/web/personas-open-source)
- [SDKs](./sdks)

Lưu ý: một số tài liệu cũ có thể nhắc `personas-open-source` ở thư mục gốc; trong repo này hiện nằm dưới `web/personas-open-source`.

### Bản đồ tổng quan

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

## Yêu cầu trước khi cài đặt

Dùng các yêu cầu phù hợp với thành phần bạn muốn chạy.

| Công cụ | Dùng cho |
| --- | --- |
| Git | Quản lý mã nguồn |
| Node.js 18+ and npm | web, personas, một số workflow plugin |
| Python 3.10+ | backend, MCP, Python SDK |
| Flutter SDK | ứng dụng mobile |
| Xcode/CocoaPods | phát triển iOS |
| Android Studio + Android SDK | phát triển Android |
| `ffmpeg` + `opus` | workflow backend/audio |
| Docker (optional) | triển khai MCP/web |
| Google Cloud + Firebase | workflow backend/app |

## Cài đặt

Vì đây là monorepo, hãy cài đặt theo từng thành phần.

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

## Cách sử dụng

### Luồng sử dụng cho người dùng cuối

1. Cài ứng dụng Omi từ các liên kết store ở trên.
2. Ghép nối/sử dụng thiết bị Omi của bạn.
3. Tạo app theo luồng webhook quick-start.
4. Nói và quan sát sự kiện chép lời theo thời gian thực tại endpoint webhook của bạn.

### Chạy backend local với app

1. Khởi động backend local trên cổng `8000`.
2. Expose backend local qua domain tĩnh ngrok.
3. Đặt `BASE_API_URL` của app thành URL ngrok của bạn.
4. Dùng ứng dụng Omi với backend local.

### Quy trình SDK

- Python SDK: quét thiết bị BLE bằng `omi-scan`, giải mã gói Opus và chép lời qua Deepgram.
- React Native SDK: kết nối, stream byte âm thanh, kiểm tra codec/pin.
- Swift SDK (`omi-lib`): quét/kết nối/chép lời bằng API `OmiManager`.

## Cấu hình

Cấu hình được phân tán theo từng thành phần. Dùng template/readme của mỗi subproject làm nguồn tham chiếu chính.

- `backend/.env.template` -> cấu hình khóa API/hạ tầng backend
- `web/frontend/.env.template` -> biến môi trường frontend web
- giá trị môi trường của `app` -> cấu hình runtime cho ứng dụng mobile
- biến môi trường `mcp` -> `OMI_API_KEY` và tùy chọn `OMI_API_BASE_URL`
- Khóa riêng cho SDK:
  - Python SDK dùng `DEEPGRAM_API_KEY`
  - Personas dùng biến môi trường Firebase/OpenRouter/RapidAPI/Mixpanel

Nếu bạn chưa chắc biến nào là bắt buộc, hãy giữ nguyên mặc định và làm theo README của thành phần đó trước khi xóa/thay đổi giá trị.

## Ví dụ

### Webhook quick-start (từ luồng root)

Dùng [webhook.site](https://webhook.site), cài app tùy chỉnh của bạn trong Omi, rồi xác minh rằng sự kiện transcript xuất hiện theo thời gian thực.

### Lệnh chạy backend

```bash
cd backend
uvicorn main:app --reload --env-file .env
```

### Lệnh chạy frontend

```bash
cd web/frontend
npm run dev
```

### Quét bằng Python SDK

```bash
cd sdks/python
omi-scan
```

## Ghi chú phát triển

- Cấu hình tự động hóa CI/CD và triển khai nằm ở:
  - `.github/workflows/`
  - `codemagic.yaml`
- `scripts/pre-commit` ở root sẽ format các file đã stage cho:
  - Dart trong `app/`
  - Python trong `backend/`
  - C/C++ trong `omi/` và `omiGlass/`
- `Package.swift` ở root repo phát hành Swift package `omi-lib` từ `sdks/swift`.
- Thư mục `i18n/` đã tồn tại và được dành cho các biến thể README/nội dung đa ngôn ngữ.

## Khắc phục sự cố

- Lỗi model/network backend khi chạy local: nếu gặp lỗi SSL download đã biết, hãy áp dụng cách xử lý `ssl` được ghi trong `backend/README.md` rồi thử lại.
- App không gọi được backend local: xác minh domain ngrok đang chạy và `BASE_API_URL` trỏ đúng URL public đó.
- Sự cố phát hiện BLE: xác nhận quyền Bluetooth trên nền tảng tương ứng đã được cấp (Terminal/Xcode/Android app tùy trường hợp).
- Sai đường dẫn trong tài liệu cũ: một số tài liệu cũ có thể hiển thị đường dẫn lỗi thời (ví dụ đường dẫn root `personas-open-source` hoặc kiểu chữ hoa/thường `omi/OmiGlass`). Trong repo này, dùng layout thư mục hiện tại như ở trên.

## Lộ trình

Phần này phản ánh tín hiệu hiện tại của repository và có thể thay đổi:

- Tiếp tục cải thiện quy trình firmware/phần cứng cho Omi và OmiGlass
- Mở rộng hệ sinh thái app/plugin và tooling cho nhà phát triển
- Nâng cao trải nghiệm web cho memories/apps/personas
- Tăng cường tích hợp MCP + SDK cho hệ sinh thái agent bên ngoài
- Thêm và duy trì các biến thể README đa ngôn ngữ trong `i18n/`

## Tài liệu

- [Introduction](https://docs.omi.me/)
- [omi App setup](https://docs.omi.me/doc/developer/AppSetup)
- [Buying Guide](https://docs.omi.me/doc/assembly/Buying_Guide/)
- [Build the device](https://docs.omi.me/doc/assembly/Build_the_device/)
- [Install firmware](https://docs.omi.me/doc/get_started/Flash_device/)
- [Create your own app in 1 minute](https://docs.omi.me/doc/developer/apps/Introduction)

## Đóng góp

- Xem [hướng dẫn đóng góp](https://docs.omi.me/doc/developer/Contribution/).
- Có thể kiếm tiền khi đóng góp! Xem [paid bounties 🤑](https://omi.me/bounties).
- Xem [các issue hiện tại](https://github.com/BasedHardware/Omi/issues).
- Tham gia [Discord](http://discord.omi.me).
- Tự xây dựng [Plugins/Integrations](https://docs.omi.me/doc/developer/apps/Introduction).

## Hỗ trợ và cộng đồng

- Trang chính: [omi.me](https://omi.me/)
- Tải xuống: [omi.me/download](https://omi.me/download)
- Tài liệu: [docs.omi.me](https://docs.omi.me/)
- Trò chuyện cộng đồng: [discord.omi.me](http://discord.omi.me)
- Theo dõi cập nhật: [x.com/kodjima33](https://x.com/kodjima33)
- Bộ phần cứng/dev kit:
  - [Buy omi Dev Kit](https://www.omi.me/products/omi-dev-kit-2)
  - [Buy Omi Glass Dev Kit](https://www.omi.me/glass)

## Giấy phép

Omi được phát hành theo <a href="https://github.com/BasedHardware/omi/blob/main/LICENSE">MIT License</a>
