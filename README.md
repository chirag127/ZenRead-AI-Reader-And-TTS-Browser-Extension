
# 📘 Zen Reader – Distraction-Free Reader Mode with AI Text-to-Speech

Zen Reader is a privacy-first browser extension that transforms cluttered web pages into clean, distraction-free reading experiences with powerful built-in text-to-speech and **AI-powered content extraction using Google Gemini**. It works across Chrome, Edge, Firefox, and all modern browsers supporting Manifest V3.

![Zen Reader Banner](extension/icons/icon128.png)

---

## ✨ Description

Zen Reader removes ads, sidebars, popups, and visual clutter from web pages so you can focus purely on the content that matters.

It uses **Google Gemini AI (client-side via API)** to extract high-quality readable content when available, and automatically falls back to **Mozilla Readability.js** for offline use. The extension also features a rich **text-to-speech system** with word highlighting, adjustable speed, and customizable voices.

Zen Reader is built with a **privacy-first architecture**:
- ✅ No backend servers  
- ✅ No databases  
- ✅ No user tracking  
- ✅ User-controlled AI API key  
- ✅ Offline fallback supported  

---

## 🚀 Live Demo

https://chirag127.github.io/Zen-Reader-Browser-Extension/

---

## 🛠️ Tech Stack / Tools Used

### Frontend (100% Client-Side)

- HTML5, CSS3, JavaScript (Vanilla)
- Chrome Extension API
- Firefox WebExtension API
- Manifest V3
- Google Gemini API (client-side)
- Mozilla Readability.js (offline fallback)
- Web Speech API (native Text-to-Speech)
- IndexedDB / Browser Storage APIs (local preferences)

✅ No Node.js  
✅ No Express  
✅ No servers  
✅ No databases  

---

## 🧪 Features

- **AI-Powered Content Extraction** using Google Gemini  
- **Offline Fallback Extraction** using Mozilla Readability.js  
- **Clean Reader UI** with only the article title, text, and images  
- **Light & Dark Mode**  
- **Font Customization** (family & size)  
- **Preserved Page Links**  
- **Instant Toggle** back to original webpage  
- **Text-to-Speech with Word Highlighting**  
- **Adjustable Reading Speed** (0.5×–4×)  
- **Floating Playback Controls**  
- **Read from Any Text Selection**  
- **Right-Click Context Menu Support**  
- **Smart Auto-Scrolling While Reading**  
- **Customizable Voice & Pitch**  
- **Local Settings Storage**  
- **Zero Telemetry & Zero Tracking**

---

## 🔑 Gemini API Setup (Required for AI Extraction)

Zen Reader uses **Google Gemini directly from your browser**.

### Steps:

1. Go to **Google AI Studio**
2. Create a **Gemini API Key**
3. Open the **Zen Reader Settings Panel**
4. Paste your API key into **Gemini API Key**
5. Save settings

✅ The API key is stored **only in your browser storage**  
✅ The key is **never sent to any server you control**  
✅ All Gemini requests are made **directly from your browser to Google**

If no API key is provided or if the user is offline, Zen Reader automatically switches to **Readability.js**.

---

## 💾 Installation Instructions

### ✅ Chrome / Edge

1. Clone or download this repository  
2. Open:
```

chrome://extensions/

```
or
```

edge://extensions/

```
3. Enable **Developer Mode**
4. Click **Load Unpacked**
5. Select the `extension` folder
6. Zen Reader will appear in your browser toolbar

---

### ✅ Firefox

1. Clone or download this repository  
2. Open:
```

about:debugging#/runtime/this-firefox

```
3. Click **Load Temporary Add-on**
4. Select any file inside the `extension` directory
5. Zen Reader will be activated

---

## 🔧 Usage

### ✅ Basic Reader Mode

1. Open any article or blog page  
2. Click the **Zen Reader icon** in your browser toolbar  
3. Zen Reader will:
- First try **Gemini AI extraction**
- If unavailable → auto-fallback to **Readability.js**
4. The page transforms into a clean reading layout  
5. Use the controls to:
- Toggle Light/Dark mode  
- Change font size & family  
- Return to the original page  

---

### 🔊 Text-to-Speech Usage

1. Click the **speaker icon** in the Zen Reader controls  
2. Control playback with:
- Play / Pause  
- Stop  
- Speed (0.5×–4×)  
- Voice selection  
- Pitch control  
3. You can also:
- Select any text  
- Right-click  
- Choose **Read Selection Aloud**

---

## 🧠 How Zen Reader Works (Hybrid AI + Offline)

1. The page DOM is captured locally
2. If online and API key exists:
- Content is sent to **Gemini for intelligent extraction**
3. If offline or API key missing:
- **Mozilla Readability.js** extracts the content locally
4. Clean text is rendered inside Zen Reader
5. Text-to-Speech runs using the **native browser voice engine**

This ensures:
- ✅ Best-quality extraction with AI
- ✅ Offline reliability
- ✅ Zero backend dependency
- ✅ Full privacy control

---

## 📂 Project Structure

```

extension/
├── icons/                   # Extension icons
├── reader/                  # Reader Mode UI
│   ├── reader.html          # Reader layout
│   ├── reader.css           # Reader styles
│   └── reader.js            # Reader logic
├── background.js            # Extension runtime
├── content.js               # Page capture & fallback extraction
├── extension.js             # Shared helper utilities
├── manifest.json            # Manifest V3 config
├── popup.html               # Popup UI
└── popup.js                 # Popup logic

```

---

## 🔐 Privacy & Security

- ✅ No backend servers  
- ✅ No telemetry  
- ✅ No tracking  
- ✅ No databases  
- ✅ API key stored only locally  
- ✅ No third-party analytics  
- ✅ Optional offline mode  
- ✅ User maintains full control

---

## 📜 License

MIT License

---

## 🌟 Vision

Zen Reader exists to restore peace to the modern web.  
No noise. No clutter. Just content.

AI-powered when you want it.  
Offline-friendly when you need it.  
Private always.

---

## ⭐ Support the Project

If Zen Reader improves your daily reading experience, please consider giving the project a ⭐ on GitHub. Your support helps the project grow and stay maintained.
