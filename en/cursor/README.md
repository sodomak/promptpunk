# Cursor

## What is in this folder

| File / folder | Deployment type | Where / what to do |
|---------------|-----------------|-------------------|
| [`user-rules.md`](user-rules.md) | **Copy into settings** | **Cursor Settings → Rules** (global, all projects) |
| [`.cursor/`](.cursor/) (`rules/*.mdc`) | **Save files** | Copy into **`your-repo/.cursor/`** (next to `package.json`, `go.mod`, …) |
| [`.cursorignore.example`](.cursorignore.example) | **Save files** | Copy / merge as **`your-repo/.cursorignore`** |
| This README (MCP, privacy, checklist) | **Read only** | Extra editor settings |

**Recommended order:** User Rules first (once per machine), then optional project files (for team + git).

| | User Rules | Project `.cursor/rules/` |
|--|------------|---------------------------|
| Where | Cursor settings | Root of your repository |
| Git / team | No | Yes |
| When | Default in every repo | Stack-specific rules + sharing |

On conflict, **project** rules override User Rules. User Rules apply to **Agent (chat)**, not Tab or Inline Edit (Ctrl+K).

Documentation: [Cursor — Rules](https://cursor.com/docs/context/rules).

## Copy into settings

1. Open **Cursor Settings** (gear icon or *File → Preferences → Cursor Settings*).
2. Go to **Rules** (sometimes **Rules, Commands** or *Rules for AI*).
3. Paste **the entire fenced block** from [`user-rules.md`](user-rules.md) into **User Rules**.

This text is **not saved from git automatically** — paste it once in Cursor settings on this machine.

## Save files into your project

1. Copy the entire **`.cursor`** folder from this promptpunk directory into the **root** of your software repository → `your-repo/.cursor/rules/*.mdc`.
2. Copy **`.cursorignore.example`** to the project root as **`.cursorignore`** (or merge patterns with an existing file). Cursor will then **skip** those paths when indexing context.

Under `.cursor/rules/` you get among others:

- `security-vibe-coding.mdc` — same nine principles as `user-rules.md` (for Agent in this project).
- `secrets-and-data.mdc` — stricter rules for `.env`, Terraform, CI, Helm (when working on those files).

## Rules vs legacy `.cursorrules`

- **Recommended format:** `.cursor/rules/*.mdc` (YAML frontmatter).
- A root **`.cursorrules`** file is **legacy** — not used in this handout.

## Privacy settings

- Enable the mode that matches your requirements for **sending code** to the model (labels such as *Privacy Mode* have appeared — verify in your version).
- **Update** the editor regularly.

## MCP (Model Context Protocol)

- Enable only **MCP servers you trust**.
- Do not copy MCP configs blindly from the internet or commit secrets.

## Checklist

- [ ] **User Rules** set from [`user-rules.md`](user-rules.md).
- [ ] (Optional) `.cursor/rules/` in git with no secrets.
- [ ] `.cursorignore` covers `.env*`, keys, backups.
- [ ] **Human review** and CI before merging AI changes.
