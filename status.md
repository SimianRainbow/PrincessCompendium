# Princess Compendium — Status

## Last update run
Date: 2026-06-25
- Improved: `039-princess-puzzle` → v1.1.0 (color-coded tier badge Easy/Medium/Hard; round pool expanded 9→18 with 3 random picks per tier for replay variety; floating background decorations; sparkle burst now targets tap position; 4 emoji sparkles + 12 dot sparkles = 16 total; tier confetti 25→42; round counter and tier toast unchanged but confetti increased)
- Added: `042-shadow-magic` — "Shadow Magic 🌒" teaching visual discrimination & shadow matching; show a colourful princess emoji, tap the matching dark silhouette from 3 choices; 18-round pool (6 per tier), 3 random per tier = 9 per game; Easy = very distinct shapes (crown, moon, unicorn), Medium = same category (flowers, animals, castle), Hard = similar outlines (star vs sparkle, lion vs tiger vs bear); CSS filter grayscale+brightness(0.08) for silhouette effect; sparkle burst on correct; wobble on wrong; tier-transition toast with playTierUp melody; 42-piece confetti on tier change; 56-piece confetti on win

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
| 2026-06-19 | 015-mermaid-lagoon-v2 | Fredoka One font, "Found: X/4" progress badge, 14-emoji CSS sparkle overlay on find, sea turtle NPC sprite | 1.1.0 |
| 2026-06-22 | 027-royal-weather | Fredoka One font, color-coded tier badge, tier-transition toast, sparkles 10→16, Round X/9 label | 1.1.0 |
| 2026-06-25 | 039-princess-puzzle | Color-coded tier badge Easy/Medium/Hard, 18-round pool (was 9), 3 random picks per tier, bg floaters, sparkle targets tap position, confetti 25→42 | 1.1.0 |

## Games due for improvement (all at v1.0.0)

Priority candidates — pick whichever has the clearest improvement path:

- ~~**006-fairy-tale-tap**~~ — ✅ done v1.1.0
- ~~**011-princess-quest**~~ — ✅ done v1.1.0
- ~~**013-magic-leaf**~~ — ✅ done v1.1.0
- ~~**015-mermaid-lagoon-v2**~~ — ✅ done v1.1.0
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
11. ~~Seasons recognition~~ — ✅ covered by `040-royal-seasons`
12. ~~Visual discrimination / shadow matching~~ — ✅ covered by `042-shadow-magic`

## Next game ID
`043-<slug>`
