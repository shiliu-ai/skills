# Shiliu AI Skills Collection

> A growing collection of [Claude Code](https://claude.ai/code) skills — open source, ready to use.

<p align="center">
  <img src="https://img.shields.io/badge/Powered_by-Claude_Code-7C3AED?style=for-the-badge" alt="Powered by Claude Code">
  <img src="https://img.shields.io/badge/Made_by-Shiliu_AI-FF6B6B?style=for-the-badge" alt="Made by Shiliu AI">
  <img src="https://img.shields.io/badge/License-MIT-green?style=for-the-badge" alt="MIT License">
</p>

---

## What are Claude Code Skills?

Skills are reusable instruction sets for [Claude Code](https://claude.ai/code) (Anthropic's CLI agent). Instead of repeating the same prompts, a Skill teaches Claude a complete workflow — just say the trigger word, and it handles the rest.

## Available Skills

| Skill | Language | Description |
|-------|----------|-------------|
| [daily-let-Agent-cook](./daily-let-Agent-cook/) | English | Generate a beautiful Apple-style daily work report |
| [日报-让Agent秀](./日报-让Agent秀/) | 中文 | 生成精美的 Apple 风格每日工作日报 |

### Daily Report Generator

Both skills do the same thing in different languages — automatically generate a stunning single-page HTML daily report:

**What it does:**
1. Scans your working directory for today's modified files
2. Collects metrics (files shipped, lines added, active projects, key deliverables)
3. Reads git commit history (if available)
4. Analyzes context to identify achievements and insights
5. Generates a glassmorphism-styled HTML report and opens a local preview

**Trigger words:**
- English: `daily report`, `let agent cook`, `wrap up`, `done for today`, `EOD report`
- 中文: `日报`, `让agent秀`, `生成日报`, `工作总结`, `下班了`

**Report features:**
- Apple-inspired glassmorphism design (frosted glass cards, floating orbs)
- Animated counter metrics
- 3 achievement cards with impact highlights
- Good Practice / Bad Practice / Best Prompt insights
- Embedded HTML demo previews (auto-detected)
- Scrolling task rail background decoration
- Single-screen layout (100vh) — no scrolling needed

## Installation

### Option 1: Copy the skill folder

Download or clone this repo, then copy the skill folder you want into your Claude Code skills directory:

```bash
# English version
cp -r daily-let-Agent-cook ~/.claude/skills/

# Chinese version
cp -r 日报-让Agent秀 ~/.claude/skills/
```

Restart Claude Code — the skill will be auto-detected.

### Option 2: Clone the whole collection

```bash
git clone https://github.com/shiliu-ai/skills.git
```

Then copy whichever skills you need into `~/.claude/skills/`.

## Usage

Once installed, just tell Claude Code:

```
> let agent cook
```

or

```
> 下班了
```

Claude will scan your work, crunch the numbers, and generate a report at:

```
./daily-reports/YYYY-MM-DD/index.html
```

A local preview server starts automatically at `http://localhost:8686`.

## Contributing

We'll keep adding more skills to this collection. If you have ideas or want to contribute, feel free to open an issue or PR.

## License

MIT

---

<p align="center">
  Made with Claude Code by <strong>Shiliu AI</strong>
</p>

---

# Shiliu AI Skills 合集

> 一个持续更新的 [Claude Code](https://claude.ai/code) Skill 开源合集，拿来即用。

---

## 什么是 Claude Code Skill？

Skill 是 [Claude Code](https://claude.ai/code)（Anthropic 的命令行 AI 助手）的可复用指令集。不用每次重复输入复杂的提示词，只需要说一个触发词，Claude 就会自动执行完整的工作流程。

## 可用 Skills

| Skill | 语言 | 说明 |
|-------|------|------|
| [daily-let-Agent-cook](./daily-let-Agent-cook/) | English | Generate a beautiful Apple-style daily work report |
| [日报-让Agent秀](./日报-让Agent秀/) | 中文 | 生成精美的 Apple 风格每日工作日报 |

### 每日日报生成器

两个 Skill 功能完全一致，只是输出语言不同 — 自动生成一页精美的 HTML 工作日报：

**它会做什么：**
1. 扫描你的工作目录，找出今天修改过的所有文件
2. 统计关键指标（文件产出、新增行数、活跃项目数、核心产出数）
3. 读取 Git 提交记录（如果有的话）
4. 分析上下文，提炼核心成就和实践洞察
5. 生成一个毛玻璃风格的 HTML 日报页面，并启动本地预览

**触发词：**
- 中文：`日报`、`让agent秀`、`生成日报`、`工作总结`、`下班了`
- English: `daily report`, `let agent cook`, `wrap up`, `done for today`, `EOD report`

**日报特色：**
- Apple 风格毛玻璃设计（磨砂玻璃卡片、浮动光球）
- 数字滚动动画的指标卡片
- 3 个核心成就卡片（带影响力标签）
- Good Practice / Bad Practice / Best Prompt 三栏洞察
- 自动检测并嵌入 HTML Demo 预览
- 滚动任务流背景装饰
- 单屏布局（100vh）— 无需滚动

## 安装方式

### 方式一：复制 Skill 文件夹

下载或 clone 本仓库，然后把你需要的 Skill 文件夹复制到 Claude Code 的 skills 目录：

```bash
# 中文版
cp -r 日报-让Agent秀 ~/.claude/skills/

# English version
cp -r daily-let-Agent-cook ~/.claude/skills/
```

重启 Claude Code，Skill 会被自动识别。

### 方式二：克隆整个合集

```bash
git clone https://github.com/shiliu-ai/skills.git
```

然后按需复制到 `~/.claude/skills/` 即可。

## 使用方法

安装完成后，只需对 Claude Code 说：

```
> 下班了
```

或者

```
> let agent cook
```

Claude 会自动扫描你的工作、统计数据、生成日报到：

```
./daily-reports/YYYY-MM-DD/index.html
```

本地预览服务器会自动启动在 `http://localhost:8686`。

## 贡献

这个合集会持续更新更多 Skill。如果你有好的想法或者想贡献代码，欢迎提 Issue 或 PR。

## 许可证

MIT

---

<p align="center">
  由 <strong>Shiliu AI</strong> 用 Claude Code 打造
</p>
