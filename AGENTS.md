# manamaths-solutions

## Layout

- `OBJECTIVES/lo-yr9-<slug>/` — one folder per LO, mirroring `manamaths`
- `OPERATIONS/templates/` — shared LaTeX template for answer PDFs
- `OPERATIONS/scripts/` — build helpers
- `OPERATIONS/data/` — tracker (if we want one later)

## Conventions

- Mirror Mana Maths LO slugs one-to-one.
- Answer PDFs must look like the worksheet PDFs: same beamer template, same card layout, same header spacing, same 3x3 grid.
- Each module has exactly Foundation, Proficient, Excellence — no more, no less.
- Answers go inside each problem card so teachers can project them in class.
- **No website / HTML output.**
- Build with `tectonic` from this repo's root.
- No separate canonical JSON — refer to `manamaths-tasks/canonical/` when you need the source LO definition.
