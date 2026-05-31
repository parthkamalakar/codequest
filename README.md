# 🪐 CodeQuest AI

> *Seeking the optimal path from beginner to expert coder.*

CodeQuest AI is a state-of-the-art, gamified coding platform designed with a premium space-eclipse dark aesthetic. Operating as a fully unified **Single-Page Application (SPA)**, it provides users with sandboxed code execution, interactive unit testing, and real-time AI mentoring right inside the browser.

---

## ✨ Features

- **3D Solar Eclipse & Navigation**: Centered glossy solar orb modeled with realistic radial light highlights, surrounded by a spinning corona glow and tracking an interactive downward scroll toggle.
- **Smooth Custom Cursor (Linear Interpolation)**: A glowing white circular cursor tracks the mouse coordinate with organic fluid lag (using lerp). It automatically scales and adapts its glowing border colors (purple, cyan, or amber) based on hoverable actions, and hides completely inside the Monaco workspace.
- **Interactive Monaco Workspace**: A high-fidelity code editor instance (the core engine powering VS Code) loaded via CDN, configured with a custom, tailored cosmic dark theme (`space-dark`), syntax highlighting, smooth blink cursors, and responsive layouts.
- **Zero-Server Sandboxed Runner**: Safely intercept and evaluate JavaScript in-browser inside sandbox scopes, outputting beautiful color-coded logs to the Custom console panel. 
- **Automated Test Vectors**: Visual unit test assertion cards verify solutions in real time. Passing all test criteria unlocks rewards via a rewarding visual overlay, awarding XP and incrementing coding streaks.
- **Local AI Mentor (Chronos)**: An automated navigations AI mentor in the sidebar. Type custom chat strings to ask for optimization paths, edge case analyses, and specific debugging hints.

---

## 🛠️ Technology Stack

- **Markup**: Semantic HTML5 structures
- **Styles**: Custom CSS3 variables, HSL color tokens, backdrop-filter glassmorphism, keyframes, and custom scrollbars.
- **Logic**: Vanilla ES6+ Javascript (Starfield particle generators, linear interpolation physics loop, intercepted console log scopes).
- **Editor**: [Monaco Editor](https://microsoft.github.io/monaco-editor/) mounted via RequireJS loader CDNs.

---

## 🚀 Instant Local Execution (No Server Needed)

CodeQuest has been consolidated into a **single, fully self-contained HTML file**. Because browser security policies (CORS) typically block Monaco Editor's cross-origin web workers when running from a local filesystem (`file://` protocol) due to origin restrictions, the script implements an **inline data-URI web worker proxy** to bypass these locks cleanly.

To run the application:
1. Navigate to the project directory.
2. **Double-click** on **[index.html](file:///Users/pranav/.gemini/antigravity/scratch/codequest/index.html)**.
3. It will launch instantly and operate flawlessly inside your browser!

---

## ☁️ Deploying to Vercel

### Option A: Direct CLI Push (Fastest)
Deploy your local folder straight to Vercel in 15 seconds:
```bash
# Navigate to the folder
cd /Users/pranav/.gemini/antigravity/scratch/codequest

# Run the on-the-fly deploy script
npx vercel
