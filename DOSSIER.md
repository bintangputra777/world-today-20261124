# Dossier — make.fun bounty "Sum up 24 November's world news in one image"

## Bounty (verified 25 Nov 2026, ~07:55 WIB)

- Bounty: **Sum up 24 November's world news in one image** — https://make.fun/bounty/news-image-20261124
- Slug: `news-image-20261124` · Prize: **$100, 50 places paid** (1st $20, 2nd $12, 3rd $6, 4th–10th $2 each, 11th–50th $1.20 each), USDC on Solana, escrow funded 2026-11-23.
- Deadline: **Thursday 26 Nov 2026, 07:00 WIB** (2026-11-26T00:00:00Z).
- Judging: an AI judge that can see images compares entries two at a time; the image itself must show the day's news (the judge has no news feed).
- Same format as the accepted 19–23 Nov entries (world-today-20261119 … world-today-20261123); this build reuses the verified render pipeline from the 20 Nov template.

## The image — five stories (checked 25 Nov against Just Security Early Edition 24 Nov 2026, The Global Eye 24 Nov 2026, Nexus Europa 24 Nov 2026, pollar.news conflicts 24 Nov 2026)

1. **GAZA — Israeli strike kills Hamas security chief.** Israeli airstrikes kill Hamas internal security chief Naeem Abu Nahel and six others in Gaza, medics say. (Just Security Early Edition, 24 Nov 2026.)
2. **UKRAINE — Russian strike on Zaporizhzhia kills two.** An overnight Russian attack hits an apartment block in Zaporizhzhia, killing two and wounding 40, including four children. (Just Security Early Edition, 24 Nov 2026.)
3. **EUROPE — Europe demands seat at Ukraine peace talks.** After Trump's call from Air Force One, European leaders at a Berlin summit insist any Ukraine deal must include Europe. (Nexus Europa, 24 Nov 2026.)
4. **NATO — NATO vows to defend space from Russia.** Chief Mark Rutte pledges NATO will defend space after reports Russia is preparing a nuclear-armed satellite. (The Global Eye / BBC, 24 Nov 2026.)
5. **COLOMBIA — Car bomb in Colombia wounds at least 25.** A car bomb in Villavicencio injures at least 25; Colombia's president blames FARC dissidents as violence flares. (pollar.news, 24 Nov 2026.)

Design: same newspaper front-page style as the earlier entries — navy masthead "THE WORLD TODAY / TUESDAY · 24 NOVEMBER 2026", five numbered colour-tagged rows, footer citing major news outlets. Rendered in code with Python/PIL (`scripts/render.py`) — no AI image generator.

## Program

`main.ts` copies `assets/entry.png` to `/output/entry.png` — deterministic, no network. Verified locally: two runs byte-identical and equal to the source asset.
