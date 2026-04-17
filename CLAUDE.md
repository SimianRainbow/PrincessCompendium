# Princess Compendium — Project Context

Built for Jet (toddler, ~2-4 years old). A growing library of princess-themed browser games that live on GitHub Pages and load inside an Android WebView app. No APK update is ever needed — push to `main` and the app picks up new games automatically via `games.json`.

## Architecture

```
games/<id>/index.html   ← each game, fully self-contained
games.json              ← master registry (auto-rebuilt by GitHub Actions on push, OR maintained manually)
lobby.html              ← launcher UI, reads games.json at runtime
android/                ← WebView shell app, points at GitHub Pages URL
```

GitHub Pages URL: `https://simiandainbow.github.io/PrincessCompendium/`

## Mandatory design rules (non-negotiable)

- **Single HTML file** — no external JS/CSS files; inline everything. Google Fonts CDN is fine.
- **No external audio files** — use Web Audio API only (oscillators, gains). Every game already has a `getAudio()` / `playTone()` helper to copy.
- **Tap targets** — minimum 90×90px, ideally 110-130px+. This is a toddler on a phone.
- **No failure states that cause distress** — wrong answers wobble/shake but always let the child try again. No timers that expire and end the game in disappointment.
- **Princess / fairy-tale theme** — crowns, gems, sparkles, castles, unicorns, magic. Pastel palette.
- **Celebratory on every correct answer** — sparkle particles and a pleasant ascending tone minimum. Full confetti + overlay on round completion.
- **Mobile portrait first** — use `clamp()` for all font sizes and dimensions. Test at ~390px wide.
- **No reading required for core gameplay** — emoji and colour carry meaning; text is supplementary.
- **Difficulty must progress** — even simple games should have easy/medium/hard tiers across rounds.

## Game registry (games.json)

Required fields for each entry:

```json
{
  "id": "NNN-slug",
  "title": "Display Title",
  "description": "One sentence — what the child does",
  "icon": "single emoji",
  "ageMin": 2,
  "ageMax": 5,
  "skill": "skill being taught",
  "version": "1.0.0",
  "category": "colours-shapes | numbers | animals | listen | stories | letters | music | adventure | play | other",
  "path": "games/NNN-slug/index.html"
}
```

After any change to a game file, bump its `version` in `games.json` (semver: `1.0.0` → `1.1.0` for improvements, `1.0.0` for new games).

## Current games

| ID | Title | Skill | Version |
|----|-------|-------|---------|
| 001-colour-match | Magic Gems 💎 | colour recognition | 1.0.0 |
| 002-counting-crowns | Counting Crowns 👑 | counting 1-5 / 1-10 | 1.1.0 |
| 003-animal-friends | Animal Friends 🦄 | animal recognition | 1.0.0 |
| 004-shape-castle | Shape Castle 🏰 | shape recognition | 1.0.0 |
| 005-princess-says | Princess Says 🎀 | listening & following instructions | 1.0.0 |
| 006-fairy-tale-tap | Fairy Tale Tap 📖 | story comprehension & choices | 1.0.0 |
| 007-letter-bubbles | Letter Bubbles 🔤 | letter recognition A-Z | 1.0.0 |
| 008-more-or-less | More or Less ⚖️ | number sense & comparing | 1.0.0 |
| 009-star-catcher | Star Catcher ⭐ | focus & reaction | 1.0.0 |
| 010-royal-orchestra | Royal Orchestra 🎵 | music & memory sequences | 1.0.0 |
| 011-princess-quest | Princess Quest 🏰 | 3D adventure & steering | 1.0.0 |
| 012-pattern-princess | Pattern Princess 🌸 | pattern recognition (ABAB/AABB) | 1.0.0 |
| 013-magic-leaf | Magic Leaf 🍃 | 3D flying & steering | 1.0.0 |

## Skills still not covered (priority order)

1. **Sorting by size** — big vs. small, biggest/smallest (pre-maths)
2. **Emotions / feelings** — happy, sad, surprised, angry (social-emotional)
3. **Opposites** — hot/cold, fast/slow, up/down, full/empty
4. **Body parts** — point to nose, ears, hands, etc.
5. **Simple addition** — 1+1, 2+1, tap the answer (ages 4-5)
6. **Spatial concepts** — in, on, under, next to, behind
7. **Rhyming / phonics** — which two words rhyme?
8. **Sorting by category** — foods vs. animals vs. vehicles
9. **Seasons / weather** — match the weather to the scene
10. **Sight words** — tap the word that matches the picture (ages 4-5)

## Git workflow

Always commit and push after any changes:

```bash
git add -A
git commit -m "feat/fix/chore: <what changed>"
git push origin main
```

The next sequential game ID is `014-<slug>`.
