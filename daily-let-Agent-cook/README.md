# Let Agent Cook — Daily Report Generator

> Say "let agent cook" and get a stunning Apple-style daily work report in seconds.

## What It Does

This Claude Code skill automatically generates a single-page HTML daily report by scanning your working directory. No manual input needed — just trigger it, and your report is ready.

**The 5-step pipeline:**

1. **Scan** — Finds all files modified today in your working directory
2. **Measure** — Counts files shipped, lines added, active projects, and key deliverables
3. **Analyze** — Reads git history and conversation context to identify achievements
4. **Generate** — Fills an Apple-style HTML template with your real data
5. **Preview** — Starts a local server and opens the report in your browser

## Report Features

- **Glassmorphism design** — Frosted glass cards, floating gradient orbs, smooth fade-in animations
- **Animated metrics** — Counter numbers roll up with cubic-bezier easing
- **3 achievement cards** — Each with category tag, description, and impact highlight
- **Practice insights** — Good Practice, Bad Practice, and Best Prompt of the day
- **Demo embedding** — Auto-detects HTML files and embeds them as iframe previews
- **Task rail** — Scrolling timeline decoration in the background
- **Single screen** — Everything fits in one viewport (100vh), no scrolling

## Installation

Copy this folder into your Claude Code skills directory:

```bash
cp -r daily-let-Agent-cook ~/.claude/skills/
```

Restart Claude Code. The skill will be auto-detected.

## Trigger Words

Any of these will activate the skill:

| Trigger | |
|---------|---|
| `daily report` | `let agent cook` |
| `end of day` | `wrap up` |
| `done for today` | `what did I do today` |
| `generate report` | `EOD report` |
| `work summary` | `standup notes` |

## Output

Reports are saved to:

```
{your-working-directory}/daily-reports/YYYY-MM-DD/index.html
```

A local preview server starts at `http://localhost:8686`.

## Requirements

- [Claude Code](https://claude.ai/code) (Anthropic's CLI agent)
- Python 3 (for the local preview server)
- Git (optional, for richer commit-based data)

## License

MIT

---

<p align="center">
  Made with Claude Code by <strong>Shiliu AI</strong>
</p>
