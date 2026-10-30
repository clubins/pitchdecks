# Clubins Pitch Decks

Research-grounded investor pitch-deck variations for **Clubins** — an IoT platform for monitoring sound, occupancy, and environmental conditions in bars and clubs.

> ⚠️ **Company metrics are placeholders.** Every traction/revenue/market-share figure specific to Clubins is an invented placeholder pending verification — see `registers/placeholder-metrics.csv`. Market and regulation figures ARE sourced (Eurostat, Initiative Musik, Clubcommission Berlin, TA Lärm) and carry on-slide source labels. Do not send any deck to an investor before placeholders are replaced.

## Deck index

| Deck | Doctrine / source | Visual direction | Slides | Status |
|---|---|---|---|---|
| [V1 — Brand-true editorial](decks/v1-brand-editorial/) | Sequoia business-plan arc | Dark editorial, Playfair Display, amber | 12 | batch one ✅ |
| [V2 — Compliance & why-now](decks/v2-compliance-whynow/) | Kawasaki 10/20/30 | Swiss typographic, red/black/white | 10 | batch one ✅ |
| [V3 — Deep-tech moat](decks/v3-deep-tech-moat/) | YC / Kevin Hale, evidence-forward | Blueprint schematic, navy + cyan | 11 | batch one ✅ |
| [V4 — Venue OS vision](decks/v4-venue-os/) | Sequoia, vision-heavy variant | Warm magazine editorial, cream + burnt orange | 11 | batch one ✅ |
| [V5 — One Saturday, measured](decks/v5-one-saturday/) | Duarte sparkline storytelling | Cinematic dark-warm, timestamped scenes | 13 | batch one ✅ |
| [V7 — Built by the people who run it](decks/v7-built-by-the-people-who-run-it/) | Simon Sinek, Golden Circle | Bauhaus geometric flat, ink + electric violet | 11 | wave two ✅ |

V1 and V4 share Sequoia as their source doctrine — different angles and imagery, same framework. This is deliberate and flagged; see the perspectives doc.

Each deck folder contains the PDF, the PPTX, and `slides/` with all slide PNGs (plus the original zip archive).

## Repository layout

- `decks/` — the deck packages, one folder per version
- `research/` — sourced market facts, the pitch-deck perspectives doctrine map (with source URLs), and the batch-one production guide
- `spec/` — link to the approved spec (authored as an Obvious Blueprint: `art_dEznXido`)
- `registers/` — placeholder-metrics register (every invented figure, its status, and where it is used)
- `evaluation/` — comparative folio of batch one: [`batch-one-evaluation.html`](evaluation/batch-one-evaluation.html) (live version in the Obvious workspace, artifact `art_pfpnoU5W`)

## Verification notes

Deck packages were verified mechanically (pdfinfo page counts, python-pptx slide read-backs, zip entry counts, palette/luminance signatures, full-res OCR sweeps). OCR cannot fully verify some special glyphs (TA Lärm umlaut, sharp-s in Haußmann); one human visual pass is recommended before external use.

## Wave two (in production)

Five further versions — V6 DocSend/HBS data-driven order, V7 Sinek Golden Circle, V8 Jobs-to-be-Done, V9 a16z category-and-wedge, V10 Tunguz seven questions — are briefed against the [sourced perspectives doc](research/pitch-deck-perspectives-sourced.md) and land here when verified.
