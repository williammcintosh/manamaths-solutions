# manamaths-solutions

## Layout

- `OBJECTIVES/lo-<slug>/` — one folder per LO, mirroring `manamaths`
- `OPERATIONS/templates/` — shared LaTeX template for answer PDFs
- `OPERATIONS/scripts/` — build helpers
- `OPERATIONS/data/` — tracker (if we want one later)

## Conventions

- Mirror Mana Maths LO slugs one-to-one.
- Answer PDFs must look like the worksheet PDFs: same beamer template, same card layout, same header spacing, same 3x3 grid.
- Each module has exactly Foundation, Proficient, Excellence — no more, no less.
- Answers go inside each problem card so teachers can project them in class.
- **No website / HTML output. PDFs only.**
- Build with `tectonic` from this repo's root.
- The main site (`manamaths.co.nz`) automatically picks up answer PDFs during site regeneration — it copies `*-answers.pdf` into `manamaths/SITE/solutions-pdfs/<slug>/` and adds "Download solutions" buttons per scaffold.
- Scaffold headings on the site use koru icons only (no text labels like "Foundation").
- No separate canonical JSON — refer to `manamaths-tasks/canonical/` when you need the source LO definition.
- **Reference LO**: `manamaths/REFERENCE_LO.md` — complete pattern for all modules.

## Module status tracking

The overall module-completeness tracker lives at:
`manamaths/OPERATIONS/data/lo-meets-expectations.json`

Use `python3 manamaths/OPERATIONS/scripts/update-lo-status.py --sync-from-fs` after adding solutions to refresh status.
