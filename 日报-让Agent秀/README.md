# 让 Agent 秀 — 每日日报生成器

> 说一句「下班了」，就能得到一份精美的 Apple 风格工作日报。

## 它能做什么

这是一个 Claude Code Skill，能自动扫描你的工作目录，生成一页精美的 HTML 日报。不需要手动填写任何内容 — 触发就行，日报自动生成。

**5 步自动流程：**

1. **扫描** — 找出今天在工作目录中修改过的所有文件
2. **统计** — 计算文件产出、新增行数、活跃项目数、核心产出数
3. **分析** — 读取 Git 提交记录和对话上下文，提炼核心成就
4. **生成** — 把真实数据填入 Apple 风格的 HTML 模板
5. **预览** — 启动本地服务器，浏览器打开即可查看

## 日报特色

- **毛玻璃设计** — 磨砂玻璃卡片、浮动渐变光球、丝滑的淡入动画
- **数字滚动动画** — 指标数字带缓动曲线滚动上升
- **3 个核心成就卡片** — 分类标签 + 描述 + 影响力亮点
- **实践洞察三栏** — Good Practice / Bad Practice / Best Prompt
- **Demo 自动嵌入** — 自动检测 HTML 文件，以 iframe 缩略图方式嵌入
- **任务流背景** — 滚动的时间线装饰，展示当天工作脉络
- **单屏布局** — 所有内容在一个屏幕内展示（100vh），无需滚动

## 安装方式

把这个文件夹复制到 Claude Code 的 skills 目录：

```bash
cp -r 日报-让Agent秀 ~/.claude/skills/
```

重启 Claude Code，Skill 会被自动识别。

## 触发词

以下任意一句话都可以触发：

| 触发词 | |
|--------|---|
| `日报` | `让agent秀` |
| `生成日报` | `工作总结` |
| `今日总结` | `下班了` |
| `做一份日报` | `帮我写日报` |
| `daily report` | `done for today` |

## 输出位置

日报生成在：

```
{你的工作目录}/daily-reports/YYYY-MM-DD/index.html
```

本地预览服务器自动启动在 `http://localhost:8686`。

## 环境要求

- [Claude Code](https://claude.ai/code)（Anthropic 的命令行 AI 助手）
- Python 3（用于启动本地预览服务器）
- Git（可选，有的话日报数据更丰富）

## 许可证

MIT

---

<p align="center">
  由 <strong>Shiliu AI</strong> 用 Claude Code 打造
</p>
