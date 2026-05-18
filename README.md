# promptpunk

[![Latest release](https://img.shields.io/github/v/release/sodomak/promptpunk?label=release)](https://github.com/sodomak/promptpunk/releases/latest)

**Česky:** [přejít na českou verzi](#cesky) · [All releases](https://github.com/sodomak/promptpunk/releases) · [Download latest](https://github.com/sodomak/promptpunk/releases/latest)

---

<a id="english"></a>

Security templates for vibe coding (ChatGPT, Claude, Cursor).

Handout from the **CryptoByte** talk — copy into your own project or account only what you use.

Keep the Czech and English template trees in sync (same filenames and layout).

## Releases and versioning

| What | Where |
|------|--------|
| All releases | [github.com/sodomak/promptpunk/releases](https://github.com/sodomak/promptpunk/releases) |
| Latest download | […/releases/latest](https://github.com/sodomak/promptpunk/releases/latest) |
| Version in repo | [`VERSION`](VERSION) |

**SemVer:** changing files under `chatgpt/`, `claude/`, `cursor/`, or `en/` on `main` triggers an automatic **PATCH** release (tag `vX.Y.Z` + GitHub Release with source archives). **MINOR** / **MAJOR** bumps: *Actions → Release → Run workflow* and choose the bump type.

## Layout

| Path | Purpose |
|------|---------|
| [`chatgpt/`](chatgpt/) | Custom Instructions (**copy into settings**) + checklist |
| [`claude/`](claude/) | Project instructions (**copy**) + Claude Code notes; optional `CLAUDE.md` (**files**) |
| [`cursor/`](cursor/) | User Rules (**copy**) + `.cursor/rules/` and `.cursorignore` (**files**) |

## How to use

1. **ChatGPT** — *copy into settings:* [`chatgpt/README.md`](chatgpt/README.md) → [`custom-instructions.md`](chatgpt/custom-instructions.md) into Custom Instructions.
2. **Claude (web)** — *copy into settings:* [`claude/README.md`](claude/README.md) → [`project-instructions.md`](claude/project-instructions.md) into Project instructions.
3. **Cursor** — *copy into settings first:* [`cursor/user-rules.md`](cursor/user-rules.md) into Cursor Settings → Rules; *then optionally save files:* [`cursor/README.md`](cursor/README.md) → copy `cursor/.cursor` and `.cursorignore` into your repo.

**Nine shared security rules** in ChatGPT, Claude (web), Cursor User Rules, and `cursor/.cursor/rules/security-vibe-coding.mdc`. Each tool’s README labels what is **copy into settings** vs **save files**.

## Czech vs English paths

| Topic | Czech templates | English templates |
|-------|-----------------|-------------------|
| Root docs | [Czech section](#cesky) | [English section](#english) |
| ChatGPT | [`chatgpt/`](chatgpt/) | [`en/chatgpt/`](en/chatgpt/) |
| Claude | [`claude/`](claude/) | [`en/claude/`](en/claude/) |
| Cursor | [`cursor/`](cursor/) | [`en/cursor/`](en/cursor/) |

## Freshness and links

Best practices and product UIs change. This pack reflects **May 2026**; verify current settings with each vendor:

- [Cursor — Rules](https://docs.cursor.com/context/rules)
- [OpenAI — Security](https://openai.com/security)
- [Anthropic — Claude Code security](https://docs.anthropic.com/en/docs/claude-code/security)
- Inspiration for part of the rules: community thread [Mnilax](https://x.com/mnilax/status/2053116311132155938) (agentic vibe coding), adapted for all three tools in this repo

---

<a id="cesky"></a>

## Česky

**English:** [back to English](#english) · [Releases](https://github.com/sodomak/promptpunk/releases) · [Stáhnout latest](https://github.com/sodomak/promptpunk/releases/latest)

Bezpečnostní šablony pro vibe coding (ChatGPT, Claude, Cursor).

Materiál z přednášky **CryptoByte** — zkopírujte si do vlastního projektu nebo účtu jen to, co používáte.

Při úpravách držte český a anglický strom šablon v souladu (stejné názvy souborů).

## Release a verzování

| Co | Kde |
|----|-----|
| Všechny release | [github.com/sodomak/promptpunk/releases](https://github.com/sodomak/promptpunk/releases) |
| Nejnovější ke stažení | […/releases/latest](https://github.com/sodomak/promptpunk/releases/latest) |
| Verze v repu | [`VERSION`](VERSION) |

**SemVer:** změna souborů v `chatgpt/`, `claude/`, `cursor/` nebo `en/` na větvi `main` spustí automatický **PATCH** release (tag `vX.Y.Z` + GitHub Release se zdrojovými archivy). **MINOR** / **MAJOR**: *Actions → Release → Run workflow* a zvolte typ bumpu.

## Struktura

| Složka / soubor | Účel |
|-----------------|------|
| [`chatgpt/`](chatgpt/) | Custom Instructions (**kopírovat do nastavení**) + checklist |
| [`claude/`](claude/) | Project instructions (**kopírovat**) + Claude Code; volitelně `CLAUDE.md` (**soubory**) |
| [`cursor/`](cursor/) | User Rules (**kopírovat**) + `.cursor/rules/` a `.cursorignore` (**soubory**) |

## Jak to použít

1. **ChatGPT** — *kopírovat do nastavení:* [`chatgpt/README.md`](chatgpt/README.md) → [`custom-instructions.md`](chatgpt/custom-instructions.md) do Custom Instructions.
2. **Claude (web)** — *kopírovat do nastavení:* [`claude/README.md`](claude/README.md) → [`project-instructions.md`](claude/project-instructions.md) do Project instructions.
3. **Cursor** — *nejdřív kopírovat do nastavení:* [`cursor/user-rules.md`](cursor/user-rules.md) do Cursor Settings → Rules; *pak volitelně uložit soubory:* [`cursor/README.md`](cursor/README.md) → složka `cursor/.cursor` a `.cursorignore` do vašeho repa.

**Devět společných bezpečnostních pravidel** u ChatGPT, Claude (web), Cursor User Rules a v `cursor/.cursor/rules/security-vibe-coding.mdc`. V README každého nástroje je uvedeno, co jde **do nastavení** a co **do souborů**.

## Cesty CZ vs EN

| Téma | České šablony | Anglické šablony |
|------|---------------|------------------|
| Dokumentace | [tato sekce](#cesky) | [anglická část](#english) |
| ChatGPT | [`chatgpt/`](chatgpt/) | [`en/chatgpt/`](en/chatgpt/) |
| Claude | [`claude/`](claude/) | [`en/claude/`](en/claude/) |
| Cursor | [`cursor/`](cursor/) | [`en/cursor/`](en/cursor/) |

## Platnost a odkazy

Doporučené postupy a UI se mění. Materiál je psán s ohledem na stav k **květnu 2026**; ověřte si aktuální volby u poskytovatele:

- [Cursor — Rules](https://docs.cursor.com/context/rules)
- [OpenAI — Security](https://openai.com/security)
- [Anthropic — Claude Code security](https://docs.anthropic.com/en/docs/claude-code/security)
- Inspirace části pravidel: komunitní vlákno [Mnilax](https://x.com/mnilax/status/2053116311132155938) (agentní vibe coding), přepracováno pro všechny tři nástroje v tomto repu
