# 视觉呈现素材库 · Visual Playbook

[English](README.en.md) · **中文**

汇报、展示、看板、路演的效果参考库。收的不是好看的截图，而是**做法**：
每条都写清楚它好在哪、可以抄什么、有没有现成的开源件能少写代码。

> 打开 [`gallery/index.html`](gallery/index.html) 看可视化版（中文 / English 可切换）。
> 想直接搜文字，看 [`references/cases.md`](references/cases.md)。

核对日期：**2026-09-28** · 105 条条目 · 8 个分类 · 105 个链接逐个访问确认

---

## 分类怎么分的

八个分类分两族，规则一句话讲完：**一个东西要么是「能动手做的做法」，要么是「拿来查的货源」，不重叠。**

| 族 | 分类 | 里面是什么 | 条数 |
| --- | --- | --- | --- |
| **做法 Approach** | 01 讲一个故事 Tell the story | 滚动叙事长页，一屏一屏讲清一个流程或系统 | 9 |
| | 02 演示一个产品 Demo the product | 左界面右代码、实时预览 | 5 |
| | 03 看一组数据 Read the numbers | 看板、BI、数据应用 | 10 |
| | 04 画一张图 Draw the chart | 图表引擎、金融图 | 12 |
| | 05 上一次讲台 Take the stage | 幻灯片与汇报材料 | 9 |
| | 06 让它动起来 Make it move | 动效、转场、三维 | 13 |
| | 07 搭一个界面 Build the interface | 组件库与设计变量 | 9 |
| **参考 Reference** | 08 找参考 Find a reference | 灵感榜、手机界面库、数据新闻、设计机构、产品界面、开源应用、报告工具 | 38 |

做法七类按「你要做什么」排，不是按技术栈排——这样找的时候是按目的找，不是按工具找。
第八类单独成族，因为那些站点的用途是「去那里看」，本身不是一种做法。

---

## 什么场合，用什么效果

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

## 仓库结构

```
visual-playbook/
├─ README.md            中文说明
├─ README.en.md         English guide
├─ data/cases.json      唯一数据源，中英双语
├─ build/
│   ├─ template.html    页面模板
│   └─ build.mjs        生成脚本
├─ gallery/index.html   生成物：双语画廊（自包含单文件）
├─ references/
│   ├─ cases.md         中文清单
│   └─ cases.en.md      English checklist
├─ docs/                仓库建议与用法
├─ tokens/              配色与字号变量
├─ THIRD_PARTY.md       抄来的代码出处与许可证
└─ CHANGELOG.md
```

关键一点：**唯一数据源是 `data/cases.json`。** 页面和两份清单都是生成出来的。
要加案例、改措辞、补英文，只改那一个文件，然后：

```bash
node build/build.mjs
```

构建会重新生成 `gallery/index.html`、`references/cases.md`、`references/cases.en.md`。
修完直接提交，GitHub Pages 也可以指向 `gallery/` 目录。

---

## 这份库怎么用

1. **先查场合表**，确定这次该用哪一类效果。
2. **进画廊**，在对应分类里挑一条最接近的。
3. **看「可以抄什么」那一行**，那才是真正动手的地方；案例本身只是参照。
4. **优先选开源件**，标签写着「开源」的可以直接装进项目。
5. 用完把结果记回 `CHANGELOG.md`，下次知道哪一个真的管用。

---

## 注意事项

- **许可证**：GSAP、Highcharts、fullPage.js、Tremor 的商用条款各不相同，对外材料先确认。
  Aceternity UI 是可以复制代码的商业产品，不是开源库。详情见 [`THIRD_PARTY.md`](THIRD_PARTY.md)。
- **星数**：核对当日的 GitHub 实时数据，会变，不必当作评价标准。
- **被拦截的链接**：Bloomberg Graphics、Canva、Gamma、澎湃新闻、Behance 等会挡住自动访问，
  浏览器里正常可开。
- **别把参考素材提交进业务仓库**。这里只放「怎么做出来」，成品留在各自的交付仓库里。
