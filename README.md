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
| [V6 — Every seat has a margin](decks/v6-every-seat-has-a-margin/) | DocSend × Eisenmann (HBS), ROI-purchase order | Light consulting minimalism, white + ink + emerald | 14 | wave two ✅ |
| [V7 — Built by the people who run it](decks/v7-built-by-the-people-who-run-it/) | Simon Sinek, Golden Circle | Bauhaus geometric flat, ink + electric violet | 11 | wave two ✅ |
| [V8 — The owner's second brain](decks/v8-owners-second-brain/) | Jobs-to-be-Done (Christensen et al.) | Warm documentary, honey light, recurring owner character | 12 | wave two ✅ |
| [V9 — Nightlife is a data category zero](decks/v9-nightlife-is-a-data-category-zero/) | a16z category-and-wedge | Abstract generative, violet-to-magenta gradients | 12 | wave two ✅ |
| [V10 — The clock is the moat](decks/v10-clock-is-the-moat/) | Tom Tunguz, seven investor questions | Brutalist mono-grid, black/white + warning yellow | 10 | wave two ✅ |
| [V11 — The answer first](decks/v11-the-answer-first/) | Minto Pyramid Principle, answer-first | FT-broadsheet analytics, salmon paper + navy ink | 11 | wave three ✅ |
| [V12 — Frame control](decks/v12-frame-control/) | Oren Klaff, Pitch Anything — frames before facts | Risograph poster, white + fluorescent pink/blue duotone | 10 | wave three ✅ |
| [V13 — The trailer, not the movie](decks/v13-the-trailer-not-the-movie/) | David S. Rose, pitching a VC — people first | Theatre playbill, aged cream + crimson, ACT I/II/III | 12 | wave three ✅ |
| [V14 — Cloud physics for the physical night](decks/v14-cloud-physics-for-the-physical-night/) | Bessemer Atlas discipline, metric-per-claim | Phosphor terminal, black + phosphor green | 11 | wave three ✅ |
| [V15 — The story you can retell](decks/v15-the-story-you-can-retell/) | First Round Review, story-first | Photocopy zine, newsprint grey + halftone collage | 11 | wave three ✅ |
| [V18 — Win the basement, then the block](decks/v18-win-the-basement-then-the-block/) | Crossing the Chasm, beachhead-first | Transit wayfinding, white + red line, station pins | 11 | wave four ✅ |

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

## Wave two

Wave two is delivered: V6 DocSend/HBS data-driven order, V7 Sinek Golden Circle, V8 Jobs-to-be-Done, V9 a16z category-and-wedge, and V10 Tunguz seven questions — briefed against the [sourced perspectives doc](research/pitch-deck-perspectives-sourced.md) and covered by the wave-two evaluation folio.
