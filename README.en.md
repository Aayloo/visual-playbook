# Visual Playbook

**English** · [中文](README.md)

> For anyone who has material and has to present it: a reference library of **which effect suits which occasion**.

![License: MIT](https://img.shields.io/badge/license-MIT-12795f)
![Entries](https://img.shields.io/badge/entries-105-ef6f0c)
![Languages](https://img.shields.io/badge/languages-%E4%B8%AD%E6%96%87%20%7C%20English-2f5fbf)
![Links checked](https://img.shields.io/badge/links-105%20checked-6b7a94)

---

## What this is

When you are producing a report, a dashboard or a demo, the slowest part is rarely the content.
It is not knowing **what it should look like**. This repository collects presentation methods that are
already proven, and organises them into one list: which kind of effect suits which occasion, who to
reference for that occasion, and which open-source pieces save you writing code.

It is not a collection of screenshots. It is a collection of **methods**. Every entry states three things:

1. **Why it is worth a look** — the problem it solves.
2. **What to copy** — concretely, not "nice design".
3. **Ready-made pieces** — the library or tool that drops into a project.

105 entries, 8 categories, bilingual throughout, and 105 links opened and confirmed one by one.

## Who it is for

- **Anyone who files a weekly, monthly or project report** and does not want to start from a blank deck.
- **Anyone building a dashboard** that changes weekly while the layout should not change at all.
- **Anyone demoing a product or walking through a system** who wants the interface and the code shown side by side.
- **Anyone writing external reports or roadshow material** who wants it to look considered rather than templated.
- **Anyone who wants their work to look more professional** — most of it needs no coding at all.

In one line: **you have material, and it has to hold up in front of other people.**

## What you can do with it

| The problem | Category | Roughly what you get |
| --- | --- | --- |
| The weekly dashboard needs new data without a redesign | 03 Read the numbers | A templating approach built on one HTML file and a chart engine: ECharts, Tremor |
| You have to explain how a system runs | 01 Tell the story | A scroll narrative: pin the canvas, reveal one step per scroll |
| You need a product demo with interface and code together | 02 Demo the product | Interface beside code with live preview: Expo Snack, Sandpack |
| You need NAV curves and drawdown bands | 04 Draw the chart | Finance-specific charts with trading-software interaction: Lightweight Charts |
| You have to take a formal stage | 05 Take the stage | Slides written in Markdown, far faster to edit than PPT |
| The interface is "not quite there" and you cannot say why | 07 Build the interface | Swap the component base and consolidate colour and type into tokens |
| You do not know where to look for inspiration | 08 Find a reference | 38 sources: award galleries, mobile UI libraries, data journalism, studios |

---

## How the taxonomy works

Eight categories in two families, with one rule: **anything is either a technique you can build or a source
you look things up in — never both.**

| Family | Category | What is in it | Entries |
| --- | --- | --- | --- |
| **Approach** | 01 Tell the story | Scroll narratives that explain a process screen by screen | 9 |
| | 02 Demo the product | Interface beside code, live preview | 5 |
| | 03 Read the numbers | Dashboards, BI, data apps | 10 |
| | 04 Draw the chart | Chart engines and finance charts | 12 |
| | 05 Take the stage | Slides and reporting material | 9 |
| | 06 Make it move | Motion, transitions, 3D | 13 |
| | 07 Build the interface | Component libraries and design tokens | 9 |
| **Reference** | 08 Find a reference | Galleries, mobile UI libraries, data journalism, studios, product UI, open-source apps, report tools | 38 |

The seven approach categories are ordered by **what you are trying to do**, not by technology stack.
The eighth sits in its own family because those sites are places to go looking, not techniques.

---

## Which effect for which occasion

| Occasion | Approach | Reference | Ready-made |
| --- | --- | --- | --- |
| Daily or weekly dashboard | One HTML file plus a chart engine; data changes weekly, layout does not | FT Visual Journalism · Reuters Graphics | ECharts · Tremor |
| Project or system walkthrough | Scroll narrative: pin the canvas, reveal one step per scroll | Apple product pages · Basement Studio | scrollytelling · Scrollama |
| Product or app demo | Two columns: interface on one side, code on the other, highlighted step by step | Expo Snack · Apple SwiftUI tutorials | Sandpack · CodeHike |
| A prototype the audience clicks through | An interactive data app: no packaging, one link and it runs | Observable Framework | Streamlit · Dash |
| External report or roadshow page | Annual-report layout with interaction, images following the scroll | Shorthand · FT ig | Quarto · Observable Framework |
| Formal meeting or review | Slides written in Markdown, restrained motion | The pacing of an Apple keynote | Slidev · Marp |
| NAV and drawdown curves | Finance-specific charts matching trading-software interaction | TradingView · Koyfin | Lightweight Charts |
| Lifting the look of the interface | Swap the component base, consolidate colour and type into tokens | shadcn/ui · Linear | Tailwind tokens · MagicUI |

The short version: **dashboards use chart engines, reviews use scroll narratives, demos use side-by-side panels,
formal occasions use slides. Never mix all four on one page.**

---

## How to use it

1. **Start with the occasion table above** to decide which kind of effect this job needs.
2. **Open the gallery** ([online](https://aayloo.github.io/visual-playbook/) or local
   [`docs/index.html`](docs/index.html)) and pick the closest entry in that category.
3. **Read the "Copy" line** — that is the actionable part; the case is only a reference.
4. **Prefer entries tagged open source** — those drop straight into a project.
5. **Record what worked** in [`CHANGELOG.md`](CHANGELOG.md) so the next job starts from evidence.

---

## Repository layout

```
visual-playbook/
├─ README.md            Chinese guide
├─ README.en.md         this file
├─ LICENSE              MIT
├─ data/cases.json      the single bilingual source of truth
├─ build/
│   ├─ template.html    page template
│   └─ build.mjs        generator
├─ docs/
│   ├─ index.html       generated: bilingual gallery (self-contained single file)
│   └─ repo-setup*.md   repository advice and usage
├─ references/
│   ├─ cases.md         Chinese checklist
│   └─ cases.en.md      English checklist
├─ tokens/              colour and type tokens
├─ THIRD_PARTY.md       linked third-party projects and licences
└─ CHANGELOG.md
```

`docs/` doubles as the GitHub Pages root, so once pushed the gallery lives at
**[aayloo.github.io/visual-playbook](https://aayloo.github.io/visual-playbook/)**.
It is also a self-contained single file: opening it locally gives the same result, and you can send it
to a colleague as is.

The important part: **`data/cases.json` is the single source of truth.** The page and both checklists are
generated. To add a case, change wording or fill in a translation, edit that one file and run:

```bash
node build/build.mjs
```

The build regenerates `docs/index.html`, `references/cases.md` and `references/cases.en.md`.
No dependencies to install. Commit the results and Pages updates itself.

---

## About the data

- **Checked**: 2026-09-28. All 105 links opened and confirmed.
- **Composition**: 56 open-source projects, 12 product references, 12 tools, 17 sites, 8 design studios.
- **Star counts** are live GitHub data from that date. They change, and they are not a quality score.
- **Blocked links.** Bloomberg Graphics, Canva, Gamma, 澎湃新闻 and Behance block automated requests but
  open normally in a browser.

---

## Licence

Everything written here — documentation, checklists, the generator, the design tokens — is under the
**MIT licence**, see [LICENSE](LICENSE). Take it, change it, use it commercially; keep the copyright notice.

Two things to keep in mind:

1. **The third-party projects linked from here have their own licences.** MIT covers only what is written
   in this repository.
2. A few carry commercial terms worth confirming — GSAP, Highcharts, fullPage.js — and Aceternity UI is a
   commercial product with copyable code, not an open-source library. Details are in
   [`THIRD_PARTY.md`](THIRD_PARTY.md).

---

## Contributing

If a link has died, a star count is stale, or you know a better ready-made piece for an effect, open an issue
or a pull request. Adding a case means adding one object to `data/cases.json`; the format is described in
[`docs/repo-setup.en.md`](docs/repo-setup.en.md).

---

<sub>Visual Playbook · 105 entries · 8 categories · 中文 / English · MIT</sub>
