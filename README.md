> **A tailored AI Skill (for Claude/Cursor) to generate authentic Reverse: 1999 web UI. Includes design tokens, strict geometric components, and signature paper/CRT motion physics.** 
> 专为 AI 辅助编程（如 Cursor/Claude）打造的《重返未来：1999》风格 UI 生成技能包。包含高度还原的设计令牌、切角组件库与纸片/CRT物理动效规则。

---

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
```

---

## 🚀 快速开始 (Quick Start)

1. **克隆或下载** 本仓库到你的本地目录。
2. 打开你的 AI 辅助编程工具（如 Cursor）。
3. 在对话中 `@` 引用 `SKILL.md` 及 `references/` 目录，并输入提示词。

**💬 提示词示例：**
> *"请阅读 `SKILL.md` 和 `references/` 下的所有文件。我要做一个‘邮件清空确认’的提示弹窗，请严格按照 Skill 里的规则，输出 HTML 和 CSS。"*

AI 将会自动为你生成包含**米色横幅、顶部 `^` 符号、几何折线暗纹、带倒三角切角的按钮**的高质量代码。

---

## 🧩 组件预览 (Component Highlights)

### 1. 提示弹窗 (Notice Modal)
*   **遮罩**：全屏毛玻璃模糊，深灰黑色。
*   **主体**：全宽的米色（`#f4e8e3`）横幅，文字为黑色宋体。
*   **按钮**：直角/微切角，内部带有细微的几何折线电路纹理。右上角有倒三角标。

### 2. 战斗血条与激情 (Health & Moxie)
*   **生命值**：带有轻微切角的平行四边形，暗绿色。
*   **激情值**：血条下方的 5 个菱形 ◇/◆。攒满时发出呼吸光晕，并使对应卡牌变形。

### 3. 星图 (The Scale)
*   利用 SVG 绘制，节点为多边形/圆形，线条相连。充能时，线条通过 `stroke-dasharray` 像电流一样点亮。

---

## 🎨 设计哲学 (Philosophy)

1999 的动效和 UI 不是现代 Web 的产物，而是对三种物理材质的模拟：

1.  **纸 (Paper)**：卡片和弹窗是纸片，入场不是放大，而是从一侧**伸展、卷曲**。
2.  **胶片 (Film)**：列表加载不是渐显，而是像电影帧一样**错峰浮出**。
3.  **CRT (老式显像管)**：Hover 反馈不是变亮，而是**电子管暖光晕染**；界面切换伴随**扫描线**的瞬间展开。

---

## 🤝 贡献 (Contributing)

如果你在游戏中发现了新的 UI 变体（如特定活动的特殊卡牌排版），或者优化了动效的 CSS 实现，欢迎提交 PR 或 Issue！

## 📄 License
[MIT License](LICENSE)
```
