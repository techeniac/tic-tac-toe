# ✏️ Tic Tac Toe — Me vs The TechEniac

[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https%3A%2F%2Fgithub.com%2Fhetvihradadiya%2Ftic-tac-toe)
[![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
[![PWA Ready](https://img.shields.io/badge/PWA-Ready-orange.svg)](manifest.json)

A stylish, hand-drawn notebook doodle-themed Tic Tac Toe game built with pure vanilla HTML, CSS, and JavaScript. Play against **The TechEniac**, an AI bot powered by the Minimax algorithm with alpha-beta pruning and dynamic difficulty balancing.

---

## ✨ Features

- 📝 **Notebook Doodle Aesthetic**: Designed to feel like sketches scribbled in the back of a school notebook — complete with paper texture, ruled lines, washi tape, cute doodles, and coffee ring stains.
- 🤖 **Smart AI Opponent ("The TechEniac")**:
  - Implements the **Minimax algorithm** with alpha-beta pruning.
  - Automatically identifies immediate winning and blocking opportunities.
  - Includes a calibrated randomness factor (~40%) to keep matches fun, dynamic, and winnable.
- 🎨 **Satisfying Visual Feedback**:
  - Ink splatter particles on each turn.
  - Animated strike-through line on winning combinations.
  - Full-screen confetti celebration upon player victory.
  - Screen shake effect when defeated.
  - Snarky, playful dialogue and reactive scoreboard tracking.
- 📱 **Mobile & Touch Optimized**:
  - Responsive layout with viewport-relative units (`dvh`).
  - Fast-response touch tap targets (`touch-action: manipulation`) with zero 300ms delay.
  - Prevention of rubber-band scroll bounce on iOS/Android devices.
- ⏸️ **Pause & Resume Controls**: Pause mid-game anytime via the on-screen button or keyboard shortcuts (`Esc` / `P`) with a dedicated doodle pause modal and restart option.
- ⚡ **Offline-First PWA (Progressive Web App)**:
  - Cache-first service worker (`sw.js`) for instant offline loading.
  - Web App Manifest (`manifest.json`) for installing directly onto desktop or mobile home screens.
- 🚀 **Vercel Deployable**: Includes optimized cache headers for PWA service worker updates and static font delivery via `vercel.json`.

---

## 📁 Project Structure

```text
.
├── index.html          # Main game markup, styles, and game logic
├── logo.svg            # Custom SVG logo and PWA icon
├── manifest.json       # Web App Manifest for PWA installation
├── sw.js               # Service Worker for offline asset caching
├── vercel.json         # Vercel deployment configuration and HTTP headers
├── _headers            # Cloudflare Pages / Netlify fallback headers
├── fonts/              # Custom handwriting font assets
│   ├── fonts.css       # Font face declarations
│   ├── caveat-400.woff2
│   ├── caveat-700.woff2
│   ├── permanent-marker.woff2
│   └── rock-salt.woff2
├── .gitignore          # Ignored editor, OS, and build files
└── README.md           # Project documentation
```

---

## 🚀 Getting Started

### Local Development

No complex build step or package manager is required! You can run the project using any local HTTP server:

#### Option 1: Python HTTP Server
```bash
# Python 3
python3 -m http.server 3000
```
Open [http://localhost:3000](http://localhost:3000) in your browser.

#### Option 2: Node `serve` or `npx`
```bash
npx serve .
```

#### Option 3: VS Code Live Server
Right-click on `index.html` and choose **"Open with Live Server"**.

---

## 🌐 Deploy to Vercel

This repository is ready for one-click deployment to **[Vercel](https://vercel.com)**.

### Via Vercel Dashboard (Recommended)

1. Push your repository to GitHub:
   ```bash
   git push -u origin main
   ```
2. Go to the [Vercel Dashboard](https://vercel.com/new).
3. Import the `hetvihradadiya/tic-tac-toe` repository.
4. Keep the default settings (Framework Preset: **Other**, Root Directory: `./`).
5. Click **Deploy**!

### Via Vercel CLI

```bash
# Install Vercel CLI if you haven't already
npm install -g vercel

# Deploy directly from terminal
vercel
```

---

## 🎮 How to Play

1. Tap or click any empty cell on the 3×3 grid to place your **O** mark in blue ink.
2. The **TechEniac** will analyze the board and place its **X** mark in red ink.
3. Form a straight line horizontally, vertically, or diagonally with three of your marks to win!
4. Click **"again!! ✏️"** to reset the board and start a rematch.

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).
