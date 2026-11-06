---
name: 休养生息 (xiuyangshengxi)
description: 三板斧家族纸账本世界的恢复分册——奶油纸地、墨线纸卡、宋体标题、朱红批注，把运动寿命当资产记账。
colors:
  ink: "#221e18"
  cream: "#f7f3ea"
  paper: "#fffdf8"
  paper-on-ink: "#f4efe4"
  bing: "#bf3a26"
  red: "#bf3a26"
  li: "#2e5f8b"
  zhong: "#a8722a"
  green: "#2e6e4e"
  yellow: "#b8860b"
  dashed-rule: "#d8d0bf"
  row-rule: "#eae3d2"
  mini-head: "#efe9da"
  small-text: "#6a6152"
  kicker-gray: "#8a8172"
  subtitle: "#5c5445"
  subtitle-deep: "#4a443a"
  footer-text: "#cfc6b4"
  footer-link: "#9fc3e8"
typography:
  display:
    fontFamily: "Songti SC, Noto Serif SC, Georgia, serif"
    fontSize: "clamp(34px, 7vw, 56px)"
    fontWeight: 900
    lineHeight: 1.1
  headline:
    fontFamily: "Songti SC, Noto Serif SC, Georgia, serif"
    fontSize: "clamp(24px, 4.8vw, 32px)"
    fontWeight: 900
  title:
    fontFamily: "Songti SC, Noto Serif SC, Georgia, serif"
    fontSize: "16.5px"
    fontWeight: 900
  numeral:
    fontFamily: "Songti SC, Noto Serif SC, Georgia, serif"
    fontSize: "clamp(22px, 4vw, 30px)"
    fontWeight: 900
  body:
    fontFamily: "-apple-system, PingFang SC, Helvetica Neue, sans-serif"
    fontSize: "15.5px"
    fontWeight: 400
    lineHeight: 1.75
  label:
    fontFamily: "-apple-system, PingFang SC, Helvetica Neue, sans-serif"
    fontSize: "12px"
    fontWeight: 700
    letterSpacing: "0.35em"
  ui:
    fontFamily: "-apple-system, PingFang SC, Helvetica Neue, sans-serif"
    fontSize: "13px"
    fontWeight: 700
rounded:
  card: "14px"
  cell: "10px"
  tag: "5px"
  badge: "4px"
  pill: "99px"
  stroke: "1px"
spacing:
  gutter: "22px"
  grid-gap: "14px"
  grid-gap-tight: "12px"
  chip-gap: "8px"
  card-pad: "16px 18px"
  section-y: "46px"
components:
  pill-filter:
    backgroundColor: "{colors.paper}"
    textColor: "{colors.ink}"
    rounded: "{rounded.pill}"
    padding: "4px 14px"
    typography: "{typography.ui}"
  pill-filter-on:
    backgroundColor: "{colors.ink}"
    textColor: "{colors.paper-on-ink}"
    rounded: "{rounded.pill}"
    padding: "4px 14px"
    typography: "{typography.ui}"
  nav-chip:
    backgroundColor: "{colors.paper}"
    textColor: "{colors.small-text}"
    rounded: "{rounded.pill}"
    padding: "2px 11px"
  share-button:
    backgroundColor: "{colors.paper}"
    textColor: "{colors.ink}"
    rounded: "{rounded.pill}"
    padding: "8px 22px"
  grade-badge-a:
    textColor: "{colors.green}"
    rounded: "{rounded.badge}"
    padding: "0 5px"
  grade-badge-b:
    textColor: "{colors.li}"
    rounded: "{rounded.badge}"
    padding: "0 5px"
  grade-badge-c:
    textColor: "{colors.zhong}"
    rounded: "{rounded.badge}"
    padding: "0 5px"
  grade-badge-d:
    textColor: "{colors.red}"
    rounded: "{rounded.badge}"
    padding: "0 5px"
  ledger-card:
    backgroundColor: "{colors.paper}"
    textColor: "{colors.ink}"
    rounded: "{rounded.card}"
---

# Design System: 休养生息 · 运动寿命账本

## Overview

**Creative North Star: "运动寿命账本 (The Longevity Ledger)"**

本站是「三板斧家族」纸账本世界的一册：奶油色（cream）桌面铺底，纸白（paper）卡片记账，1.5px 墨线勾边，宋体（Songti SC 栈）执笔标题与数字，系统黑体（PingFang SC 栈）写正文。账本语汇承载全部结构与导航——支出 / 回账 / 坏账 / 复利 / 审计，七个章节即七本分账。深度来自印刷式的硬偏移阴影（2–3px、零模糊），不来自光效；动效只有两处账房动作——条目落账入场与选中时的印章脉冲，均在 `prefers-reduced-motion` 下关闭。

