# Princess Compendium — Status

## Last update run
Date: 2026-06-16
- Improved: `011-princess-quest` → v1.1.0 (3 rounds: speed 6 / 5 stars, speed 8.5 / 6 stars, speed 11 / 7 stars; tier badge "🌟 Round X/3" in HUD; inter-round toast with playRoundWin melody; 14-particle CSS sparkle burst on each star collect; Fredoka One font; hair grows across all rounds via totalStars; confetti on round-end)
- Added: `039-princess-puzzle` — "Princess Puzzle" teaching odd-one-out reasoning & categorisation; 9 rounds across 3 tiers (Easy: animals/fruits/royal; Medium: flowers/sea creatures/clothes; Hard: night sky/flying/sweets); 4-emoji 2×2 grid; odd item shuffled to random position each round; sparkle burst + celebrate overlay on correct; wobble on wrong; tier toasts between tiers

## Improvement history

| Date | Game | Change | New version |
|------|------|--------|-------------|
| 2026-04-17 | 002-counting-crowns | 3 difficulty tiers, sparkles, richer audio | 1.1.0 |
| 2026-04-22 | 009-star-catcher | Removed distress timer; target-count tiers + sparkle bursts | 1.1.0 |
| 2026-04-25 | 003-animal-friends | +6 animals, animal sounds, 3 difficulty tiers, sparkles | 1.1.0 |
| 2026-04-28 | 007-letter-bubbles | Tier badge, tap-to-hear phonics tones, sparkle bursts, 12 rounds | 1.1.0 |
| 2026-05-01 | 001-colour-match | 3 tiers, 12 colours (incl. orange/teal/brown/white/grey/navy), sparkles, dynamic grid | 1.1.0 |
| 2026-05-04 | 004-shape-castle | +3 shapes (Oval/Rectangle/Pentagon), 3 tiers, 9 rounds, sparkle bursts | 1.1.0 |
| 2026-05-07 | 010-royal-orchestra | +2 instruments (Flute/Piano), 3 tiers, sparkle bursts, tier badge, round-win melody | 1.1.0 |
| 2026-05-10 | 005-princess-says | 3 tiers, 24-item pool (colours+animals+foods), 2×3 Hard grid, sparkle bursts | 1.1.0 |
| 2026-05-13 | 012-pattern-princess | Fixed pattern logic, ABC+ABBC patterns, 3-item themes, tier badge, 9 rounds | 1.1.0 |
| 2026-05-16 | 008-more-or-less | Tier badge, LESS questions, sparkle burst, 9 rounds, locked state, round counter | 1.1.0 |
| 2026-05-19 | 021-body-parts | Named tier badges, knee added, emoji sparkles, round counter, prompt variety, part reinforcement in celebration | 1.1.0 |
| 2026-05-22 | 019-feelings-faces | Fredoka font, single tier badge, progress bar, locked state, 4-note correct sound, bigger sparkle burst, emotion name in celebration, 28 scenarios | 1.1.0 |
| 2026-05-25 | 020-opposites | Fredoka font, progress bar, colour-coded tier badge, round counter X/18, 18 pairs (was 12), emoji sparkles in burst, pastel BG, tier-change message | 1.1.0 |
| 2026-05-28 | 018-size-sort | Round counter X/Y, emoji sparkles in burst, 25-item pool (was 15), richer tier-transition messages | 1.1.0 |
| 2026-05-31 | 022-magic-adding | Fredoka font, round counter, tier-transition toast, equation in celebrate ("2+3=5!"), 14 sparkles | 1.1.0 |
| 2026-06-01 | 023-spatial-princess | Fredoka font, round counter X/18, tier-transition toast, 2 extra targets + 3 containers, 16 sparkles | 1.1.0 |
| 2026-06-04 | 024-rhyme-time | Fredoka font, round counter X/12, tier-transition toast, 4th pair per tier, shuffled tiers, 16 sparkles | 1.1.0 |
| 2026-06-07 | 006-fairy-tale-tap | Fredoka font, 3 complete stories, Forest path, sparkle on choices, tier badge, story counter, tier toast | 1.1.0 |
| 2026-06-10 | 025-princess-sort | Fredoka font, sparkle 12→16, tier-transition toast, 4-note audio, playTierUp, fixed duplicate pool item | 1.1.0 |
| 2026-06-13 | 013-magic-leaf | 3-tier speed/banana scaling, tier badge, inter-round toast, 14-particle sparkle on collect, restartTier() | 1.1.0 |
| 2026-06-16 | 011-princess-quest | 3 rounds (speed 6/8.5/11, 5/6/7 stars), tier badge, inter-round toast, 14-particle sparkle burst, Fredoka One | 1.1.0 |

## Games due for improvement (all at v1.0.0)

Priority candidates — pick whichever has the clearest improvement path:

- ~~**006-fairy-tale-tap**~~ — ✅ done v1.1.0
- ~~**011-princess-quest**~~ — ✅ done v1.1.0
- ~~**013-magic-leaf**~~ — ✅ done v1.1.0
- **015-mermaid-lagoon-v2** — tier badge, more NPC variety
- ~~**018-size-sort**~~ — ✅ done v1.1.0
- ~~**019-feelings-faces**~~ — ✅ done v1.1.0
- ~~**020-opposites**~~ — ✅ done v1.1.0
- ~~**021-body-parts**~~ — ✅ done v1.1.0
- ~~**022-magic-adding**~~ — ✅ done v1.1.0
- ~~**023-spatial-princess**~~ — ✅ done v1.1.0
- ~~**024-rhyme-time**~~ — ✅ done v1.1.0
- ~~**025-princess-sort**~~ — ✅ done v1.1.0

## Skills not yet covered

See `CLAUDE.md` for the full prioritised list. Top 3 to build next:
1. ~~Sight words~~ — ✅ covered by `028-sight-words`
2. ~~Colour mixing~~ — ✅ covered by `029-colour-mixing`
3. Sorting by size (big vs small, biggest/smallest — pre-maths) — covered by 018 but could expand
4. ~~Body parts extension (left/right)~~ — ✅ covered by `033-left-right`
5. ~~Front/back body awareness~~ — ✅ covered by `035-front-back`
6. ~~Sequencing / ordinal concepts~~ — ✅ covered by `034-princess-sequence`
7. ~~Simple subtraction~~ — ✅ covered by `036-princess-takeaway`
8. ~~Time of day~~ — ✅ covered by `037-princess-day`
9. ~~Animal family recognition~~ — ✅ covered by `038-royal-babies`
10. ~~Odd-one-out / categorisation reasoning~~ — ✅ covered by `039-princess-puzzle`

## Next game ID
`040-<slug>`
