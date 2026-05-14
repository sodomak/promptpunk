# Cursor — deploying this pack into your project

## What to copy

1. Copy the entire **`.cursor`** folder from this directory into the **root** of your software repository (next to `package.json`, `go.mod`, etc.).
2. Copy **`.cursorignore.example`** to the project root as **`.cursorignore`** (or merge patterns with an existing file). Cursor will then **skip** those paths when indexing context — reducing accidental secret leakage into prompts.

## Rules vs legacy `.cursorrules`

- **Recommended format:** project rules in **`.cursor/rules/*.mdc`** (YAML frontmatter; see files in this pack).
- A root **`.cursorrules`** file is a **legacy** path; this handout standardises on **`.cursor/rules/`** only.

Documentation: [Cursor — Rules](https://docs.cursor.com/context/rules).

## Privacy settings

- In Cursor settings, choose the mode that matches your requirements for **sending code** to the model (UI labels evolve; names like *Privacy Mode* have appeared in the past — verify in your version).
- **Update** the editor regularly; security fixes apply to MCP and configuration surfaces too.

## MCP (Model Context Protocol)

- Enable only **MCP servers you trust**; read which tools the server registers (network, filesystem).
- MCP configuration is sensitive — do not copy configs blindly from the internet and do not commit secrets.

## Checklist

- [ ] `.cursor/rules/` is in git (shared with the team) but contains no secrets.
- [ ] `.cursorignore` covers `.env*`, keys, backups, large binaries.
- [ ] **Human review** and CI run before merging AI-generated changes.
