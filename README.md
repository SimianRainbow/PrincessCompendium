# Princess Compendium 👑

A library of princess-themed mini-games for Jet, built for touch-first 2–4 year olds.

## How it works

```
GitHub repo  →  GitHub Pages (hosts HTML games + games.json)  →  Android app (WebView shell)
```

Each game is a self-contained HTML file. Adding a new game to the repo is the only thing needed — the app picks it up automatically via `games.json`.

---

## Setup (one-time)

### 1. Create the GitHub repo

1. Go to GitHub and create a public repo named **`princess-compendium`**
2. Push this folder to it:
   ```
   cd PrincessCompendium
   git init
   git remote add origin https://github.com/YOUR_USERNAME/princess-compendium.git
   git add .
   git commit -m "initial commit"
   git push -u origin main
   ```

### 2. Enable GitHub Pages

1. Go to repo Settings → Pages
2. Source: **Deploy from a branch**, branch: `main`, folder: `/ (root)`
3. Your games will be live at: `https://YOUR_USERNAME.github.io/princess-compendium/`

### 3. Update the URL in two places

Replace `YOUR_USERNAME` in:
- `android/app/src/main/assets/lobby.html` (two occurrences)
- `android/app/src/main/java/com/princesscompendium/MainActivity.kt` (BASE_URL)

### 4. Build and install the Android app

1. Open `android/` in Android Studio (Arctic Fox or newer)
2. Wait for Gradle sync
3. Connect a phone or tablet with USB debugging on
4. Run → or build a debug APK and sideload it

---

## Adding a new game

1. Create a folder under `games/` (e.g. `games/003-animal-sounds/`)
2. Add `index.html` (the game) and `manifest.json`:
   ```json
   {
     "id": "003-animal-sounds",
     "title": "Animal Friends",
     "description": "Tap the animal that matches the sound",
     "icon": "🦄",
     "ageMin": 2,
     "ageMax": 4,
     "skill": "animal recognition",
     "version": "1.0.0"
   }
   ```
3. Push to `main` — GitHub Actions rebuilds `games.json` automatically
4. The app shows the new game on next launch (no APK update needed)

---

## Game design rules for 2–3 year olds

- **No reading required** — icons, colours, and emoji only
- **Giant touch targets** — minimum 100×100px
- **Immediate feedback** — sound + animation within 100ms of tap
- **Short loops** — max 6 rounds, each under 20 seconds
- **Big celebration** — confetti + stars at the end of every round
- **Difficulty progression** — start easy (3 options), add more later
- **Audio** — use the Web Audio API tone helpers already in the games

---

## Current games

| # | Title | Skill |
|---|-------|-------|
| 001 | Magic Gems 💎 | Colour recognition |
| 002 | Counting Crowns 👑 | Counting 1–5 |

## Planned games

- Animal Friends 🦄 — animal recognition / sounds
- Shape Castle 🏰 — shape sorting
- Princess Says 🎀 — following instructions (Simon Says)
- Fairy Tale Tap 📖 — interactive story with choices
