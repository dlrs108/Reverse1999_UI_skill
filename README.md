# 📺 Reverse: 1999 UI Skill

> "A digital interface simulating physical objects and vintage electronics."
> 一个专为 AI 编程助手（如 Cursor、Claude、Windsurf）设计的 Skill，旨在让 AI 能够稳定、精确地生成《重返未来：1999》风格的 Web 界面代码。

---

## 💡 这是什么？

如果你直接让 AI “写一个 1999 风格的界面”，它往往会给出一个充满圆角、渐变平滑、扁平化的现代 UI，顶多加上一些毫无灵魂的噪点。

这个 Skill 不是简单的提示词。它是基于对《重返未来：1999》游戏内 **14 个核心界面**（大厅、抽卡、档案、战斗等）的逐像素拆解，提炼出的**一套严密的规则集**。

它强迫 AI 遵守 1999 的真实物理法则：**绝对直角、米色横幅弹窗、错位拼贴、纸片与 CRT 动效**。

## ✨ 核心特性 (Core Features)

- 🟫 **几何切角与线框 (Chamfered & Wireframe)**：摒弃所有 `border-radius`，大量使用 1px 极细线稿与几何缺口。
- 📜 **米色横幅弹窗 (Cream Banner Modals)**：极其反直觉的设计，在全黑背景中弹出 100% 宽度的浅粉色/米色横幅。
- 🎞️ **胶片错峰与通电动效 (Film & CRT Motion)**：拒绝平滑缓动，使用 `snap-then-settle` 曲线、纸片展开、电子管暖光晕染和扫描线故障。
- 🌌 **星图能量槽 (Constellation Scale)**：用 SVG 节点连线代替传统进度条，充能时伴随电流顺延的节点点亮。
- 🎴 **战斗状态 UI (Combat Status)**：带切角的平行四边形生命条 + 5 颗菱形激情（Moxie）槽。

---

## 📂 目录结构 (Structure)

```text
reverse1999-ui-skill/
├── SKILL.md                 # 核心入口：规则、触发条件、AI工作流
└── references/
    ├── tokens.md            # 色彩、字体、几何规则
    ├── components.md        # 按钮、弹窗、卡牌、战斗状态组件
    └── motion.md            # 动效物理隐喻与CSS关键帧参数
