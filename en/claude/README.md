# Claude — two different contexts

## 1) Claude.ai (browser) — Projects

A Claude Project has its own **Project instructions** and often uploaded files. Steps:

1. Create a **Project** and paste **the fenced template block** from [`project-instructions.md`](project-instructions.md) into the instructions field. Copy the whole block at once.
2. Do **not** upload `.env` files, production exports, contracts with personal data, or internal documents that must not leave your company perimeter unless you have approval and the right account type.

## 2) Claude Code (terminal / IDE)

Claude Code has its own permission model, memory (`CLAUDE.md`), and Anthropic security docs. Read:

- [`claude-code-hardening.md`](claude-code-hardening.md) in this repo (short checklist).
- Official docs: [Claude Code — Security](https://docs.anthropic.com/en/docs/claude-code/security), [Permissions](https://docs.anthropic.com/en/docs/claude-code/permissions), [Memory](https://docs.anthropic.com/en/docs/claude-code/memory).

## Shared rule

**Secrets do not belong in git** — not in shared `CLAUDE.md`, not in README examples with real connection strings. Use local files ignored by git and a team-agreed convention.
