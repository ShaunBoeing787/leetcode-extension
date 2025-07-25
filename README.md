# 🧠 DebugMate - LeetCode Hint Chrome Extension

> 🔧 Built by Shaunak & Ritwik  
> 📅 Progress log: **July 25, 2025**

---

## 🚀 Overview

**DebugMate** is a Chrome Extension that provides intelligent, AI-generated hints for LeetCode problems using Google's **Gemini API**. It enhances your coding journey with point-wise hints, smart UI, and problem detection.

---

## ✅ Features Implemented (Day 1)

### 🎯 LeetCode AI Hint System
- Detects if the user is on a LeetCode problem page.
- Fetches the question slug from URL.
- Queries LeetCode's GraphQL API to retrieve full problem data.
- Sends formatted prompt to **Gemini 2.5 Flash API** to generate **three-point hints**.
- Displays hints dynamically via popup.

### 🧩 Popup UI
- Fully functional `popup.html` in dark mode.
- Gradient "💡 Get Hint" button.
- Separate sections for:
  - ✅ Problem Pages
  - ⚠️ Non-Problem Pages (with image and message)

### 🔽 Collapsible Hint Display
- Hints are shown in expandable dropdowns:
  - `Hint 1`
  - `Hint 2`
  - `Hint 3`
- Uses `##` markers to split Gemini response cleanly.

### 🖼️ Assets and Icons
- Extension icon added: `assets/icon48.jpg`
- Image for non-problem page warning.
- Icons configured via `manifest.json`.

### 🛠️ Bug Fixes / Improvements
- Fixed malformed `manifest.json` errors.
- Centered image inside popup view.
- Added border-radius to give popup rounded edges.
- Troubleshot VS Code Git commit loading issue.

---

## 📁 Project Structure

<pre> 📁 debugmate/ ├── 📁 assets/ │ ├── icon48.jpg │ └── not-found.png ├── 📁 src/ │ ├── background.js │ ├── leetcodeContent.js │ └── 📁 ui/ │ ├── popup.html │ └── popup.js ├── manifest.json └── README.md </pre>


---

## 🧠 Feature Ideas (Coming Soon)

- ✨ “Explain Solution” using Gemini
- ♻️ Regenerate hints with different tones
- 📚 Save and mark problems as "solved"
- 🏷️ Show topic tags and difficulty badges
- 📝 Notes section for each problem
- 📤 Export hints/notes to Notion or PDF
- ⚙️ Inject starter code templates (C++, Java, Python)

---

## 💡 Usage

1. Clone the repo
2. Load the extension in Chrome via `chrome://extensions`
3. Enable Developer Mode → Load Unpacked → Select project folder
4. Navigate to any [LeetCode problem](https://leetcode.com/problems/)
5. Click extension icon → "💡 Get Hint"

---

## 📌 Note

Make sure to add your own **Gemini API key** in `leetcodeContent.js`:

```js
const apiKey = "YOUR_API_KEY_HERE";



Let me know if you'd like:
- GitHub badges (like “Built with Gemini”, “Made with ❤️ by Students”)
- A LICENSE file
- A preview screenshot section

Happy shipping, Shaunak 🚀
