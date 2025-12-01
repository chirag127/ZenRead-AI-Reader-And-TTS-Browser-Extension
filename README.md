
# 📘 Zen Reader – Distraction-Free Reader Mode with Text-to-Speech

A lightweight, privacy-friendly browser extension that transforms any cluttered webpage into a clean, distraction-free reading experience with powerful text-to-speech support. Zen Reader works across Chrome, Edge, Firefox, and all modern browsers supporting Manifest V3.

![Zen Reader Banner](extension/icons/icon128.png)

---

## ✨ Description

Zen Reader is a browser extension designed to strip away ads, sidebars, popups, and visual noise from web pages—so you can focus purely on the content that matters.

It also features an advanced **text-to-speech system** with word highlighting, adjustable speed, and customizable voices, making web content more accessible, productive, and comfortable to consume.

Zen Reader combines **AI-powered content extraction**, a beautiful reading interface, and **offline fallback mechanisms** to ensure consistent performance across all websites.

---

## 🚀 Live Demo

Visit the official demo site:

https://chirag127.github.io/Zen-Reader-Browser-Extension/

---

## 🛠️ Tech Stack / Tools Used

### Frontend (Browser Extension)

- HTML5, CSS3, JavaScript (Vanilla)
- Chrome Extension API
- Firefox WebExtension API
- Manifest V3
- Mozilla Readability.js (fallback extraction)
- Web Speech API (Text-to-Speech)

### Backend (Optional AI Extraction)

- Node.js
- Express.js
- Google Generative AI API (Gemini 2.0 Flash Lite)
- CORS for secure cross-origin requests

---

## 🧪 Features

- **AI-Powered Content Extraction** using Gemini 2.0 Flash Lite  
- **Clean Reader UI** showing only the article title, text, and images  
- **Light & Dark Mode** for comfortable reading  
- **Font Customization** (family and size controls)  
- **Preserved Page Links** for in-article navigation  
- **Instant Toggle** between Original View and Reader View  
- **Text-to-Speech with Word Highlighting**  
- **Adjustable Reading Speed** (0.5× to 4×)  
- **Floating Playback Controls** (Play, Pause, Stop)  
- **Read from Any Selection**  
- **Right-Click Context Menu Support** for instant reading  
- **Smart Auto-Scrolling** while reading  
- **Customizable Voice & Pitch**  
- **Offline Fallback** using Readability.js when AI is unavailable  

---

## 💾 Installation Instructions

### 🔧 Backend Setup (For AI Extraction)

1. Navigate to the backend directory:
```

cd backend

```
2. Install dependencies:
```

npm install

```
3. Create environment variables:
```

cp .env.example .env

```
4. Add your Gemini API key:
```

GEMINI_API_KEY=your_api_key_here

```
5. Start the backend server:
```

npm start

```

---

### 🌐 Extension Setup

#### ✅ Chrome / Edge

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

#### ✅ Firefox

1. Clone or download this repository  
2. Open:
```

about:debugging#/runtime/this-firefox

```
3. Click **Load Temporary Add-on**
4. Select any file inside the `extension` directory
5. Zen Reader will be activated

---

### ⚙️ Configuration

To change:
- Backend API URL  
- Toggle Gemini AI extraction  

Update the following file:
```

extension/config.js

```

---

## 🔧 Usage

### ✅ Basic Reader Mode

1. Open any article or blog page  
2. Click the **Zen Reader icon** in your browser toolbar  
3. The page instantly transforms into a clean reading layout  
4. Use the control bar to:
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

## 🧠 How Zen Reader Works

Zen Reader uses the **Gemini 2.0 Flash Lite AI model** to intelligently extract the most relevant content from any webpage.

When AI extraction is unavailable:
- The extension automatically falls back to **Mozilla Readability.js**, ensuring Zen Reader works even **offline**.

This dual-layer design guarantees:
- High-quality extraction
- Maximum compatibility
- Zero website dependency

---

## 📸 Screenshots

![Zen Reader Light Theme](https://via.placeholder.com/800x450.png?text=Zen+Reader+Light+Theme)
![Zen Reader Dark Theme](https://via.placeholder.com/800x450.png?text=Zen+Reader+Dark+Theme)
![Zen Reader Text-to-Speech](https://via.placeholder.com/800x450.png?text=Zen+Reader+Text-to-Speech)

---

## 💻 Development

### 📁 Project Structure

```

extension/
├── icons/                   # Extension icons
├── reader/                  # Reader Mode UI
│   ├── reader.html          # Reader layout
│   ├── reader.css           # Reader styles
│   └── reader.js            # Reader logic
├── background.js            # Extension background runtime
├── content.js               # Content extraction logic
├── extension.js             # Shared helper utilities
├── manifest.json            # Manifest V3 config
├── popup.html               # Popup UI
└── popup.js                 # Popup logic

```

---

### 🧩 Key Components

1. **Background Script** – Coordinates extension state and messaging  
2. **Content Script** – Extracts readable content from web pages  
3. **Reader UI** – Displays distraction-free reading layout  
4. **Popup UI** – Control panel to activate Zen Reader  
5. **Helpers** – Shared utility logic  

---

## 🧪 Testing

1. Open:
```

test/test_article.html

```
2. Click the Zen Reader icon  
3. Verify:
- Content extraction
- Theme switching
- Text-to-Speech playback  
- Selection-based reading  

---

## 📜 License

MIT License

---

## 🌟 Vision

Zen Reader exists to restore peace to the modern web.  
No noise. No clutter. Just content.

Whether you’re reading articles, documentation, blogs, or long research papers—Zen Reader transforms the web into a calm, focused reading environment.

---

## ⭐ Support the Project

If Zen Reader improves your reading experience, please consider giving the project a ⭐ on GitHub. Your support helps the project grow and evolve.
