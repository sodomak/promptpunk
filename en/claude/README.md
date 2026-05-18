# Claude

## What is in this folder

| File | Deployment type | Where / what to do |
|------|-----------------|-------------------|
| [`project-instructions.md`](project-instructions.md) | **Copy into settings** | Claude.ai → **Project** → **Instructions** field |
| [`claude-code-hardening.md`](claude-code-hardening.md) | **Read only** | Checklist for Claude Code (permissions, memory, bash) |
| (optional) same text as `project-instructions.md` | **Save files** | File `CLAUDE.md` in your repo **root** if you use **Claude Code** in the terminal |

## Copy into settings (Claude.ai — Projects)

1. In Claude.ai, create a **Project**.
2. Paste **the entire fenced block** from [`project-instructions.md`](project-instructions.md) into **Project instructions**.
3. Do **not** upload `.env` files, production exports, contracts with personal data, or internal documents that must not leave your company perimeter unless you have approval and the right account type.

Text from this repo is **not saved automatically** — you paste it in the project UI.

## Save files (optional — Claude Code)

If you use **Claude Code** in the terminal / IDE:

- You may copy the fenced block from [`project-instructions.md`](project-instructions.md) into **`CLAUDE.md`** at the root of your software repository (same nine rules).
- Do **not** put real secrets in `CLAUDE.md` — it often ends up in git.

## Claude Code — read only

Claude Code has its own permissions, memory, and shell. Read:

- [`claude-code-hardening.md`](claude-code-hardening.md) (checklist in this repo).
- [Claude Code — Security](https://docs.anthropic.com/en/docs/claude-code/security), [Permissions](https://docs.anthropic.com/en/docs/claude-code/permissions), [Memory](https://docs.anthropic.com/en/docs/claude-code/memory).

The same **nine security rules** apply as for ChatGPT and Cursor in the promptpunk repo.

## Shared rule

**Secrets do not belong in git** — not in shared `CLAUDE.md`, not in README examples with real connection strings.
