# 📰 Ink HN: AI-Powered Hacker News Reader

A minimalist, paper-styled web reader for Hacker News, enhanced with Google Gemini AI for content summaries and explanations.

![App Preview](preview.png)

## ✨ Features

- **Paper-like UI**: A clean, distraction-free interface designed for comfortable reading (`Kumbh Sans` font & warm colors).
- **🤖 AI Integration (Gemini)**:
  - **Summarize**: Get a structured Markdown summary of any article instantly.
  - **Explain Like I'm 5**: Get a simple explanation of complex tech topics.
  - **Auto-Translation**: Automatically translates technical titles to English (or your preferred language) using AI context.
- **Smart Tracking**: 
  - Visual indicators (dots) for unread stories.
  - Auto-marks stories as read when you expand them or click the link.
- **Local Storage**: Saves your feed and read status locally in your browser. No login required.
- **Responsive**: Works perfectly on desktop and mobile devices.

## 🚀 How to Use

1. **Clone or Download** this repository.
2. **Get an API Key**: You need a Google Gemini API Key. Get one for free at [Google AI Studio](https://aistudio.google.com/).
3. **Configure**:
   - Open `index.html` in any text editor (Notepad, VS Code, TextEdit).
   - Locate this line (around line 300):
     ```javascript
     const GEMINI_API_KEY = 'INSERT_YOUR_KEY_HERE';
     ```
   - Replace `'INSERT_YOUR_KEY_HERE'` with your actual API Key.
4. **Run**:
   - Simply double-click `index.html` to open it in your browser.
   - Enjoy reading!

> **⚠️ Security Note:** Never commit your actual API Key to GitHub. If you plan to modify and push this code, keep the key placeholder in the version control and only add your real key locally.

## 🛠️ Tech Stack

- **Frontend**: Vanilla HTML5, CSS3, JavaScript (ES6+). No build tools or frameworks required.
- **AI Model**: Google Gemini 3 Flash (via direct API calls).
- **Data Source**: Official Hacker News API (Firebase).
- **Content Extraction**: Uses `Jina.ai` and `Codetabs` proxies to fetch article text for the AI analysis.
- **Markdown Parsing**: `marked.js` library.

## 📄 License

This project is open source and available under the [MIT License](LICENSE).