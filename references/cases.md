# 视觉呈现素材库 / Visual Playbook

> 汇报、展示、看板、路演的效果参考
>
> 核对日期: 2026-09-28 &nbsp;|&nbsp; 105 条目 &nbsp;|&nbsp; 8 分类

这里收的不是好看的截图，而是做法。每个案例都写清楚它好在哪、能直接抄什么、有没有现成的开源件。

**看板用图表引擎，复盘用滚动叙事，演示用左右分栏，正式场合用幻灯片。四类不要混在一页里。**

---

## 目录

- [01 讲一个故事](#01-讲一个故事) — 9 条
- [02 演示一个产品](#02-演示一个产品) — 5 条
- [03 看一组数据](#03-看一组数据) — 10 条
- [04 画一张图](#04-画一张图) — 12 条
- [05 上一次讲台](#05-上一次讲台) — 9 条
- [06 让它动起来](#06-让它动起来) — 13 条
- [07 搭一个界面](#07-搭一个界面) — 9 条
- [08 找参考](#08-找参考) — 38 条

---

## 做法 / Approach

_七种可以直接用的手段。每一项都是一种效果。_

### 01 讲一个故事

把一个流程或一个系统，用滚动一屏一屏讲清楚。适合项目复盘、系统汇报。

| 名称 | 类型 | 星数 | 为什么值得看 | 可以抄什么 |
| --- | --- | --- | --- | --- |
| [Basement Studio · scrollytelling](https://github.com/basementstudio/scrollytelling) | 开源 | ★1,665 | 把长页面切成一个个场景，滚动驱动切换，这个团队的官网用的就是同一套引擎。 | 场景怎么切分、固定画布加进度指示 |
| [CodeHike](https://github.com/code-hike/codehike) | 开源 | ★5,385 | 代码逐行讲解、逐行高亮的引擎。要边讲边演示代码，这是最省力的一条路。 | 行内注释、高亮、分步骤推进的组合 |
| [React Scrollama](https://github.com/squirrelsquirrel78/react-scrollama) | 开源 | ★405 | 把「滚到第几步」变成状态变量的轻量库，做分步揭示最省事。 | 滚动位置到步骤的映射写法 |
| [Closeread（Quarto 扩展）](https://github.com/qmd-lab/closeread) | 开源 | ★236 | 在 Quarto 里写滚动叙事的扩展，报告和网页可以共用一份源文件。 | 一份 Markdown 同时产出报告和网页 |
| [Apple AirPods Pro](https://www.apple.com/airpods-pro/) | 成品 | — | 滚动一句一个画面，图随滚动放大缩小，把发布会的节奏搬到了网页上。 | 首屏文案的结构、逐句替换的排版 |
| [Apple Vision Pro](https://www.apple.com/vision-pro/) | 成品 | — | 极简底色、大留白、克制的动效，最能体现「贵」的一种做法。 | 留白比例与字体层级 |
| [Linear](https://linear.app) | 成品 | — | 深色、大字、动效克制，是产品感最强的一类官网。 | 首屏三行文案怎么写、快捷键演示动画 |
| [Vercel](https://vercel.com) | 成品 | — | 技术产品的官网范式，把抽象的东西画成一眼看懂的图。 | 用示意图讲架构，而不是用文字堆 |
| [Stripe](https://stripe.com) | 成品 | — | 长期被当作企业官网的设计标杆，信息密度高但不乱。 | 分栏节奏、产品截图的呈现方式 |

### 02 演示一个产品

左边界面、右边代码，改一行看一行。做产品演示、技术分享时最直观。

| 名称 | 类型 | 星数 | 为什么值得看 | 可以抄什么 |
| --- | --- | --- | --- | --- |
| [Expo Snack](https://snack.expo.dev) | 工具 | ★510 | 左边写代码，右边手机里实时跑起来。最接近「左边手机、右边敲代码」这个画面的现成工具。 | 直接当演示台用，改一行看一行 |
| [Sandpack](https://github.com/codesandbox/sandpack) | 开源 | ★6,246 | 把「代码加实时预览」嵌进你自己任何网页里。 | 嵌进内部文档，做成可交互的说明页 |
| [StackBlitz · WebContainer](https://github.com/stackblitz/webcontainer-core) | 开源 | ★4,644 | 在浏览器里跑完整前端工程，连依赖安装都不用配。 | 发一个链接就能演示，不配环境 |
| [Apple SwiftUI 教程](https://developer.apple.com/tutorials/swiftui) | 成品 | — | 左边代码、右边实时预览、分步骤高亮，这类演示的教科书。 | 步骤导航和当前步骤高亮的交互 |
| [Tailwind Play](https://play.tailwindcss.com) | 工具 | — | 改样式即时看到结果，现场调界面最快的方式。 | 开会时当场改给领导看 |

### 03 看一组数据

每周或每天更新的那一类，重点是数据换、版式不动，所以模板化比好看更重要。

| 名称 | 类型 | 星数 | 为什么值得看 | 可以抄什么 |
| --- | --- | --- | --- | --- |
| [Apache Superset](https://github.com/apache/superset) | 开源 | ★74,944 | 成熟的开源看板平台，接上数据库就能出图，不用自己写前端。 | 图表组合、筛选器布局、权限思路 |
| [Grafana](https://github.com/grafana/grafana) | 开源 | ★76,963 | 监控场景最强，实时刷新和阈值告警的看板做得最顺。 | 自动刷新、阈值变色的呈现方式 |
| [Metabase](https://github.com/metabase/metabase) | 开源 | ★49,440 | 非技术同事也能自己拖出图的 BI 工具。 | 让同事自助取数的组织方式 |
| [Redash](https://github.com/getredash/redash) | 开源 | ★28,817 | 写 SQL 直接出图，最适合数据人自己快速搭一版。 | 查询与图表的绑定方式 |
| [Lightdash](https://github.com/lightdash/lightdash) | 开源 | ★6,166 | 建在 dbt 上的看板，指标定义和看板同源，不容易出现两套口径。 | 指标口径统一的做法 |
| [Evidence](https://github.com/evidence-dev/evidence) | 开源 | ★6,962 | 写 Markdown 加 SQL 就直接生成看板，最适合每周更新的汇报。 | 把周报写成模板，数据换文件不换版式 |
| [Observable Framework](https://github.com/observablehq/framework) | 开源 | ★3,650 | 用 Markdown 生成数据报告和数据应用，可以导出成静态页面。 | 对外报告、可交互专题 |
| [Streamlit](https://github.com/streamlit/streamlit) | 开源 | ★45,845 | 半天就能做出「能点」的演示应用，参数一改图表跟着变。 | 给领导试参数的那种演示 |
| [Plotly Dash](https://github.com/plotly/dash) | 开源 | ★24,438 | 交互式数据应用框架，联动筛选做得比 Streamlit 更细。 | 多图联动的写法 |
| [Quarto](https://github.com/quarto-dev/quarto-cli) | 开源 | ★6,023 | 一份源码同时出报告、网页、幻灯片和 PDF。 | 汇报材料多形态统一输出 |

### 04 画一张图

图表引擎本身。选一个主力就够，换来换去只会让几份材料长得不像同一套。

| 名称 | 类型 | 星数 | 为什么值得看 | 可以抄什么 |
| --- | --- | --- | --- | --- |
| [Apache ECharts](https://github.com/apache/echarts) | 开源 | ★67,405 | 国内最稳的图表引擎，中文排版和交互都最省心，升级现有看板的首选。 | 主题配色、tooltip 与图例的中文排版 |
| [D3](https://github.com/d3/d3) | 开源 | ★113,774 | 自由度最高的可视化底层，别人做不出来的图靠它。 | 需要非常规图表时再上，学习成本高 |
| [Recharts](https://github.com/recharts/recharts) | 开源 | ★27,595 | 配 React 最顺手的图表库，组件化写法，改起来快。 | 把图表当普通组件拼装 |
| [Plotly.js](https://github.com/plotly/plotly.js) | 开源 | ★18,348 | 科学计算类图表最全，三维和统计图不用另找库。 | 统计分布类图表的画法 |
| [Highcharts](https://github.com/highcharts/highcharts) | 开源 | ★12,493 | 金融与商业报告里的老牌选择，图表交互打磨得很细。 | 图表内的交互与导出功能 |
| [AntV G2](https://github.com/antvis/G2) | 开源 | ★12,621 | 蚂蚁的可视化语法，做叙事型图表和看板都合适。 | 图表分层与标注的写法 |
| [Vega-Lite](https://github.com/vega/vega-lite) | 开源 | ★5,497 | 用一段 JSON 描述图表，不改代码就能换图，适合批量出图。 | 图表配置与数据分离 |
| [Observable Plot](https://github.com/observablehq/plot) | 开源 | ★5,390 | 几行代码出一张讲究的图，默认样式就很像出版物。 | 默认样式与留白，直接拿来当基准 |
| [Chart.js](https://www.chartjs.org) | 开源 | — | 最轻便的入门库，常规折线柱状饼图几分钟就能上。 | 简单图表不要过度设计 |
| [TradingView Lightweight Charts](https://github.com/tradingview/lightweight-charts) | 开源 | ★17,373 | TradingView 出的金融图表，K 线、净值曲线、回撤区间专用。 | 组合净值走势、回撤区间标注 |
| [Tremor](https://github.com/tremorlabs/tremor) | 开源 | ★3,639 | 专做看板卡片的组件库，指标加迷你趋势图的组合很舒服。 | 指标卡片的风格与信息密度 |
| [VisActor · VChart](https://www.visactor.io) | 工具 | — | 国产可视化套件，叙事型图表和看板都有现成件。 | 滚动叙事的图表写法 |

### 05 上一次讲台

正式场合还是幻灯片，但可以用 Markdown 写，改起来比 PPT 快得多。

| 名称 | 类型 | 星数 | 为什么值得看 | 可以抄什么 |
| --- | --- | --- | --- | --- |
| [Slidev](https://github.com/slidevjs/slidev) | 开源 | ★48,859 | Markdown 写幻灯片，代码高亮最好，适合技术类汇报。 | 一份 md 出正式演示稿 |
| [reveal.js](https://github.com/hakimel/reveal.js) | 开源 | ★72,352 | 网页幻灯片的鼻祖，插件生态最全。 | 讲解备注、分栏、图表插件 |
| [Spectacle](https://github.com/FormidableLabs/spectacle) | 开源 | ★10,165 | 用 React 写幻灯片，方便把自己做的图表组件直接嵌进去。 | 把看板嵌进演示页 |
| [Marp](https://github.com/marp-team/marp-cli) | 开源 | ★3,840 | Markdown 一键转 PDF 或 PPT，最省事的一条路。 | 快速出正式 PDF 交上去 |
| [impress.js](https://github.com/impress/impress.js) | 开源 | ★38,172 | 三维空间演示，回头率最高。 | 开场用一次，别全程用 |
| [WebSlides](https://github.com/webslides/WebSlides) | 开源 | ★6,325 | 现成的 HTML 幻灯片模板，样式完整，改文案就能用。 | 没有时间自己排时的起点 |
| [Gamma](https://gamma.app) | 工具 | — | 生成式演示工具，临时场合出稿最快。 | 救急用，正式稿还是自己排 |
| [Pitch](https://pitch.com) | 工具 | — | 模板质量明显高于自带 PPT，协作也顺。 | 找好看版式的起点 |
| [IEA World Energy Outlook](https://www.iea.org/reports/world-energy-outlook-2024) | 成品 | — | 权威报告的版式与图表规范，章节结构值得抄。 | 章节结构、图表注释写法 |

### 06 让它动起来

上面那些效果的技术底座。先只上平滑滚动，其余按需要再加。

| 名称 | 类型 | 星数 | 为什么值得看 | 可以抄什么 |
| --- | --- | --- | --- | --- |
| [Lenis](https://github.com/darkroomengineering/lenis) | 开源 | ★16,055 | 平滑滚动，性价比最高的一个改动，几行代码换掉生硬的手感。 | 直接加进任何现有页面 |
| [GSAP](https://github.com/greensock/GSAP) | 开源 | ★28,671 | 滚动、时间轴、逐帧动画的行业标准。 | 复杂动效才需要，商用授权先确认 |
| [Motion](https://github.com/motiondivision/motion) | 开源 | ★33,760 | 原 Framer Motion，React 项目里最顺手。 | 列表进出、卡片展开的过渡 |
| [anime.js](https://github.com/juliangarnier/anime) | 开源 | ★73,160 | 轻量、语法简单，做数字滚动和图标动画很好。 | 数字往上滚的动效 |
| [AutoAnimate](https://github.com/formkit/auto-animate) | 开源 | ★13,924 | 一行代码给列表加过渡，性价比极高。 | 筛选、排序时的列表过渡 |
| [Theatre.js](https://github.com/theatre-js/theatre) | 开源 | ★12,704 | 可视化作关键帧，像做动画片一样调页面。 | 需要精细编排动效时用 |
| [fullPage.js](https://github.com/alvarotrigo/fullPage.js) | 开源 | ★35,384 | 整屏滚动，一屏一节，演示感强。 | GPL-3.0，商用之前先确认 |
| [Swiper](https://github.com/nolimits4web/swiper) | 开源 | ★41,905 | 轮播与滑动的标配，卡片墙和案例墙都用它。 | 卡片墙的滑动手感 |
| [three.js](https://github.com/mrdoob/three.js) | 开源 | ★116,004 | 网页三维的完整方案，能做的东西最多。 | 收益最高但也最重，最后再考虑 |
| [react-three-fiber](https://github.com/pmndrs/react-three-fiber) | 开源 | ★32,580 | 用 React 的写法写 three.js，状态管理跟项目一致。 | 三维场景的组件化写法 |
| [Spline](https://spline.design) | 工具 | — | 不用写三维代码，拖出来就能嵌进网页。 | 想要三维但不想学 three.js 时的出口 |
| [Rive](https://rive.app) | 工具 | — | 交互动画交付，界面动效领域目前最好的选择。 | 界面里的动态图标、加载状态 |
| [Lottie](https://github.com/airbnb/lottie-web) | 开源 | ★32,129 | 设计师出动画、开发直接用的标准格式。 | 图标动效、空状态插画 |

### 07 搭一个界面

看起来很难的效果，大部分已经有现成组件。按技术栈选一个底座就够。

| 名称 | 类型 | 星数 | 为什么值得看 | 可以抄什么 |
| --- | --- | --- | --- | --- |
| [shadcn/ui](https://github.com/shadcn-ui/ui) | 开源 | ★124,728 | 现在做高级感界面的默认底座，组件代码直接进你的项目。 | 卡片、表格、标签页的层级与间距 |
| [MagicUI](https://github.com/magicuidesign/magicui) | 开源 | ★22,406 | 现成的动效组件：跑马灯、便当栅格、光束连线、程序坞，都是看起来很难的效果。 | 直接拿这些效果拼首屏 |
| [HeroUI](https://github.com/heroui-inc/heroui) | 开源 | ★30,839 | 原 NextUI，观感现代，动效自带。 | 快速搭出成体系的界面 |
| [Ant Design](https://github.com/ant-design/ant-design) | 开源 | ★99,629 | 企业级中后台的成熟方案，国内项目最稳。 | 表格、表单和复杂交互 |
| [Mantine](https://github.com/mantinedev/mantine) | 开源 | ★31,777 | 组件全、文档好，React 项目里上手快。 | 配套的 hooks 与表单校验 |
| [daisyUI](https://github.com/saadeghi/daisyui) | 开源 | ★42,495 | 纯 CSS 组件类，任何技术栈都能用，改主题最方便。 | 一键换主题的做法 |
| [Radix Primitives](https://github.com/radix-ui/primitives) | 开源 | ★19,340 | 无样式的交互底座，可访问性做得最扎实。 | 自己做组件时当底座 |
| [Tailwind CSS](https://github.com/tailwindlabs/tailwindcss) | 开源 | ★97,720 | 上面这些库几乎都建在它上面。 | 先把设计变量定下来，再谈组件 |
| [Aceternity UI](https://ui.aceternity.com) | 工具 | — | 大量发布会级的卡片、背景光效组件，代码可以直接复制。 | 首屏背景与卡片光效（商业产品，注意授权） |

## 参考 / Reference

_用来找东西的地方，本身不是做法。灵感榜、界面库、行业来源都在这里。_

### 08 找参考

要动手之前先去这些地方看。它们不是做法，是货源。

#### 网页灵感榜

| 名称 | 类型 | 星数 | 为什么值得看 | 可以抄什么 |
| --- | --- | --- | --- | --- |
| [Awwwards](https://www.awwwards.com) | 网站 | — | 全球网页设计评选榜，找成品灵感最快的地方。 | 按 Site of the Day 扫一遍，收集版面结构 |
| [Godly](https://godly.website) | 网站 | — | 人工筛选的高质量网页库，比综合榜更克制。 | 找干净而高级的版面参考 |
| [Land-book](https://land-book.com) | 网站 | — | 按行业和版面类型归档的落地页库，检索比刷榜高效。 | 先定版面结构，再填内容 |
| [Codrops](https://tympanus.net/codrops/) | 网站 | — | 不只给灵感，还给原理和可运行的代码，上手门槛最低。 | 照着它的示例改自己的页面 |

#### 手机界面库

| 名称 | 类型 | 星数 | 为什么值得看 | 可以抄什么 |
| --- | --- | --- | --- | --- |
| [Mobbin](https://mobbin.com) | 网站 | — | 真实 App 的截图与完整流程库，做某个 App 的界面时从这里找最快。 | 按行业筛，金融和投资类单独看 |
| [Refero](https://refero.design) | 网站 | — | 按界面元素检索的真实产品设计参考，颗粒度比截图库细。 | 找具体的图表页、设置页怎么排 |
| [Page Flows](https://pageflows.com) | 网站 | — | 录屏式记录真实产品的操作流程，能看清点下去之后发生什么。 | 设计交互流程时的对照 |
| [ScreensDesign](https://screensdesign.com) | 网站 | — | 按付费转化拆解真实 App 的界面，看的是设计背后的动机。 | 引导流程和付费页的写法 |
| [UI Sources](https://www.uisources.com) | 网站 | — | 按交互类型归类真实 App 的动效，找微交互很方便。 | 加载、展开、切换的过渡方式 |

#### 数据新闻

| 名称 | 类型 | 星数 | 为什么值得看 | 可以抄什么 |
| --- | --- | --- | --- | --- |
| [FT 视觉新闻](https://ig.ft.com) | 网站 | — | 把复杂数据讲成人人看得懂的图，做汇报最该学的一组。 | 图注写法、色彩克制、结论前置 |
| [Reuters Graphics](https://www.reuters.com/graphics/) | 网站 | — | 新闻级图表规范，每张图都能独立看懂。 | 图表标题直接写结论 |
| [The Pudding](https://pudding.cool) | 网站 | — | 用滚动和交互讲故事的天花板，视觉化叙事的范本。 | 数据叙事的分镜设计 |
| [Information is Beautiful](https://www.informationisbeautiful.net) | 网站 | — | 信息图的另一种路数，复杂关系画成一张图。 | 一张图讲清一个复杂议题 |
| [Our World in Data](https://ourworldindata.org) | 网站 | — | 图表规范、配色、注释方式都值得直接照搬。 | 统一配色体系加清晰图例 |
| [SCMP Infographics](https://www.scmp.com/infographics/) | 网站 | — | 中英双语环境下的信息图，最贴近香港读者的阅读习惯。 | 中英混排的图表标注 |
| [财新数字说](https://datanews.caixin.com) | 网站 | — | 中文语境下的数据叙事，最贴近你的受众。 | 中文标题写法、图表里的中文排版 |
| [澎湃新闻 · 美数课](https://www.thepaper.cn) | 网站 | — | 面向大众的数据栏目，把专业内容降维讲清楚。 | 给非专业读者的解释顺序 |

#### 设计机构

| 名称 | 类型 | 星数 | 为什么值得看 | 可以抄什么 |
| --- | --- | --- | --- | --- |
| [Active Theory](https://activetheory.net) | 机构 | — | 专做这类页面的顶级团队，作品集本身就是最好的参考库。 | 每个项目拆解它的入场动效与转场 |
| [Immersive Garden](https://www.immersive-garden.com) | 机构 | — | 滚动叙事与三维结合得非常顺，节奏控制是教科书级。 | 画面节奏与色彩克制度 |
| [Resn](https://www.resn.co.nz) | 机构 | — | 互动创意做得大胆，适合找「敢一点」的做法。 | 把互动机制当成叙事的一部分 |
| [Hello Monday](https://hellomonday.com) | 机构 | — | 大品牌官网的专业户，结构清晰、执行稳。 | 企业级官网的信息结构 |
| [Basement Studio](https://basement.studio) | 机构 | — | 自己开源了滚动叙事引擎，官网就是那套引擎的展示。 | 把官网当成技术方案的说明书 |
| [Studio Freight](https://studiofreight.com) | 机构 | — | 把极简排版做到极致，页面几乎只有字和动效。 | 只用排版也能撑起一页 |
| [Locomotive](https://locomotive.ca) | 机构 | — | 平滑滚动库的开发者，官网手感就是标准答案。 | 滚动的手感和缓动曲线 |
| [Merci-Michel](https://www.merci-michel.com) | 机构 | — | 互动广告出身，擅长把复杂交互做得轻松。 | 让用户不动脑就知道下一步 |

#### 产品界面参考

| 名称 | 类型 | 星数 | 为什么值得看 | 可以抄什么 |
| --- | --- | --- | --- | --- |
| [Robinhood](https://robinhood.com) | 成品 | — | 投资类 App 的界面范式，信息密度和视觉层次的标杆。 | 持仓页与行情页的组织方式 |
| [Copilot Money](https://copilot.money) | 成品 | — | 个人理财 App 里设计口碑最好的之一，图表和分类做得极细。 | 消费分类与趋势图的配色 |
| [Koyfin](https://www.koyfin.com) | 成品 | — | 专业投研终端里界面最清爽的一个，图表密度高但不挤。 | 多图同屏时的间距与分区 |
| [TradingView](https://www.tradingview.com) | 成品 | — | 金融图表交互的行业基准，缩放和标注的手感最好。 | 图表上的标注与区间选择 |
| [Monarch Money](https://www.monarchmoney.com) | 成品 | — | 把资产总览做成一张图，个人财务的仪表盘范式。 | 总览页的层级安排 |

#### 开源应用（可跑起来看）

| 名称 | 类型 | 星数 | 为什么值得看 | 可以抄什么 |
| --- | --- | --- | --- | --- |
| [OpenBB](https://github.com/OpenBB-finance/OpenBB) | 开源 | ★73,556 | 开源的投研终端，界面专业，能在本地完整跑起来。 | 研究报告页与数据表的组织方式 |
| [Maybe](https://github.com/maybe-finance/maybe) | 开源 | ★54,262 | 开源个人理财应用，界面精致程度在开源界罕见，已停止维护但代码仍可参考。 | 图表配色与卡片层级 |
| [Ghostfolio](https://github.com/ghostfolio/ghostfolio) | 开源 | ★9,367 | 开源投资组合跟踪工具，正好对应多资产配置这个场景。 | 组合配置页与资产分布图 |
| [Actual Budget](https://github.com/actualbudget/actual) | 开源 | ★29,190 | 开源预算应用，交互响应快，前端实现干净。 | 表格类界面的键盘操作 |

#### 可交互报告工具

| 名称 | 类型 | 星数 | 为什么值得看 | 可以抄什么 |
| --- | --- | --- | --- | --- |
| [Shorthand](https://shorthand.com) | 工具 | — | 不写代码就能做可交互长报告，年报和专题页模板很多。 | 要快速出对外长页时用 |
| [Ceros](https://www.ceros.com) | 工具 | — | 设计自由度最高的交互内容平台，营销侧用得最多。 | 不写代码做复杂版式 |
| [Infogram](https://infogram.com) | 工具 | — | 图表和信息图模板最全的在线工具。 | 需要大量模板时按需取用 |
| [Tableau Public](https://public.tableau.com) | 工具 | — | 公开作品库，能看到别人怎么做联动和筛选。 | 多图联动的公开案例 |

## 核对日期 / Checked

2026-09-28 &nbsp;|&nbsp; 生成物，请勿直接编辑

- 星数为核对当日的 GitHub 实时数据。
- 标 `—` 的表示不是开源项目，没有星数。
- 个别站点会拦截自动访问，浏览器里正常可以打开。

---

本文件由 `build/build.mjs` 从 `data/cases.json` 生成，请不要直接编辑。
