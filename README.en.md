# Visual Playbook · 视觉呈现素材库

**English** · [中文](README.md)

A reference library for reporting, demos, dashboards and roadshows. Not screenshots — **methods**.
Every entry says what makes it good, what to copy, and whether a ready-made open-source piece saves you code.

> Open [`gallery/index.html`](gallery/index.html) for the visual version (switch between 中文 and English).
> To search the text directly, read [`references/cases.en.md`](references/cases.en.md).

Checked: **2026-09-28** · 105 entries · 8 categories · 105 links opened and confirmed

---

## How the taxonomy works

Eight categories in two families, with one rule: **anything is either a technique you can build or a source you look things up in — never both.**

| Family | Category | What is in it | Entries |
| --- | --- | --- | --- |
| **Approach** | 01 Tell the story | Scroll narratives that explain a process or system screen by screen | 9 |
| | 02 Demo the product | Interface beside code, live preview | 5 |
| | 03 Read the numbers | Dashboards, BI, data apps | 10 |
| | 04 Draw the chart | Chart engines and finance charts | 12 |
| | 05 Take the stage | Slides and reporting material | 9 |
| | 06 Make it move | Motion, transitions, 3D | 13 |
| | 07 Build the interface | Component libraries and design tokens | 9 |
| **Reference** | 08 Find a reference | Award galleries, mobile UI libraries, data journalism, studios, product UI, open-source apps, report tools | 38 |

The seven approach categories are ordered by **what you are trying to do**, not by technology stack —
so you search by purpose rather than by tool. The eighth sits in its own family because those sites are places to
go looking, not techniques in themselves.

---

## Which effect for which occasion

| Occasion | Approach | Reference | Ready-made |
| --- | --- | --- | --- |
| Daily or weekly dashboard | One self-contained HTML file plus a chart engine; data changes weekly, layout does not | FT Visual Journalism · Reuters Graphics | ECharts · Tremor |
| Project or system walkthrough | Scroll narrative: pin the canvas and reveal one step per scroll | Apple product pages · Basement Studio | scrollytelling · Scrollama |
| Product or app demo | Two columns: interface on one side, code on the other, highlighted step by step | Expo Snack · Apple SwiftUI tutorials | Sandpack · CodeHike |
| A prototype the audience clicks through | Build an interactive data app: no packaging, one link and it runs | Observable Framework | Streamlit · Dash |
| External report or roadshow page | Annual-report layout with interaction, images and text following the scroll | Shorthand · FT ig | Quarto · Observable Framework |
| Formal meeting or review | Slides written in Markdown, with restrained motion | The pacing of an Apple keynote | Slidev · Marp |
| NAV and drawdown curves | Finance-specific charts with interaction matching trading software | TradingView · Koyfin | Lightweight Charts |
| Lifting the look of the interface | Swap the component base and consolidate colour and type into one set of tokens | shadcn/ui · Linear | Tailwind tokens · MagicUI |

The short version: **dashboards use chart engines, reviews use scroll narratives, demos use side-by-side panels,
formal occasions use slides. Never mix all four on one page.**

---

## Repository layout

```
visual-playbook/
├─ README.md            Chinese guide
├─ README.en.md         this file
├─ data/cases.json      the single bilingual source of truth
├─ build/
│   ├─ template.html    page template
│   └─ build.mjs        generator
├─ gallery/index.html   generated: bilingual gallery (self-contained single file)
├─ references/
│   ├─ cases.md         Chinese checklist
│   └─ cases.en.md      English checklist
├─ docs/                repository advice and usage
├─ tokens/              colour and type tokens
├─ THIRD_PARTY.md       origin and licence for copied code
└─ CHANGELOG.md
```

The important part: **`data/cases.json` is the single source of truth.** The page and both checklists are generated.
To add a case, change wording or fill in a translation, edit that one file and run:

```bash
node build/build.mjs
```

The build regenerates `gallery/index.html`, `references/cases.md` and `references/cases.en.md`.
Commit the results; GitHub Pages can point at the `gallery/` directory.

---

## How to use it

1. **Start with the occasion table** to decide which kind of effect this job needs.
2. **Go to the gallery** and pick the closest entry in that category.
3. **Read the "Copy" line.** That is the actionable part; the case itself is only a reference.
4. **Prefer entries tagged Open source** — those drop straight into a project.
5. **Record what worked** in `CHANGELOG.md` so the next job starts from evidence.

---

## Caveats

- **Licences.** GSAP, Highcharts, fullPage.js and Tremor each carry different commercial terms; confirm before
  using them in external material. Aceternity UI is a commercial product with copyable code, not an open-source
  library. See [`THIRD_PARTY.md`](THIRD_PARTY.md).
- **Star counts** are live GitHub data from the date checked. They change, and they are not a quality score.
- **Blocked links.** Bloomberg Graphics, Canva, Gamma, 澎湃新闻 and Behance block automated requests but open
  normally in a browser.
- **Do not commit reference material into delivery repositories.** This repository holds *how to build it*;
  the finished work belongs in its own project repository.
