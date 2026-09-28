# Changelog

Format: one entry per meaningful update. Note what was actually used, not only what was added.

## 2026-09-28 — v2026.09

Initial release.

- 105 entries across 8 categories, in two families: **Approach** (7 categories) and **Reference** (1 category).
- Bilingual throughout: `data/cases.json` carries `zh` and `en` for every description; the gallery has a
  language switch that persists in `localStorage`.
- 105 links opened and confirmed on this date. 56 entries are open-source projects with live star counts.
- Built the generator: one data file produces the gallery page and both checklists.
- Not yet done: no `patterns/` directory, no reusable code skeletons — the library is reference material only.

## 2026-09-28 — v2026.09.1

- Repository made public.
- Added an MIT licence covering this repository's own content.
- Rewrote both READMEs as a public-facing introduction: what this is, who it is for, what you can do
  with it, and what the licence does and does not cover.
- Moved the generated gallery from `gallery/index.html` to `docs/index.html`, because GitHub Pages can
  only publish from the repository root or `/docs`. It is now live at
  https://aayloo.github.io/visual-playbook/
