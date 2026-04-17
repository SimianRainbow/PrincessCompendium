# Princess Compendium Update

Your job this run: make two contributions to the Princess Compendium.

1. **Improve one existing game**
2. **Create one brand-new original game**

Read `CLAUDE.md` first for project context, design rules, and the full game registry.
Read `status.md` to see what was done last run, which games are due for improvement, and which skills still need covering.

---

## Step 1 — Pick the game to improve

From `status.md`, choose the game most in need of improvement. Good improvements:
- Difficulty progression (easy → medium → hard rounds) with a visible tier indicator
- Sparkle / particle effects on correct answers
- Richer audio feedback (ascending tones on correct, melody on round win)
- More content variety (more colours, shapes, animals, letters, etc.)
- Fixing any design rule violations (e.g. timers that cause distress)

Read the current `index.html` before writing — understand what's already there, then extend it.

After improving:
- Bump its `version` in `games.json` (e.g. `1.0.0` → `1.1.0`)
- Write the updated `index.html` back to its original path

---

## Step 2 — Create one new game

Pick a skill from the "Skills not yet covered" list in `status.md` (or `CLAUDE.md` if status.md is stale).

Assign it the next sequential ID from `status.md`. Create:
- `games/<new-id>/index.html` — the game (single self-contained HTML file)
- A new entry in `games.json`

Follow all design rules in `CLAUDE.md` strictly.

---

## Step 3 — Verify

1. Confirm both HTML files are well-formed (DOCTYPE, viewport meta, no broken tags).
2. Confirm `games.json` is valid JSON with the version bump and new entry.
3. Confirm the new game folder and file exist on disk.

---

## Step 4 — Update status.md

Update `status.md`:
- Set "Last update run" to today's date and describe what was done
- Add a row to the improvement history table
- Update "Next game ID"
- Remove the newly-covered skill from the "not yet covered" list

---

## Step 5 — Commit and push

```bash
git add -A
git commit -m "feat: improve <game-id> + add <new-game-id>

- <game-id> v<new-version>: <one-line summary of improvement>
- <new-game-id>: new game teaching <skill>"
git push origin main
```

Confirm the push succeeded. If it fails, report the error clearly.

---

## Output

Briefly summarise: which game was improved and what changed, what the new game is and what it teaches, and whether the push succeeded.