反元素（已确认不出现）：无渐变、无照片、无暗色章节；墨色只以「封面块」形态出现（账单头、表头、页脚）。朱红（bing）是唯一批注色，稀有即分量。

**Key Characteristics:**

- 家族纸账本材质：cream 地 + paper 卡 + 1.5px 墨边 + 硬偏移阴影
- 宋黑分工：宋体 900 管标题、数字、徽章、印章式表头；黑体管正文与注释
- 账本语汇即信息架构（现金流 / 分级 / 坏账 / 跟腱 / 复利 / 审计 / 小额账目）
- 证据等级用四色数据编码（绿 / 蓝 / 青铜 / 红），与批注朱红严格分离
- 全站仅两处动效，共享同一条 easing（`cubic-bezier(.16,1,.3,1)`），可一键关闭

## Colors

纸账本调色：两层暖白（cream 地、paper 卡）上压一墨四彩，全部色值在 `:root` 定义。

### Primary

- **朱红批注 bing** (#bf3a26)：唯一强调色。h1 站名后半段、每章标题的 em 短语、激活时间块的边框与标题、统计卡大数字、流言卡的「“ ”」引号。每节至多一批注位。
- **墨 ink** (#221e18)：正文文字、全部 1.5px 边框、账单 / 表头 / 页脚等封面块底色、激活态药丸底色。

### Secondary

- **链接蓝 li** (#2e5f8b)：全站链接默认色（纸白上 6.61:1）；兼任 B 级证据色。
- **等级绿 green** (#2e6e4e)：A 级徽章、记账「＋」号、回账标签、绿灯圆点。
- **等级红 red** (#bf3a26)：与 bing 同值不同名——`--red` 只做语义（D 级、无效支出、「－」号、红灯、流言判定加粗），`--bing` 只做批注。写样式时跟随变量名分工。

### Tertiary

- **青铜 zhong** (#a8722a)：C 级徽章与速览数字。
- **信号黄 yellow** (#b8860b)：仅作黄灯圆点填充（非文字，3.20:1 不用于文字）。

### Neutral

- **奶油地 cream** (#f7f3ea)：body 底色；nav 以 94% 透明度加 8px 背景模糊复用。
- **纸白 paper** (#fffdf8)：所有卡片、表格、药丸底色。
- **纸上字 paper-on-ink** (#f4efe4)：墨色块上的文字（14.46:1）。
- **虚线规 dashed-rule** (#d8d0bf)：卡内虚线分隔（账单行、时间块左栏右缘）、浅色描边（药丸 / nav chips 默认边框）。
- **行线 row-rule** (#eae3d2)：表格行间实线。
- **表头纸 mini-head** (#efe9da)：mini 表表头底色。
- **小字 small-text** (#6a6152)：注释、图例、次级说明的统一色（cream 上 5.51:1，达标小字地板）。
- **kicker 灰 kicker-gray** (#8a8172)：仅限顶部 kicker 标签（3.47:1，故家族规约将其锁死在这一处装饰位）。
- **副题 subtitle** (#5c5445) / **副题深 subtitle-deep** (#4a443a)：章节副题 / hero 副文两级深灰。
- **页脚字 footer-text** (#cfc6b4) / **页脚链 footer-link** (#9fc3e8)：墨底页脚的正文与链接。

### Named Rules

**The Single Vermilion Rule.** 每个版面区域只有一种强调：朱红 bing 做批注，等级四色（绿 / 蓝 / 青铜 / 红）只做数据编码，永不兼任装饰。绿蓝青铜红不用于链接、标题或任何无等级语义的位置。

**The Small-Text Floor Rule.** cream/paper 上的说明文字不浅于 #6a6152（≥4.5:1）、不小于 11.5px；#8a8172 仅限 kicker 一处，禁止下移到任何承载信息的文字。

## Typography

**Display Font:** Songti SC（fallback: Noto Serif SC, Georgia, serif）
**Body Font:** -apple-system / PingFang SC（fallback: Helvetica Neue, sans-serif）

**Character:** 宋体 900 是账房先生的手——标题、数字、徽章、印章式表头一律宋体加粗，笔画密而压纸；黑体是记账员的日常字，承担全部正文与注释。全局 `line-break:strict`，数字与单位（如「7–9 小时」「30–40g」）以 `.nw` 锁定不断行。

### Hierarchy

- **Display** (900, clamp(34px, 7vw, 56px), 1.1)：h1 站名，仅首屏一处。
- **Headline** (900, clamp(24px, 4.8vw, 32px))：`h2.sec-head` 章节标题，格式「第N章 · 科目：em 批注短语」。
- **Title** (900, 16.5px)：卡片标题（ach-card h3 17px、test h3 与时间块时间 16.5px、流言标题 16px、账单头 15px + 0.2em 字距）。
- **Numeral** (900, clamp(22px, 4vw, 30px))：统计卡大数字、复利卡 big（24px）、tally 字母（17px）——账本里的金额一律宋体。
- **Body** (400, 15.5px, 1.75)：body 正文；卡内条目收窄至 13.2–13.8px / 1.6–1.7。
- **Label** (700, 12px, 0.35em 字距)：kicker，家族英文大写（"RECOVERY LEDGER"），#8a8172。
- **UI** (700, 13px)：药丸按钮、图例、hint。

### Named Rules

**The 宋黑分工 Rule.** 宋体只写七个字：标题、数字、徽章、引号、表头、站名、stamp。正文段落、列表、注释一律黑体。宋体排段落即出戏。

## Layout

单列账本流：`.wrap` 最大 1080px、左右 22px 内边距。sticky nav（top:0，`rgba(247,243,234,.94)` + `backdrop-filter: blur(8px)`，底缘 1.5px 墨线）内含站名、七个章节 chips 与家族链接；`html` 设 `scroll-padding-top:76px` 保证锚点落点不被 nav 遮挡。

首屏居中纵向流：kicker → h1 → 副文（660px 限宽）→「今晚的账单」卡（560px 限宽）→ 一句收束。章节统一 `padding:46px 0 4px`，每章 = sec-head + sec-sub（760px 限宽、14px）+ 器材。

多列网格与断点（全部降为单列，无中间档）：

| 网格 | 桌面 | 断点 |
|------|------|------|
| tally 等级速览 | 4 列 / gap 10px | ≤540px → 2 列 |
| statline 数据卡 | 3 列 / gap 12px | ≤640px → 1 列 |
| myths 流言卡 | 2 列 / gap 12px | ≤760px → 1 列 |
| comp 复利卡 | 2 列 / gap 14px | ≤760px → 1 列 |
| tests 自检卡 | 2 列 / gap 14px | ≤820px → 1 列 |
| foot3 足部卡 | 3 列 / gap 14px | ≤820px → 1 列 |

时间块 `.tblock` 是 150px | 1fr 双栏 grid（左时间右条目）；账目总表列宽 130 / 64 / auto / 230px，≤640px 隐藏「怎么做」列（`.hide-m`）。

交互布局：现金流章的四个时段药丸选中后，对应时间块 `scrollIntoView` 居中；账目章的等级筛选只做行显隐，不重排。

## Elevation & Depth

印刷式硬偏移阴影：零模糊、2–3px 位移、墨色带透明，全部配在 1.5px 墨边卡上。边框负责结构，阴影只确认「这张纸浮在桌上」；无环境光、无悬停抬升。

### Shadow Vocabulary

- **卡片静置** (`box-shadow: 2px 2px 0 rgba(34,30,24,.12)`)：时间块、总表、流言卡、统计卡、内容卡、自检卡的默认态。
- **首页账单** (`box-shadow: 3px 3px 0 rgba(34,30,24,.14)`)：仅 hero 账单卡，全页唯一的更深一档，标记「封面」地位。
- **印章激活** (`box-shadow: 3px 3px 0 rgba(191,58,38,.25)` + bing 边框)：选中时间块，阴影染红即盖章。

### Named Rules

**The Hard Offset Rule.** 阴影永远是 0 模糊的墨色偏移（2–3px），偏移量随状态加深（2px→3px）；禁止 blur、禁止彩色漫射光、禁止 hover 抬卡。墨色块（表头 / 页脚）不投影。

## Shapes

1.5px 墨线是全部绘图语言：卡片、表格、时间块、统计卡、tally 格共用同一条描边。圆角随容器尺寸分级：卡 14px、tally 格 10px、标签 5px、徽章 4px、药丸 99px（全圆端）；圆点（红绿灯 11px）与数字圆徽章（26px）用正圆。卡内分隔用 1px 虚线（#d8d0bf）模仿账本撕线，表格行用 1px 实线（#eae3d2），mini 表末行开放不封线。账目总表行首的 3px 等级色条以内嵌 box-shadow 实现（`inset 3px 0 0`），tally 划记为 3.5×15px、1px 圆角的墨色竖条。

## Components

### Chips（导航锚点）

- **Shape:** 全圆药丸（99px）
- **Style:** paper 底、#6a6152 字（12.5px）、1px #d8d0bf 边、内距 2px 11px
- **State:** hover 边框转墨；无选中态（点击即锚点跳转，非切换器）

### Pill filters（时段路由 / 等级筛选）

- **Shape:** 全圆药丸（99px）、内距 4px 14px、13px/700
- **Default:** paper 底 + 1.5px #d8d0bf 边 + 墨字；hover 边框转墨
- **Active:** 墨底 + #f4efe4 字——选中即「盖章入墨」
- **Note:** `.rt-btn` 与 `.f-btn` 视觉完全一致，是同一个器件的两个部署

### Cards / Containers

- **Corner Style:** 14px（统一）
- **Background:** paper
- **Shadow Strategy:** 见 Elevation & Depth（2px 静置 / 3px 首页账单）
- **Border:** 1.5px 墨，恒在
- **Internal Padding:** 14px 16px（统计卡）→ 16px 18px（流言 / 自检）→ 18px 20px（内容卡），随内容长度微升

### 今晚的账单（signature）

首屏核心器件：墨头条 + 三行记账条目。头部为墨底宋体 900（15px、0.2em 字距、#f4efe4、内距 7px 16px）；三行（支出 / 回账 / 无效支出）以 1px 虚线分隔，每行左侧 64px 定宽标签（5px 圆角、1px 描边、12px/800）：支出 = 墨、回账 = 绿、无效支出 = 红。入场为账目落账动画：`.55s cubic-bezier(.16,1,.3,1)` 上浮渐显，表头 0.05s、三行依次 0.17 / 0.29 / 0.41s 交错。

### 竖排时间块（tblock）

150px | 1fr 双栏纸卡：左栏宋体时间（16.5px/900）+ 黑体小注（11.5px），右缘 1px 虚线；右栏为 ＋/－ 记账列表。选中态换 bing 边框与标题、阴影染红，并播 stamp 印章脉冲（scale .995→1.012→1，`.4s`）。`prefers-reduced-motion:reduce` 下入场与脉冲一并关闭。

### ＋/－ 记账列表（plist）

条目 13.8px、行距 1.65，`padding-left:22px` 让位给行首记账符号：`＋`（绿）/`－`（红），900 字重、绝对定位左缘。条目内小注（12px、#6a6152）与证据徽章内联混排。

### 等级徽章（.g）

11px 宋体 900 方角徽章（4px 圆角、1px 描边同色、内距 0 5px），A/B/C/D 四色（绿 / 蓝 / 青铜 / 红），内联跟随任何主张句末。账目总表行首另有 3px 同色内嵌条双重编码。

### 账目总表（table.ledger）

墨底宋体表头行（#f4efe4）+ paper 表身；单元 13.5px、行线 1px #eae3d2；行首 3px 等级色条；≤640px 隐藏末列。配合 tally 速览（宋体大写字母 + JS 生成的墨色划记竖条，5/3/3/3）与等级筛选药丸使用。

### mini 表（table.mini）

卡内嵌数据表：#efe9da 表头（1.5px 墨线下缘）、13px、行线 1px #eae3d2、末行开放。无外框无圆角——它住在卡片里，不自己成卡。

### 数据与指示器件

统计卡（宋体 900 bing 大数字 + 12.5px 注）；红绿灯圆点（11px 正圆：绿 #2e6e4e / 黄 #b8860b / 红 #bf3a26，行内、margin-right 7px）；自检数字圆徽章（26px 墨底正圆、#f4efe4 宋体 900）；流言卡（宋体 900 谣言标题 + bing「“ ”」引号 + 判定加粗转红）。

### Ink blocks（封面块）

墨底反白块仅三处：账单头、总表表头、页脚（32px 0 38px、居中）。页脚字 #cfc6b4、链接 #9fc3e8；分享按钮为墨底上的 paper 药丸（hover 提白至 #fff，点击后文案换「✓ 已复制」1.6s）。

## Do's and Don'ts

### Do:

- **Do** 每张纸卡成对出现 1.5px 墨边 + 硬偏移阴影（14px 圆角），阴影随状态 2px→3px 加深。
- **Do** 证据等级只走四色编码：徽章、行首色条、tally 字母三处同步。
- **Do** 标题、数字、徽章、表头一律宋体 900；正文与注释一律黑体。
- **Do** 小字不小于 11.5px、不浅于 #6a6152；kicker 灰 #8a8172 只给 kicker。
- **Do** 数字与单位套 `.nw` 锁行（全局 `line-break:strict`）。
- **Do** 新章节沿用账本命名（支出 / 回账 / 坏账 / 审计……）与「第N章 · 科目：朱红短语」标题式。
- **Do** 所有动效用 `cubic-bezier(.16,1,.3,1)`，并包进 `prefers-reduced-motion:reduce` 关闭分支。

### Don't:

- **Don't** 用渐变、照片或大面积暗色；墨色只以账单头 / 表头 / 页脚三种封面块出现。
- **Don't** 给阴影加 blur 或彩色漫射；禁止 hover 抬卡——本世界没有「浮起」交互。
- **Don't** 在一节内引入第二种强调色；绿 / 蓝 / 青铜 / 红不承担等级以外的任何视觉职务。
- **Don't** 用宋体排正文段落，或用黑体排标题与金额。
- **Don't** 给 nav chips 加选中态——它们是锚点，不是筛选器。
- **Don't** 让链接默认色脱离 #2e5f8b（墨底块内除外，用 #9fc3e8）。
