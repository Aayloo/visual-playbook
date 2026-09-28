# Visual Playbook / 视觉呈现素材库

> Reference library for reporting, demos, dashboards and roadshows
>
> Checked: 2026-09-28 &nbsp;|&nbsp; 105 entries &nbsp;|&nbsp; 8 categories

Not screenshots — methods. Every entry says what makes it good, what to copy, and whether there is a ready-made open-source piece.

**Dashboards use chart engines, reviews use scroll narratives, demos use side-by-side panels, formal occasions use slides. Never mix all four on one page.**

---

## Contents

- [01 Tell the story](#01-tell-the-story) — 9 entries
- [02 Demo the product](#02-demo-the-product) — 5 entries
- [03 Read the numbers](#03-read-the-numbers) — 10 entries
- [04 Draw the chart](#04-draw-the-chart) — 12 entries
- [05 Take the stage](#05-take-the-stage) — 9 entries
- [06 Make it move](#06-make-it-move) — 13 entries
- [07 Build the interface](#07-build-the-interface) — 9 entries
- [08 Find a reference](#08-find-a-reference) — 38 entries

---

## Approach / 做法

_Seven techniques you can use directly. Each one is a specific effect._

### 01 Tell the story

Walk through a process or a system one screen at a time as the reader scrolls. For project reviews and system walkthroughs.

| Name | Type | Stars | Why it is worth a look | What to copy |
| --- | --- | --- | --- | --- |
| [Basement Studio · scrollytelling](https://github.com/basementstudio/scrollytelling) | Open source | ★1,665 | Splits a long page into scenes and drives the switch with scroll. The studio's own site runs on this same engine. | How scenes are carved up; pinned canvas plus progress indicator |
| [CodeHike](https://github.com/code-hike/codehike) | Open source | ★5,385 | An engine for line-by-line code walkthroughs and highlights. The least effort way to explain code as you present it. | Inline annotations, highlights and step-by-step advance |
| [React Scrollama](https://github.com/squirrelsquirrel78/react-scrollama) | Open source | ★405 | Turns 'which step are we on' into a state variable. The easiest way to build step-by-step reveals. | Mapping scroll position to a step index |
| [Closeread（Quarto 扩展）](https://github.com/qmd-lab/closeread) | Open source | ★236 | A Quarto extension for scroll narratives, so the report and the web page share one source file. | One Markdown file producing both report and site |
| [Apple AirPods Pro](https://www.apple.com/airpods-pro/) | Product | — | One sentence per screen; images scale as you scroll. Launch-event pacing, moved onto the web. | The hero copy structure; sentence-by-sentence replacement |
| [Apple Vision Pro](https://www.apple.com/vision-pro/) | Product | — | Minimal ground, generous whitespace, restrained motion. The clearest way to signal production value. | Whitespace ratio and type hierarchy |
| [Linear](https://linear.app) | Product | — | Dark, large type, restrained motion. The strongest example of product-feel on a marketing site. | How to write a three-line hero; how to animate a keyboard shortcut |
| [Vercel](https://vercel.com) | Product | — | A template for technical product sites: abstract concepts drawn as diagrams you get at a glance. | Explaining architecture with diagrams instead of paragraphs |
| [Stripe](https://stripe.com) | Product | — | A long-standing benchmark for corporate sites: high information density without the mess. | Column rhythm; how product screenshots are framed |

### 02 Demo the product

Interface on one side, code on the other, change a line and watch it land. The clearest format for product and technical demos.

| Name | Type | Stars | Why it is worth a look | What to copy |
| --- | --- | --- | --- | --- |
| [Expo Snack](https://snack.expo.dev) | Tool | ★510 | Code on the left, a live phone running it on the right. The closest off-the-shelf match to the split-screen demo you described. | Use it as the demo stage; change a line, show the result |
| [Sandpack](https://github.com/codesandbox/sandpack) | Open source | ★6,246 | Embeds code plus live preview into any page you already own. | Embed in internal docs to make an interactive explainer |
| [StackBlitz · WebContainer](https://github.com/stackblitz/webcontainer-core) | Open source | ★4,644 | Runs a full front-end project in the browser, no dependency setup needed. | Share one link and demo, with no environment setup |
| [Apple SwiftUI 教程](https://developer.apple.com/tutorials/swiftui) | Product | — | Code left, live preview right, step-by-step highlighting. The textbook version of this format. | Step navigation and current-step highlighting |
| [Tailwind Play](https://play.tailwindcss.com) | Tool | — | Change a style and see it immediately. The fastest way to adjust a layout live. | Editing the design live in a meeting |

### 03 Read the numbers

For weekly or daily refreshes the priority is that data changes while the layout does not. Templating matters more than looks.

| Name | Type | Stars | Why it is worth a look | What to copy |
| --- | --- | --- | --- | --- |
| [Apache Superset](https://github.com/apache/superset) | Open source | ★74,944 | A mature open-source dashboard platform: connect a database and chart, with no front-end work. | Chart sets, filter layout, permission model |
| [Grafana](https://github.com/grafana/grafana) | Open source | ★76,963 | Strongest for monitoring: live refresh and threshold alerts are the smoothest here. | Presenting auto-refresh and threshold colouring |
| [Metabase](https://github.com/metabase/metabase) | Open source | ★49,440 | A BI tool non-technical colleagues can drag a chart out of themselves. | Organising self-service access for colleagues |
| [Redash](https://github.com/getredash/redash) | Open source | ★28,817 | Write SQL, get charts. Best for a quick self-built version by whoever holds the data. | How queries bind to charts |
| [Lightdash](https://github.com/lightdash/lightdash) | Open source | ★6,166 | Dashboards built on dbt, so metric definitions and charts share one source of truth. | Keeping metric definitions consistent |
| [Evidence](https://github.com/evidence-dev/evidence) | Open source | ★6,962 | Markdown plus SQL produces the dashboard. The best fit for a weekly-updated report. | Turning the weekly report into a template: swap data, keep the layout |
| [Observable Framework](https://github.com/observablehq/framework) | Open source | ★3,650 | Markdown generates data reports and data apps, exportable as static pages. | External reports and interactive features |
| [Streamlit](https://github.com/streamlit/streamlit) | Open source | ★45,845 | Half a day gets you a clickable demo app where charts follow the parameters. | Demos where the audience tries the parameters |
| [Plotly Dash](https://github.com/plotly/dash) | Open source | ★24,438 | An interactive data app framework with finer cross-filtering than Streamlit. | Wiring several charts to each other |
| [Quarto](https://github.com/quarto-dev/quarto-cli) | Open source | ★6,023 | One source produces the report, the site, the slides and the PDF. | One report in several output formats |

### 04 Draw the chart

The chart engines themselves. Pick one as the workhorse; switching between them makes your material look unrelated.

| Name | Type | Stars | Why it is worth a look | What to copy |
| --- | --- | --- | --- | --- |
| [Apache ECharts](https://github.com/apache/echarts) | Open source | ★67,405 | The most dependable engine for Chinese-language charts, and the first choice for upgrading an existing dashboard. | Theme palettes; Chinese typography in tooltips and legends |
| [D3](https://github.com/d3/d3) | Open source | ★113,774 | The most flexible visualisation layer, for charts nobody else can produce. | Reach for it only for unusual charts; the learning curve is steep |
| [Recharts](https://github.com/recharts/recharts) | Open source | ★27,595 | The smoothest chart library for React: component-shaped, quick to adjust. | Treating charts as ordinary components |
| [Plotly.js](https://github.com/plotly/plotly.js) | Open source | ★18,348 | The most complete for scientific charts; 3D and statistical plots included. | Statistical and distribution charts |
| [Highcharts](https://github.com/highcharts/highcharts) | Open source | ★12,493 | A long-standing choice for financial and business reports, with finely polished interaction. | In-chart interaction and export features |
| [AntV G2](https://github.com/antvis/G2) | Open source | ★12,621 | Ant Group's grammar of graphics, good for both narrative charts and dashboards. | Layering and annotation in charts |
| [Vega-Lite](https://github.com/vega/vega-lite) | Open source | ★5,497 | Describe a chart in JSON and swap it without touching code. Good for generating charts in bulk. | Separating chart config from data |
| [Observable Plot](https://github.com/observablehq/plot) | Open source | ★5,390 | A polished chart in a few lines; the defaults already look like print. | Default styling and whitespace as a baseline |
| [Chart.js](https://www.chartjs.org) | Open source | — | The lightest starting point: ordinary line, bar and pie charts in minutes. | Not over-designing simple charts |
| [TradingView Lightweight Charts](https://github.com/tradingview/lightweight-charts) | Open source | ★17,373 | TradingView's finance charts, built for candlesticks, NAV curves and drawdown bands. | NAV curves and drawdown band annotations |
| [Tremor](https://github.com/tremorlabs/tremor) | Open source | ★3,639 | Components made for dashboard cards; the metric-plus-sparkline pairing reads well. | Metric card style and information density |
| [VisActor · VChart](https://www.visactor.io) | Tool | — | A Chinese visualisation suite with ready-made narrative charts and dashboards. | Charts that work inside a scroll narrative |

### 05 Take the stage

Formal occasions still call for slides, but Markdown produces them and they are far faster to edit than a PPT.

| Name | Type | Stars | Why it is worth a look | What to copy |
| --- | --- | --- | --- | --- |
| [Slidev](https://github.com/slidevjs/slidev) | Open source | ★48,859 | Slides in Markdown with the best code highlighting, made for technical talks. | One Markdown file producing a formal deck |
| [reveal.js](https://github.com/hakimel/reveal.js) | Open source | ★72,352 | The original web slide framework, with the broadest plugin ecosystem. | Speaker notes, columns and chart plugins |
| [Spectacle](https://github.com/FormidableLabs/spectacle) | Open source | ★10,165 | Slides written in React, so your own chart components drop straight in. | Embedding a dashboard in a deck |
| [Marp](https://github.com/marp-team/marp-cli) | Open source | ★3,840 | Markdown to PDF or PPTX in one command. The least effort route. | Producing a formal PDF to hand over |
| [impress.js](https://github.com/impress/impress.js) | Open source | ★38,172 | Three-dimensional presentations. The highest attention yield. | Use once at the opening, never throughout |
| [WebSlides](https://github.com/webslides/WebSlides) | Open source | ★6,325 | A complete HTML slide template. Change the copy and it is usable. | A starting point when there is no time to design |
| [Gamma](https://gamma.app) | Tool | — | A generative deck tool, fastest for last-minute occasions. | For emergencies; formal decks are still worth laying out yourself |
| [Pitch](https://pitch.com) | Tool | — | Noticeably better templates than bundled slide software, and smoother collaboration. | A starting point for a well-designed layout |
| [IEA World Energy Outlook](https://www.iea.org/reports/world-energy-outlook-2024) | Product | — | Layout and chart conventions from an authoritative report; the chapter structure is worth copying. | Chapter structure and chart annotation |

### 06 Make it move

The technical base under everything above. Start with smooth scrolling alone and add the rest on demand.

| Name | Type | Stars | Why it is worth a look | What to copy |
| --- | --- | --- | --- | --- |
| [Lenis](https://github.com/darkroomengineering/lenis) | Open source | ★16,055 | Smooth scrolling: the highest return per line of code, replacing a stiff scroll in minutes. | Add it to any existing page |
| [GSAP](https://github.com/greensock/GSAP) | Open source | ★28,671 | The industry standard for scroll, timeline and frame animation. | Only for complex motion; check the commercial licence first |
| [Motion](https://github.com/motiondivision/motion) | Open source | ★33,760 | Formerly Framer Motion, the smoothest fit in React. | List transitions and card expansion |
| [anime.js](https://github.com/juliangarnier/anime) | Open source | ★73,160 | Lightweight with simple syntax, good for counting numbers and icon animation. | Numbers that count up |
| [AutoAnimate](https://github.com/formkit/auto-animate) | Open source | ★13,924 | One line adds transitions to a list. Extremely high return. | List transitions during filter and sort |
| [Theatre.js](https://github.com/theatre-js/theatre) | Open source | ★12,704 | Visual keyframing: tune the page the way you would animate a film. | When motion needs precise choreography |
| [fullPage.js](https://github.com/alvarotrigo/fullPage.js) | Open source | ★35,384 | Full-screen scrolling, one section per screen, with a strong presentation feel. | GPL-3.0, confirm before commercial use |
| [Swiper](https://github.com/nolimits4web/swiper) | Open source | ★41,905 | The default for carousels and swipes; used for card and case walls. | The swipe feel of a card wall |
| [three.js](https://github.com/mrdoob/three.js) | Open source | ★116,004 | The complete solution for 3D on the web, capable of the most. | Highest ceiling but heaviest; consider it last |
| [react-three-fiber](https://github.com/pmndrs/react-three-fiber) | Open source | ★32,580 | three.js written the React way, with state management that matches the rest of the project. | Componentising a 3D scene |
| [Spline](https://spline.design) | Tool | — | No 3D code needed; drag it together and embed it. | The escape hatch when you want 3D without learning three.js |
| [Rive](https://rive.app) | Tool | — | Interactive animation handoff and currently the best choice for UI motion. | Animated icons and loading states in an interface |
| [Lottie](https://github.com/airbnb/lottie-web) | Open source | ★32,129 | The standard format for a designer to hand animation to a developer. | Icon motion and empty-state illustrations |

### 07 Build the interface

Most effects that look hard already have components. Pick one base for your stack and stay with it.

| Name | Type | Stars | Why it is worth a look | What to copy |
| --- | --- | --- | --- | --- |
| [shadcn/ui](https://github.com/shadcn-ui/ui) | Open source | ★124,728 | The default base for a refined interface today; component code lands in your own project. | Hierarchy and spacing in cards, tables and tabs |
| [MagicUI](https://github.com/magicuidesign/magicui) | Open source | ★22,406 | Ready-made motion components: marquees, bento grids, animated beams, docks. All the effects that look hard. | Assembling a hero out of them |
| [HeroUI](https://github.com/heroui-inc/heroui) | Open source | ★30,839 | Formerly NextUI: modern-looking with motion built in. | Building a coherent interface quickly |
| [Ant Design](https://github.com/ant-design/ant-design) | Open source | ★99,629 | The mature choice for enterprise back-office systems, and the safest in Chinese projects. | Tables, forms and complex interaction |
| [Mantine](https://github.com/mantinedev/mantine) | Open source | ★31,777 | Complete components and good documentation; quick to pick up in React. | Its hooks and form validation |
| [daisyUI](https://github.com/saadeghi/daisyui) | Open source | ★42,495 | Pure CSS component classes that work with any stack, and the easiest theming. | Switching themes in one step |
| [Radix Primitives](https://github.com/radix-ui/primitives) | Open source | ★19,340 | Unstyled interaction primitives with the most solid accessibility. | A base for building your own components |
| [Tailwind CSS](https://github.com/tailwindlabs/tailwindcss) | Open source | ★97,720 | Nearly every library above is built on it. | Fix the design tokens before touching components |
| [Aceternity UI](https://ui.aceternity.com) | Tool | — | A large set of launch-grade cards and background effects with copyable code. | Hero backgrounds and card glow (commercial product; check the licence) |

## Reference / 参考

_Places to go looking. Not techniques in themselves: galleries, UI libraries and industry sources._

### 08 Find a reference

Look here before you start. These are not techniques; they are where the material comes from.

#### Web galleries

| Name | Type | Stars | Why it is worth a look | What to copy |
| --- | --- | --- | --- | --- |
| [Awwwards](https://www.awwwards.com) | Site | — | The global web design awards. The fastest way to find finished inspiration. | Scan Site of the Day for layout structures |
| [Godly](https://godly.website) | Site | — | A hand-curated library of high-quality sites, more restrained than the big awards lists. | Finding clean, elevated layouts |
| [Land-book](https://land-book.com) | Site | — | Landing pages filed by industry and layout type. More efficient to search than to scroll an awards list. | Choosing the layout structure before writing content |
| [Codrops](https://tympanus.net/codrops/) | Site | — | Not just inspiration: explanations and working code. The lowest barrier to starting. | Adapting one of its demos to your own page |

#### Mobile UI libraries

| Name | Type | Stars | Why it is worth a look | What to copy |
| --- | --- | --- | --- | --- |
| [Mobbin](https://mobbin.com) | Site | — | Screenshots and complete flows from real apps. The fastest place to start on a specific app interface. | Filter by industry; browse finance and investing separately |
| [Refero](https://refero.design) | Site | — | Real product design references searchable by UI element; finer-grained than a screenshot library. | Seeing how a chart page or settings page is laid out |
| [Page Flows](https://pageflows.com) | Site | — | Screen-recorded flows from real products, showing what happens after the click. | A benchmark when designing an interaction flow |
| [ScreensDesign](https://screensdesign.com) | Site | — | Dissects real apps by conversion step, so you see the motive behind the design. | Onboarding flows and paywall pages |
| [UI Sources](https://www.uisources.com) | Site | — | Real app motion filed by interaction type; handy for micro-interactions. | Loading, expanding and switching transitions |

#### Data journalism

| Name | Type | Stars | Why it is worth a look | What to copy |
| --- | --- | --- | --- | --- |
| [FT 视觉新闻](https://ig.ft.com) | Site | — | Complex data turned into charts anyone can read. The single most useful reference for reporting. | Chart captions, restrained colour, conclusion first |
| [Reuters Graphics](https://www.reuters.com/graphics/) | Site | — | Newsroom-grade chart discipline: every chart stands on its own. | Writing the conclusion in the chart title |
| [The Pudding](https://pudding.cool) | Site | — | The ceiling for storytelling with scroll and interaction, and a model for visual narrative. | Storyboarding a data narrative |
| [Information is Beautiful](https://www.informationisbeautiful.net) | Site | — | A different route for infographics: complex relationships drawn as a single image. | Explaining a complex issue in one image |
| [Our World in Data](https://ourworldindata.org) | Site | — | Chart conventions, colour and annotation all worth adopting wholesale. | One colour system with clear legends |
| [SCMP Infographics](https://www.scmp.com/infographics/) | Site | — | Infographics in a bilingual environment, closest to how Hong Kong readers actually read. | Chart labelling with mixed Chinese and English |
| [财新数字说](https://datanews.caixin.com) | Site | — | Data storytelling written for a Chinese audience, closest to your readers. | Chinese headline writing and Chinese typography inside charts |
| [澎湃新闻 · 美数课](https://www.thepaper.cn) | Site | — | A mass-market data desk that makes specialist material legible to everyone. | The order in which things are explained to non-specialists |

#### Design studios

| Name | Type | Stars | Why it is worth a look | What to copy |
| --- | --- | --- | --- | --- |
| [Active Theory](https://activetheory.net) | Studio | — | A top-tier studio for exactly this kind of page; its portfolio is the reference library. | Break each project down into its entrance motion and transitions |
| [Immersive Garden](https://www.immersive-garden.com) | Studio | — | Scroll narrative fused smoothly with 3D; the pacing is textbook. | Pacing and colour restraint |
| [Resn](https://www.resn.co.nz) | Studio | — | Bold interactive work, useful when you need something braver. | Treating the interaction itself as part of the story |
| [Hello Monday](https://hellomonday.com) | Studio | — | Specialists in big-brand sites: clear structure, reliable execution. | Information architecture for an enterprise site |
| [Basement Studio](https://basement.studio) | Studio | — | They open-sourced their scroll narrative engine; the site is the demo of it. | Treating the site as documentation for the technique |
| [Studio Freight](https://studiofreight.com) | Studio | — | Minimal typography pushed to its limit; almost nothing but type and motion. | Carrying a whole page with typography alone |
| [Locomotive](https://locomotive.ca) | Studio | — | The makers of the smooth-scroll library; their site is the reference implementation. | Scroll feel and easing curves |
| [Merci-Michel](https://www.merci-michel.com) | Studio | — | From interactive advertising; good at making complex interaction feel effortless. | Signalling the next step without making anyone think |

#### Product UI references

| Name | Type | Stars | Why it is worth a look | What to copy |
| --- | --- | --- | --- | --- |
| [Robinhood](https://robinhood.com) | Product | — | The interface paradigm for investing apps, and a benchmark for density and hierarchy. | How positions and quotes pages are organised |
| [Copilot Money](https://copilot.money) | Product | — | Among the best-designed personal finance apps; charts and categories are finely done. | Colour in category and trend charts |
| [Koyfin](https://www.koyfin.com) | Product | — | The cleanest interface among professional research terminals: dense charts that still breathe. | Spacing and zoning when several charts share a screen |
| [TradingView](https://www.tradingview.com) | Product | — | The industry benchmark for financial chart interaction; zooming and annotation feel best here. | Annotation and range selection on a chart |
| [Monarch Money](https://www.monarchmoney.com) | Product | — | The whole net worth in one view; a dashboard paradigm for personal finance. | The hierarchy of an overview page |

#### Open-source apps you can run

| Name | Type | Stars | Why it is worth a look | What to copy |
| --- | --- | --- | --- | --- |
| [OpenBB](https://github.com/OpenBB-finance/OpenBB) | Open source | ★73,556 | An open-source investment research terminal with a professional interface that runs locally. | How research pages and data tables are organised |
| [Maybe](https://github.com/maybe-finance/maybe) | Open source | ★54,262 | An open-source personal finance app with rare polish for open source. No longer maintained, but the code still reads well. | Chart colour and card hierarchy |
| [Ghostfolio](https://github.com/ghostfolio/ghostfolio) | Open source | ★9,367 | An open-source portfolio tracker, matching the multi-asset allocation scenario directly. | Allocation pages and asset distribution charts |
| [Actual Budget](https://github.com/actualbudget/actual) | Open source | ★29,190 | An open-source budgeting app with fast interaction and a clean front-end. | Keyboard-first operation in table interfaces |

#### Interactive report tools

| Name | Type | Stars | Why it is worth a look | What to copy |
| --- | --- | --- | --- | --- |
| [Shorthand](https://shorthand.com) | Tool | — | Interactive long-form reports with no code, with plenty of annual-report and feature templates. | When an external long page is needed quickly |
| [Ceros](https://www.ceros.com) | Tool | — | The most design-flexible interactive content platform, most used on the marketing side. | Complex layout without writing code |
| [Infogram](https://infogram.com) | Tool | — | The online tool with the most complete chart and infographic templates. | Pulling templates when volume matters |
| [Tableau Public](https://public.tableau.com) | Tool | — | A public gallery showing how others build cross-filtering and linking. | Public examples of linked charts |

## Checked / 核对日期

2026-09-28 &nbsp;|&nbsp; generated, do not edit

- Star counts are GitHub data as of the date checked.
- A dash means the entry is not an open-source project and has no star count.
- A few sites block automated requests but open normally in a browser.

---

Generated by `build/build.mjs` from `data/cases.json`. Do not edit this file directly.
