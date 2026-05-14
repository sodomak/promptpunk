# Security templates for vibe coding (ChatGPT, Claude, Cursor)

Handout from the **CryptoByte / promptpunk** talk — copy into your own project or account only what you use.

**Keep this tree in sync** with the Czech mirror under [`../`](../README.md) (same filenames and layout) so updates stay predictable.

## Layout

| Path | Purpose |
|------|---------|
| [`chatgpt/`](chatgpt/) | Custom Instructions and checklist for ChatGPT |
| [`claude/`](claude/) | Claude Projects instructions + Claude Code notes |
| [`cursor/`](cursor/) | `.cursor/rules/` templates and `.cursorignore` example |

## How to use

1. **ChatGPT:** open [`chatgpt/README.md`](chatgpt/README.md), paste `custom-instructions.md` into Custom Instructions.
2. **Claude (web):** new Project → instructions from [`claude/project-instructions.md`](claude/project-instructions.md).
3. **Cursor:** copy `cursor/.cursor` to your repo root and copy or merge `cursor/.cursorignore.example` as `.cursorignore`. Details in [`cursor/README.md`](cursor/README.md).

## Czech vs English paths

| Topic | Czech | English |
|-------|-------|---------|
| Root | [`../README.md`](../README.md) | [`README.md`](README.md) |
| ChatGPT | [`../chatgpt/`](../chatgpt/) | [`chatgpt/`](chatgpt/) |
| Claude | [`../claude/`](../claude/) | [`claude/`](claude/) |
| Cursor | [`../cursor/`](../cursor/) | [`cursor/`](cursor/) |

## Freshness and links

Best practices and product UIs change. This pack reflects **May 2026**; verify current settings with each vendor:

- [Cursor — Rules](https://docs.cursor.com/context/rules)
- [OpenAI — Security](https://openai.com/security)
- [Anthropic — Claude Code security](https://docs.anthropic.com/en/docs/claude-code/security)

## Disclaimer

These files are **not a legal or security audit**, do not replace corporate DLP, your contract with the model vendor, or your organisation’s training. You use them at your own risk.
