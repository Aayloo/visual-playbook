# Visual Playbook · 视觉呈现素材库

[English](README.en.md) · **中文**

> 给「手上有一堆内容、要讲给别人看」的人：一份**什么场合用什么效果**的参考库。

![License: MIT](https://img.shields.io/badge/license-MIT-12795f)
![Entries](https://img.shields.io/badge/entries-105-ef6f0c)
![Languages](https://img.shields.io/badge/languages-%E4%B8%AD%E6%96%87%20%7C%20English-2f5fbf)
![Links checked](https://img.shields.io/badge/links-105%20checked-6b7a94)

---

## 这是什么

做汇报、做看板、做演示的时候，最耗时间的往往不是内容，是**想不出该长成什么样**。
这个仓库把「别人已经证明好用的呈现方式」整理成一张清单：每一类效果适合什么场合、
那个场合该参考谁、有哪些现成的开源件可以少写代码。

它收的不是好看的截图，是**做法**。每条都写三件事：

1. **为什么值得看** —— 它解决的问题是什么。
2. **可以抄什么** —— 落到具体，不是「设计不错」这种话。
3. **现成件** —— 有没有开源库或者工具，能直接装进项目。

一共 105 条，分八个分类，全部中英双语，105 个链接都逐个访问核对过。

## 面向谁

- **要交周报、月报、项目汇报的人** —— 不想每次都从一张空白 PPT 开始。
- **要做看板的人** —— 数据每周换，版式想定下来一次就别再动。
- **要做产品演示、系统讲解的人** —— 想把界面和代码并排讲清楚。
- **要写对外报告、路演材料的人** —— 想让材料看起来像回事，而不是模板味。
- **想让自己做的东西看起来专业一点的人** —— 不写代码也能用上里面的一大半。

一句话：**你手上有一批内容，需要让它在别人面前站得住。**

## 能拿它做什么

| 你想解决的事 | 翻到哪一类 | 大概能拿到什么 |
| --- | --- | --- |
| 早会看板要更新，但版式不想重做 | 03 看一组数据 | 单文件 HTML 加图表引擎的模板化思路，代表工具 ECharts、Tremor |
| 要把一个系统怎么跑讲清楚 | 01 讲一个故事 | 滚动叙事长页，画布钉住、滚到哪一步揭示哪一步 |
| 要做产品演示，界面和代码并排 | 02 演示一个产品 | 左界面右代码、实时预览，代表工具 Expo Snack、Sandpack |
| 要画净值曲线、回撤区间 | 04 画一张图 | 金融专用图表，交互对齐交易软件，代表工具 Lightweight Charts |
| 要上一次正式讲台 | 05 上一次讲台 | 用 Markdown 写幻灯片，改起来比 PPT 快得多 |
| 觉得界面「差点意思」但说不出差在哪 | 07 搭一个界面 | 换掉组件底座，把配色和字号收敛成一套变量 |
| 不知道从哪找灵感 | 08 找参考 | 灵感榜、手机界面库、数据新闻、设计机构等 38 个来源 |

---

## 分类怎么分的

八个分类分两族，规则一句话讲完：**一个东西要么是「能动手做的做法」，要么是「拿来查的货源」，不重叠。**

| 族 | 分类 | 里面是什么 | 条数 |
| --- | --- | --- | --- |
| **做法** | 01 讲一个故事 Tell the story | 滚动叙事长页，一屏一屏讲清一个流程或系统 | 9 |
| | 02 演示一个产品 Demo the product | 左界面右代码、实时预览 | 5 |
| | 03 看一组数据 Read the numbers | 看板、BI、数据应用 | 10 |
| | 04 画一张图 Draw the chart | 图表引擎、金融图 | 12 |
| | 05 上一次讲台 Take the stage | 幻灯片与汇报材料 | 9 |
| | 06 让它动起来 Make it move | 动效、转场、三维 | 13 |
| | 07 搭一个界面 Build the interface | 组件库与设计变量 | 9 |
| **参考** | 08 找参考 Find a reference | 灵感榜、手机界面库、数据新闻、设计机构、产品界面、开源应用、报告工具 | 38 |

做法七类按「你要做什么」排，不按技术栈排 —— 找的时候按目的找，不按工具找。
第八类单独成族，因为那些站点的用途是「去那里看」，本身不是一种做法。

---

## 什么场合用什么效果

| 场合 | 推荐做法 | 参考对象 | 现成件 |
| --- | --- | --- | --- |
| 早会 / 周会动态看板 | 单文件 HTML 加图表引擎；数据每周换，版式不动 | FT 视觉新闻 · Reuters Graphics | ECharts · Tremor |
| 项目 / 系统汇报 | 滚动叙事长页：画布钉住，滚到哪一步就揭示哪一步 | Apple 产品页 · Basement Studio | scrollytelling · Scrollama |
| 产品 / App 演示 | 左右分栏：一边界面、一边代码，逐步高亮 | Expo Snack · Apple SwiftUI 教程 | Sandpack · CodeHike |
| 领导要「点着看」的原型 | 做成交互式数据应用，不打包、发个链接就能用 | Observable Framework | Streamlit · Dash |
| 对外报告 / 路演长页 | 可交互年报式排版，图文跟随滚动 | Shorthand · FT ig | Quarto · Observable Framework |
| 正式会议 / 评审 | 用 Markdown 写幻灯片，动效克制 | Apple Keynote 的节奏 | Slidev · Marp |
| 净值 / 回撤曲线 | 金融专用图表，交互对齐交易软件 | TradingView · Koyfin | Lightweight Charts |
| 界面观感想上一个台阶 | 换掉组件底座，配色和字号收敛成一套变量 | shadcn/ui · Linear | Tailwind tokens · MagicUI |

一句话原则：**看板用图表引擎，复盘用滚动叙事，演示用左右分栏，正式场合用幻灯片。四类不要混在一页里。**

---

## 怎么用

1. **先查上面的场合表**，确定这次该用哪一类效果。
2. **进画廊**（[在线版](https://aayloo.github.io/visual-playbook/) 或本地 [`docs/index.html`](docs/index.html)），
   在对应分类里挑一条最接近的。
3. **读「可以抄什么」那一行** —— 那才是真正动手的地方，案例本身只是参照。
4. **优先选标签写着「开源」的** —— 那些可以直接装进项目。
5. **用完记一笔**在 [`CHANGELOG.md`](CHANGELOG.md) 里，下次知道哪个真的管用。

---

## 仓库结构

```
visual-playbook/
├─ README.md            中文说明
├─ README.en.md         English guide
├─ LICENSE              MIT
├─ data/cases.json      唯一数据源，中英双语
├─ build/
│   ├─ template.html    页面模板
│   └─ build.mjs        生成脚本
├─ docs/
│   ├─ index.html       生成物：双语画廊（自包含单文件）
│   └─ repo-setup*.md   仓库建议与用法
├─ references/
│   ├─ cases.md         中文清单
│   └─ cases.en.md      English checklist
├─ tokens/              配色与字号变量
├─ THIRD_PARTY.md       引用到的第三方项目与许可证
└─ CHANGELOG.md
```

`docs/` 同时是 GitHub Pages 的发布目录，所以推上去之后画廊就在
**[aayloo.github.io/visual-playbook](https://aayloo.github.io/visual-playbook/)** 上。
它也是自包含单文件，本地双击打开效果一样，可以直接发给同事。

关键一点：**唯一数据源是 [`data/cases.json`](data/cases.json)。**
画廊页面和两份清单都是生成出来的。要加案例、改措辞、补英文，只改那一个文件，然后：

```bash
node build/build.mjs
```

构建会重新生成 `docs/index.html`、`references/cases.md`、`references/cases.en.md`，
不需要安装任何依赖。跑完直接提交，Pages 会自动更新。

---

## 数据说明

- **核对日期**：2026-09-28。105 个链接逐个访问确认。
- **构成**：56 条开源项目、12 条成品参考、12 个工具、17 个网站、8 家设计机构。
- **星数**：核对当日的 GitHub 实时数据，会变，不必当作评价标准。
- **被拦截的链接**：Bloomberg Graphics、Canva、Gamma、澎湃新闻、Behance 等会挡住自动访问，
  浏览器里正常可以打开。

---

## 许可证

本仓库自己写的内容（文档、清单、生成脚本、设计变量）采用 **MIT 许可证**，见 [LICENSE](LICENSE)。
可以直接拿去改、用在商业项目里，保留版权声明即可。

注意两件事：

1. **仓库里链接到的第三方项目各有各的许可证**，MIT 只覆盖本仓库自己写的东西。
2. 其中有几个的商用条款需要单独确认，比如 GSAP、Highcharts、fullPage.js；
   而 Aceternity UI 是可以复制代码的商业产品，不是开源库。
   详情和注意点写在 [`THIRD_PARTY.md`](THIRD_PARTY.md)。

---

## 贡献

发现链接失效、星数过期，或者知道某个效果有更好的现成件，欢迎提 Issue 或 PR。
加一条案例只需要改 `data/cases.json` 里的一个对象，格式见 [`docs/repo-setup.md`](docs/repo-setup.md)。

---

<sub>Visual Playbook · 105 条 · 8 个分类 · 中文 / English · MIT</sub>
