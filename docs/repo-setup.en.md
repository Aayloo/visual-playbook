# Repository setup and usage

**English** · [中文](repo-setup.md)

## Why this is a separate repository

Folding this material into a delivery repository causes three problems: it cannot be reused across projects,
it pollutes the deliverable, and the commit history becomes a timeline nobody can read.
The convention is one line: **delivery repositories hold finished work; this one holds how it gets built.**

| Repository | Visibility | What goes in it |
| --- | --- | --- |
| `visual-playbook` | Private | Case library, method, reusable effects, design tokens |
| Delivery repositories (a system, a workbench, a report) | As the delivery requires | Only the working product code and docs |
| `visual-kit` (optional, later) | Public + Template repository | Starter templates extracted from this repository |

Build only the first one for now. Once this repository holds three or four polished templates, extract
`visual-kit`. Do not split into two on day one.

## Everyday use

### Adding a case

Edit `data/cases.json` only, adding one object to the right category's `items`:

```json
{
  "name": "Name of the tool or project",
  "url": "https://example.com",
  "type": "oss",
  "stars": "★1,234",
  "why":  { "zh": "它好在哪，一两句话。", "en": "What makes it good, in one or two sentences." },
  "steal":{ "zh": "可以抄什么，落到具体。", "en": "What to copy, concretely." }
}
```

`type` accepts five values: `oss`, `site`, `tool`, `org`, `product`. Drop `stars` entirely for anything that is
not an open-source project rather than writing a placeholder.

Then run:

```bash
node build/build.mjs
```

### Adding a category

Add an object to `data/categories`, copying the fields from a neighbour. `family` is either `approach` or
`reference`. If a category needs internal grouping, give it `subs` and point each case at one with `sub` —
that is how category 08 ("Find a reference") is built.

### Keep both languages in step

Every `why` and `steal` carries `zh` and `en`. **Edit the English in the same pass as the Chinese.**
Changing one side only is how the two versions start meaning different things.

## Publishing the gallery

`gallery/index.html` is a self-contained single file, so both routes work:

1. **Open it locally** — fastest, and easy to send to a colleague.
2. **GitHub Pages** — `Settings → Pages → Source`, then `main` branch and the `/gallery` directory.
   Note that free accounts only publish Pages from public repositories; while this repository stays private,
   the single file is how it travels.

## Large files

Convert screenshots to WebP. Anything over 1 MB, and all screen recordings, should go to Git LFS or be hosted
elsewhere with only a link committed.

## Turning "effects I want to try" into a backlog

Open a Projects board in this repository with three columns:

| Want to try | In progress | In use |
| --- | --- | --- |
| Effects and pages worth copying | Templates being adapted | Already used in a real report |

One rule: an effect only moves to **In use** once it has actually appeared in a report.
That keeps this repository from becoming a collection that never produces anything.

## Conventions

- Use lowercase English with hyphens for repository and file names (`visual-playbook`), never Chinese names.
- Add topics so it stays findable: `design-system` `data-visualization` `scrollytelling` `dashboard` `presentation` `templates`.
- Tag significant updates, for example `v2026.09`, so you can trace which version a past report used.
- Record copied code and components in `THIRD_PARTY.md`, especially the ones with commercial restrictions.
