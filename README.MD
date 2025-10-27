<a alt="Whats Link+: WA Easy Direct Message and QR Code">
<img src="https://github.com/Machina-Labs-Agency/Whats-Link-Plus/blob/f16c16cc4f949704eea20c805ebe7ec87fa8663c/Assets/Main-banner-PT-BR.png">
</a>

<h1 align="center">Whats Link+: WA Easy Direct Message and QR Code</h1>

<h6 align="center">Whats Link+ is a lightweight and user-friendly Chrome extension that makes it easy to send WhatsApp messages and generate shareable links directly from your browser.</h6>

<p align="center">
  <img src="https://img.shields.io/badge/License-MIT-yellow.svg">  <img src="https://img.shields.io/badge/Made%20with-JavaScript-blue">  <img src="https://img.shields.io/badge/Platform-Chromium%20Extension-green">
</p>

---

## Features

* **Context Menu Integration:** Right-click on any selected phone number on a webpage to instantly open a chat.
* **Dynamic All-in-One Popup:**
    * Starts in a **clean, compact view** for quickly sending messages.
    * Click **"Link & QR Code Generator"** to smoothly expand the UI, revealing powerful tools for creating shareable links and QR codes without cluttering the main view.
    * Choose to open chats with the **Desktop/Mobile App** or with **WhatsApp Web**.
    * Save your preferred country code and "Open with" choice as defaults.
* **Link & QR Code Generator:**
    * Create shareable links for `api.whatsapp.com` or `web.whatsapp.com`.
    * Add optional pre-filled text to your links.
    * Instantly generate a scannable QR code.
    * **Download** the QR code as a PNG file or **Share** it using your device's native sharing menu.
* **Smart Country Code Detection:** Automatically recognizes phone numbers from the US and Brazil.
* **Recent Numbers:** Automatically saves your last 5 used numbers for quick access in a scrollable list.
* **Multi-Language Support:** Automatically displays in English or Brazilian Portuguese (`pt-BR`) based on your browser's language setting.


---

## Installation Guide

1.  **Download:** Download all the extension files into a single folder on your computer.
2.  **Open Chrome Extensions:** Open Google Chrome and navigate to `chrome://extensions`.
3.  **Enable Developer Mode:** Turn on the "Developer mode" toggle in the top-right corner.
4.  **Load Unpacked:** Click the "Load unpacked" button and select the folder where you saved the extension files.
5.  The extension icon will now appear in your browser's toolbar.

---

## Getting Started Instructions

### Quick Message
1. Click the extension icon in the toolbar
2. Select "Quick Message" from the side navigation
3. Enter or select a phone number (country code vertically aligned)
4. Click "Send Message"
- Receive visual feedback within the view itself if there are errors

### Link & QR Code Generator
1. Select "Link Generator" from the side navigation
2. Enter the phone number and optional message (fields vertically aligned)
3. Click "Generate Link & QR Code"
4. Copy the link, download the QR code, or share directly
- Notifications appear within the view

### Saving Your Preferences

1.  In the popup, select your desired default country code from the dropdown.
2.  Choose your preferred "Open with" method (App or Web).
3.  Click the **"Save Defaults"** button.
4.  All future sessions and context-menu actions will now use these settings.

---

### Technologies
- Manifest V3: Current Chrome extensions standard
- Vanilla JavaScript (ES6+): No external frameworks
- QRCode.js: QR code generation
- Chrome Storage API: Data persistence

---

## License

This project is licensed under the APACHE [License](LICENSE).

---

## Privacy
This extension:
- Does not collect personal data
- Only stores settings and history locally
- Does not perform tracking or show ads
- Works completely offline (except for opening WhatsApp)

---

## Disclaimer

This is an independent project and is not officially affiliated with WhatsApp or Meta. Please read the full [Legal Disclaimer](DISCLAIMER.md).
WhatsApp™ is a trademark of WhatsApp Inc., registered in the U.S. and other countries. This extension has no relationship to WhatsApp™ or WhatsApp Inc.
