# 仓库建议与用法

[English](repo-setup.en.md) · **中文**

## 为什么单独开一个仓库

如果把这份素材塞进业务仓库，会有三个问题：跨项目复用不了、交付物被污染、提交历史混成一条看不懂的时间线。
所以约定一句话：**业务仓库只放成品，这个仓库负责「怎么做出来」。**

建议的仓库分工：

| 仓库 | 可见性 | 装什么 |
| --- | --- | --- |
| `visual-playbook` | 私有 | 素材清单、方法论、可复用效果、设计变量 |
| 业务仓库（例如某个系统、某个工作台） | 按交付需要 | 只放能跑的产品代码和文档 |
| `visual-kit`（可选，以后再说） | 公开 + Template repository | 从本仓库抽出来的可复制起步模板 |

先只要第一个。等这个仓库里攒出三四个打磨过的模板，再抽 `visual-kit`，不要一开始就拆两个。

## 日常怎么用

### 加一条案例

只改 `data/cases.json`，在对应分类的 `items` 里加一个对象：

```json
{
  "name": "工具或项目的名字",
  "url": "https://example.com",
  "type": "oss",
  "stars": "★1,234",
  "why":  { "zh": "它好在哪，一两句话。", "en": "What makes it good, in one or two sentences." },
  "steal":{ "zh": "可以抄什么，落到具体。", "en": "What to copy, concretely." }
}
```

`type` 只能填这五个：`oss`（开源）、`site`（网站）、`tool`（工具）、`org`（机构）、`product`（成品）。
`stars` 不是开源项目就整个去掉，不要写「无」。

然后：

```bash
node build/build.mjs
```

### 加一个分类

在 `data/categories` 里加一个对象，照抄相邻分类的字段。
`family` 只能是 `approach`（做法）或 `reference`（参考）。
如果这一族里面还要再分组，给分类加 `subs`，再在每一条案例上写 `sub` 指过去——第八类「找参考」就是这么做的。

### 中英文都要改

每一条的 `why` 和 `steal` 都有 `zh` 和 `en` 两个字段。
**改中文的时候顺手把英文一起改**，只改一边，两边慢慢就会讲不同的事。

## 发布画廊

`gallery/index.html` 是自包含单文件，两种用法都行：

1. **本地双击打开**——最快，也方便直接发给同事。
2. **GitHub Pages**——仓库 `Settings → Pages → Source` 选 `main` 分支的 `/gallery` 目录。
   注意免费账号只给公开仓库发 Pages；仓库保持私有时，就靠单文件传播。

## 大文件

截图统一转 WebP；单个超过 1 MB 的、以及录屏，别直接提交，用 Git LFS 或者放到别处只留链接。

## 把「想做的效果」变成待办

在这个仓库里开一个 Projects 看板，三列就够：

| 想做 | 在做 | 已用上 |
| --- | --- | --- |
| 想试的效果、想抄的页面 | 正在改的模板 | 已经用在某份汇报里的 |

规则：一个效果**只有真正用在某份汇报里了**，才移到「已用上」。这样这个仓库不会变成只收藏不产出的地方。

## 几条约定

- 仓库名、文件名用英文小写连字符（`visual-playbook`），不要中文名。
- 给仓库加 topics 方便以后搜：`design-system` `data-visualization` `scrollytelling` `dashboard` `presentation` `templates`。
- 每次大更新打个 tag，例如 `v2026.09`，以后能对回「那次汇报用的是哪一版」。
- 抄来的代码和组件，记到 `THIRD_PARTY.md`，尤其是商用条款有限制的那几个。
