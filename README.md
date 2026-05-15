<div align="center">

![CaptchaSonic Banner](https://github.com/user-attachments/assets/d6db3efe-5deb-43b3-be0b-2e74d2c1fc6e)

# CaptchaSonic — AI-Powered CAPTCHA Solver

### Browser Extension · RPA Integration · Web Unlocker

[![Version](https://img.shields.io/badge/version-v0.3.1-blue?style=for-the-badge)](https://github.com/Captcha-Sonic/CaptchaSonic-Extension/releases)
[![License: MIT](https://img.shields.io/badge/license-MIT-green?style=for-the-badge)](LICENSE)
[![Chrome](https://img.shields.io/badge/Chrome-Extension-4285F4?style=for-the-badge&logo=googlechrome&logoColor=white)](https://github.com/Captcha-Sonic/CaptchaSonic-Extension/releases)
[![Firefox](https://img.shields.io/badge/Firefox-Add--on-FF7139?style=for-the-badge&logo=firefoxbrowser&logoColor=white)](https://github.com/Captcha-Sonic/CaptchaSonic-Extension/releases)
[![Edge](https://img.shields.io/badge/Edge-Extension-0078D7?style=for-the-badge&logo=microsoftedge&logoColor=white)](https://github.com/Captcha-Sonic/CaptchaSonic-Extension/releases)

**Automatically solve CAPTCHAs using cutting-edge AI — no manual intervention needed.**

[📥 Download v0.3.1](https://github.com/Captcha-Sonic/CaptchaSonic-Extension/releases) · [🌐 Website](https://captchasonic.com) · [📊 Dashboard](https://my.captchasonic.com) · [💬 Discord](https://discord.captchasonic.com) · [✈️ Telegram](https://telegram.captchasonic.com)

</div>

---

## 🚀 What's New in v0.3.1

- 🔧 Improved **Geetest v4 Slide** solve accuracy with human-like drag simulation
- 🛡️ Enhanced **reCAPTCHA** detection reliability
- 🎯 Added **Binance CAPTCHA** solver support
- ⚡ Faster background task resolution and reduced latency
- 🐛 Bug fixes across content scripts and proxy handling
- 🌍 Multi-browser build pipeline (Chrome MV3, Firefox MV2, Edge MV3)

---

## ✅ Supported CAPTCHA Types

| CAPTCHA Type | Status | Notes |
|:---|:---:|:---|
| **PopularCaptcha** (Image / Grid / BBox / Multi) | ✅ Supported | Full challenge-type coverage |
| **reCAPTCHA v2** (Visible & Invisible) | ✅ Supported | Checkbox + image challenges |
| **reCAPTCHA v3** | ✅ Supported | Score-based token generation |
| **AWS WAF CAPTCHA** | ✅ Supported | Puzzle-based challenges |
| **Geetest v3** (Slide / Click) | ✅ Supported | Multiple challenge modes |
| **Geetest v4** (Slide) | ✅ Supported | Adaptive slide solving |
| **BLS OCR / Text CAPTCHA** | ✅ Supported | Optical character recognition |
| **mtCaptcha** | ✅ Supported | Interactive widget solving |
| **CaptchaFox** | ✅ Supported | Widget auto-solve |
| **Tencent CAPTCHA** | ✅ Supported | Slide & puzzle challenges |
| **TikTok CAPTCHA** | ✅ Supported | Slide, circle, and click types |
| **Prosopo / Procaptcha** | ✅ Supported | PoW-based challenges |
| **Binance CAPTCHA** | ✅ Supported | Custom puzzle challenges |
| **Universal OCR** | 🔜 Coming Soon | General-purpose text recognition |

---

## ⚡ Key Features

- **🤖 AI-Powered Solving** — Leverages advanced AI models for high-accuracy CAPTCHA resolution
- **🔌 Zero-Config Integration** — Works automatically on any website with supported CAPTCHAs
- **🌐 Multi-Browser Support** — Chrome, Firefox, Edge, Brave, and all Chromium-based browsers
- **📱 Mobile Compatible** — Touch event simulation for mobile browser environments
- **⚙️ Custom API Endpoint** — Connect your own solving infrastructure via settings
- **🔐 Integrity Verification** — Built-in WASM-based request signing for tamper-proof communication
- **🎨 Theming Support** — Light & dark mode with customizable popup UI
- **📊 Analytics Dashboard** — Track solve rates, usage, and performance at [my.captchasonic.com](https://my.captchasonic.com)
- **🧩 Proxy Management** — Built-in proxy support with health checking and rotation
- **🔄 Auto-Retry Logic** — Smart retry with countdown notifications on transient failures

---

## 📥 Installation

### Download from Releases (Recommended)

1. Download the latest release for your browser from the [Releases Page](https://github.com/Captcha-Sonic/CaptchaSonic-Extension/releases).
2. Follow the guide for your browser:
   - 🟢 **Chrome / Brave / Edge:** [Chrome Installation Guide](https://github.com/Captcha-Sonic/CaptchaSonic-Extension/blob/main/how_to_Install_Zip_Chrome_Extension_Guide.md)
   - 🟠 **Firefox:** [Firefox Installation Guide](https://github.com/Captcha-Sonic/CaptchaSonic-Extension/blob/main/how_to_Install_Zip_Chrome_Extension_Guide.md#loading-extensions-in-mozilla-firefox)


#### Build Targets

| Command | Browser | Manifest |
|:---|:---|:---|
| `bun run build:chrome` | Chrome / Brave / Edge | MV3 |
| `bun run build:firefox` | Firefox | MV2 |
| `bun run build:edge` | Edge | MV3 |
| `bun run build:all` | All browsers | — |

---

## ⚡ How to Use

1. **Install** the CaptchaSonic extension in your browser.
2. **Visit** any webpage with a supported CAPTCHA challenge.
3. **Relax** — CaptchaSonic detects and solves the CAPTCHA automatically.

> No manual clicking, no tokens to copy — it just works.

---

## 🏗️ Architecture

```
captchasonic-extension/
├── entrypoints/           # Content scripts for each CAPTCHA type
│   ├── background.js      # Service worker (task routing, API calls)
│   ├── popup/             # Extension popup UI (SolidJS + Tailwind)
│   ├── options/           # Settings page
│   └── *.content.js       # Per-CAPTCHA detection & solving logic
├── src/
│   ├── tools.js           # Shared utilities (DOM, canvas, drag simulation)
│   ├── integrity.js       # WASM-based request signing
│   └── proto/             # Protobuf definitions
├── public/
│   ├── icons/             # Extension icons
│   ├── _locales/          # i18n strings
```

**Tech Stack:** WXT Framework · SolidJS · Tailwind CSS v4 · AssemblyScript / WASM · Protobuf

---

## 🔗 Links

| Resource | URL |
|:---|:---|
| 🌐 Homepage | [captchasonic.com](https://captchasonic.com) |
| 📊 Dashboard & Pricing | [my.captchasonic.com](https://my.captchasonic.com) |
| 💬 Discord Community | [discord.captchasonic.com](https://discord.captchasonic.com) |
| ✈️ Telegram | [telegram.captchasonic.com](https://telegram.captchasonic.com) |
| 📥 Releases | [GitHub Releases](https://github.com/Captcha-Sonic/CaptchaSonic-Extension/releases) |

---

## 💡 FAQ

<details>
<summary><strong>Is CaptchaSonic free to use?</strong></summary>

CaptchaSonic offers free usage during the beta period. Paid plans with affordable pricing will be available after the beta ends.
</details>

<details>
<summary><strong>Which browsers are supported?</strong></summary>

Chrome, Firefox, Edge, Brave, Opera, and any Chromium-based browser. The extension ships with MV3 for Chrome/Edge and MV2 for Firefox.
</details>

<details>
<summary><strong>How accurate is the CAPTCHA solving?</strong></summary>

CaptchaSonic uses advanced AI vision models to achieve high solve rates. Accuracy varies by CAPTCHA type — hCaptcha and reCAPTCHA typically see 90%+ success rates.
</details>

<details>
<summary><strong>Can I use my own API endpoint?</strong></summary>

Yes. Go to the extension settings and configure a custom API endpoint to route solve requests through your own infrastructure.
</details>

<details>
<summary><strong>Does it work with proxies?</strong></summary>

Yes. CaptchaSonic includes a built-in proxy manager with health checking, rotation, and support for HTTP/HTTPS/SOCKS5 protocols.
</details>

<details>
<summary><strong>Can I suggest new CAPTCHA types or features?</strong></summary>

Absolutely! Open an issue in this repository or reach out on [Discord](https://discord.captchasonic.com) or [Telegram](https://telegram.captchasonic.com).
</details>

---

## 🧑‍💻 Contributing

We welcome contributions! To get started:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/my-feature`)
3. Commit your changes (`git commit -m 'feat: add my feature'`)
4. Push to the branch (`git push origin feature/my-feature`)
5. Open a Pull Request

Please follow our [Contribution Guidelines](CONTRIBUTING.md) and ensure all builds pass before submitting.

---

## 📄 License

CaptchaSonic is licensed under the **MIT License**. See the [LICENSE](LICENSE) file for details.

---

<div align="center">

![CaptchaSonic](https://github.com/user-attachments/assets/1b82f378-38bc-40a4-a843-4e30e512b4b9)

### ⚡ Try CaptchaSonic today — free AI CAPTCHA solving, zero hassle.

[Download v0.3.1](https://github.com/Captcha-Sonic/CaptchaSonic-Extension/releases) · [Get Started](https://captchasonic.com)

</div>
