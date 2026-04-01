# Iron Log — Gym Tracker PWA

A mobile-first progressive web app for logging workouts, tracking PRs, and visualizing progress.

## Features
- Log sets with weight, reps, RPE, and notes
- Personal records detection with PR badges
- Progress charts (max weight over time, volume by exercise)
- 1RM calculator with training percentages
- Full workout history
- Works offline after first load
- Installable on iPhone / Android home screen

## Deploy to GitHub Pages (5 minutes)

### 1. Create the repo
```
git init
git add .
git commit -m "init Iron Log"
gh repo create ironlog --public --push
```
Or create manually on github.com and push.

### 2. Enable GitHub Pages
- Go to your repo → Settings → Pages
- Source: Deploy from branch → `main` → `/ (root)`
- Save

### 3. Add icons (optional but recommended)
Generate icons at https://realfavicongenerator.net using any image.
Drop `icon-192.png` and `icon-512.png` into the repo root.

### 4. Install on your phone

**iPhone (Safari):**
1. Open your GitHub Pages URL in Safari
2. Tap the Share button (box with arrow)
3. Scroll down → "Add to Home Screen"
4. Tap Add — it appears as an app icon

**Android (Chrome):**
1. Open the URL in Chrome
2. Tap the 3-dot menu → "Add to Home Screen"
3. Or Chrome may show an install banner automatically

## Files
- `index.html` — the entire app
- `manifest.json` — PWA metadata (name, colors, icons)
- `sw.js` — service worker (offline caching)
- `icon-192.png` / `icon-512.png` — app icons (add your own)

## Data
All workout data is stored in your browser's localStorage — it stays on your device and never leaves. If you clear your browser data, your logs will be cleared too. For backup, a future "Export CSV" button could be added easily.
