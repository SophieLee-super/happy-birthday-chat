# Changelog

Every version of this project stays reachable — updates are always new commits on top, never rewrites, and milestone versions are kept as GitHub Releases so any older version can be downloaded exactly as it was.

This repo was first published at v6 (2026-11-18). The earlier iterations were built and reviewed one by one before the first upload; they're recorded here so the project's story is complete.

## v7 — 2026-11-20 · current · 中英合并 Bilingual

- **One project, one page, two languages**: the Chinese and English versions are merged into this single page — no more separate language repos
- New **中文 / EN switch** (top-right) flips everything: the full chat script (including the auto-computed "Crazy Weekday" joke), all birthday-fact screens (birth weekday, same-day celebrities Lewis Hamilton & Nicolas Cage, the Galileo history line, birth flower, days alive, turning age), the cake texts, the closing letter, and every hint / button / status label
- Switching mid-experience re-renders the current act in the new language; the chat replays from the start in that language
- Defaults to Chinese; `?lang=en` in the link opens it in English, and combines with `?date=`
- All four acts, the `?date=` birthday logic, images and interactions unchanged

## v6 — 2026-11-18

- Removed the zodiac screen and the birthstone (by request — less is more)
- The birth-flower screen now shows a photo of a carnation
- The same-day-birthday screen now has portrait cards: Lewis Hamilton and Nicolas Cage, each with a one-line intro
- All three photos are baked into the page itself — no external image links

## v5 — 2026-11-18

- Date-driven generation: give the page a birth date and it fills itself in
- The link can carry the date (`?date=2007-01-07`) — the whole special act and the weekday joke regenerate from it
- Demoed on 2007-01-07: born on a Sunday, next birthday a Thursday, turning 20, 7,305 days

## v4 — 2026-11-18

- The chat script was rewritten word-for-word by the author, with tap-only branching replies ("在的 / 咋了", "当然 / 啥日子呀"…) — the site now speaks in her exact words

## v3 — 2026-11-17

- Chat became one-way auto-play: her messages only, he never types — the free-text input box was removed ("he can't actually talk back, so don't fake it")
- Balloons increased to 16 on cake entry + 18 when the candle goes out

## v2 — 2026-11-17

- Chat now opens with exactly "在吗"
- Special-birthday fact cards replaced by one plain sentence per screen, tap to advance
- Cake flattened to a matte look, five candles reduced to one, balloons now rise from the bottom

## v1 — 2026-11-17

- First build: phone-style simulated chat, special-birthday cards, balloons / lights / cake, and a letter typed out character by character
