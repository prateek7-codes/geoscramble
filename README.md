# GeoScramble — Country Unscramble Game

A clean, minimal word game where players unscramble jumbled country names.
Built with vanilla HTML/CSS/JS — zero dependencies, instant load.

## Stack
- Pure HTML + CSS + JavaScript (no framework)
- Single file: `index.html`
- Ready for static hosting (Vercel, Netlify, GitHub Pages)

---

## 🚀 Deploy to Vercel (from Replit)

### Step 1 — Replit Setup
1. Create a new Replit → choose **"Import from GitHub"** or **"HTML/CSS/JS"** template
2. Replace the default `index.html` with the contents of `index.html` from this project
3. Click **Run** to preview in Replit

### Step 2 — Push to GitHub
In the Replit Shell:
```bash
git init
git add .
git commit -m "Initial commit: GeoScramble game"
git remote add origin https://github.com/YOUR_USERNAME/geoscramble.git
git push -u origin main
```

### Step 3 — Deploy to Vercel
1. Go to [vercel.com](https://vercel.com) → New Project
2. Import your GitHub repo
3. Framework Preset: **Other** (it's a static site)
4. Build & Output settings: leave blank (root `index.html` is served directly)
5. Click **Deploy** ✅

---

## Game Features
- 80+ countries in the pool
- 10 random rounds per game
- ✅ Green tick for correct answers
- ❌ Red tick + shake animation for wrong answers
- Streak counter & score tracker
- Skip button
- Summary screen with performance rating
- Keyboard-friendly (Enter to submit)

---

## Customisation

### Add more countries
Edit the `COUNTRIES` array in `index.html`:
```js
const COUNTRIES = [
  "FRANCE", "JAPAN", "BRAZIL", // add more here
];
```

### Change number of rounds
```js
rounds = pickRound(10); // change 10 to any number
```

### Change colour scheme
Edit CSS variables at the top of the `<style>` block:
```css
:root {
  --accent: #c8f560; /* change accent colour */
  --bg: #0a0a0f;     /* change background */
}
```
