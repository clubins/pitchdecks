<!-- Exported from Obvious artifact art_3NmFyl2x: Deck Production Guide — Batch One (V1–V5) -->

# Deck Production Guide — Batch One (V1–V5)

You are producing ONE assigned deck version for Clubins. This guide is shared truth; your task description carries your version's angle, framework, visual direction, and slide outline. Spec of record: `art_dEznXido`.

## 1. Product truth (every version must be consistent with this)

- Clubins gives venue staff live visibility of **sound levels, occupancy, and environmental conditions** in bars and clubs — "sound levels, occupancy, and environmental conditions for venue staff, live" (clubins-hack README.md).
- German positioning: "misst Lautstärke, Auslastung und Umgebung in Bars und Clubs und macht daraus betriebsfähige Entscheidungsdaten" (website-hack README.md).
- Full stack: ESP32-S3 sensors with Rust firmware → Go ingestion → ClickHouse → Flutter dashboards (web, Android, iOS); NixOS infrastructure; ZITADEL auth.
- Live today: dashboard/api/ingest/beta.clubins.de resolve; firmware, Flutter, and Go checks passed validation 2026-10-25 (docs/macos-validation.md).
- Stage: pre-launch, recruiting pilot venues (pilot@clubins.de). Never claim public launch or paying customers.

## 2. Hard rules

- **English** throughout. 16:9 slides. Slide images exactly **1344×768**.
- Slide titles are **takeaway claims**, not topics. One idea per slide. 10–14 slides.
- **All imagery custom-generated** for your version (image-generation tool). No stock look, no art direction reused across versions, no dashboard screenshots of the real product — use styled dashboard renders instead.
- **Never put the product logo through image generation** — place the provided `clubins-logo.jpg` as a composed element only where your brief says so.
- Company metrics: use **only** the canonical placeholder numbers in §5, verbatim, tracked in the metrics register. Never invent additional company numbers.
- Market/regulation facts: use **only** the sourced facts document (importantDocuments). Frame noise as documented displacement risk, never a fake national statistic. Sensor-market figures are commercial estimates — label them.
- Team slide: **Patrick Haußmann** (Munich — founder, product & platform) and **Swiftb0y** (Berlin — engineering). No one else.

## 3. Image generation loop (QA your own slides)

1. Generate each slide at 1344×768 (`size="1344x768"`). Keep on-slide text minimal — large garbled text is a regenerate trigger.
2. **View every generated slide** (view-file) before packaging. Regenerate any slide with garbled/unreadable text, watermarks, or off-palette drift.
3. Keep character/scene consistency inside your version: reuse descriptors and `existingImageIds` for scene-continuity slides.

## 4. Formats and packaging (sandbox: computerId `obvious`)

Work in `/home/user/work/deck-<version>/slides/` (one PNG per slide, named `01-…png` …). Then:

```bash
# PDF
python3 -m img2pdf slides/*.png -o clubins-v<version>.pdf
# PPTX (16:9, full-bleed image per slide) — python-pptx and img2pdf are preinstalled
python3 make_pptx.py   # 13.333in x 7.5in slide, picture fill
# Upload
obvious files upload --path=clubins-v<version>.pdf --name="Clubins V<version> <Angle>.pdf"
obvious files upload --path=clubins-v<version>.pptx --name="Clubins V<version> <Angle>.pptx"
obvious files upload --path=$(zip slides.zip slides/*.png) --name="Clubins V<version> slides.zip"
```

## 5. Canonical placeholder metrics (verbatim, register-tracked)

| Metric | Value |
|---|---|
| Founded | 2025 (Munich) |
| Team size | 2 |
| Venue interviews conducted | 40 |
| Design-partner LOIs signed | 5 |
| Pilot venues installing | 3 (Q1 2027) |
| Waitlist venues | 120 |
| Sensors produced | 25 |
| Pilot → paid conversion | 80% |
| Price | €149 / venue / month |
| Hardware | €199 / sensor |
| Ask | €500k pre-seed (SAFE) |
| Runway | 12 months |
| Use of funds | 2 engineering hires + sensor batch #2 (200 units) + 10 pilot venues |
| Target | 100 venues by end of 2027 |

Every one of these lands in the Placeholder Metrics Register with status PLACEHOLDER — Patrick swaps real values later. Do not add numbers.

## 6. Acceptance criteria (ship gate — verify before reporting)

1. 10–14 slides, English, your framework followed.
2. Every slide title is a takeaway claim; one idea per slide.
3. Every generated slide viewed and legible; art direction consistent inside the version.
4. PDF page count == slide count (`pdfinfo`); PPTX opens with the same count (python-pptx read-back).
5. Placeholder numbers used verbatim; market claims carry their source; no invented market numbers.
6. Files uploaded (PDF, PPTX, PNG zip) and file ids reported.

## 7. Report format

Report back: slide count, framework used, uploaded file ids (PDF/PPTX/zip), any deviations from the brief, and any acceptance criterion you could not meet.
