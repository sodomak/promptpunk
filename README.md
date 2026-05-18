# promptpunk

[![Latest release](https://img.shields.io/github/v/release/sodomak/promptpunk?label=release)](https://github.com/sodomak/promptpunk/releases/latest)

**Česky:** [přejít na českou verzi](#cesky) · [All releases](https://github.com/sodomak/promptpunk/releases) · [Download latest](https://github.com/sodomak/promptpunk/releases/latest)

---

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
| [`chatgpt/`](chatgpt/) | Custom Instructions and checklist for ChatGPT |
| [`claude/`](claude/) | Claude Projects instructions + Claude Code notes |
| [`cursor/`](cursor/) | `.cursor/rules/` templates and `.cursorignore` example |

## How to use

1. **ChatGPT:** open [`chatgpt/README.md`](chatgpt/README.md), copy the **entire fenced block** from [`chatgpt/custom-instructions.md`](chatgpt/custom-instructions.md) into Custom Instructions.
2. **Claude (web):** new Project → paste the **entire fenced block** from [`claude/project-instructions.md`](claude/project-instructions.md) into instructions.
3. **Cursor:** copy `cursor/.cursor` to your repo root and copy or merge `cursor/.cursorignore.example` as `.cursorignore`. Details in [`cursor/README.md`](cursor/README.md).

**ChatGPT and Claude (web):** the templates in [`chatgpt/custom-instructions.md`](chatgpt/custom-instructions.md) and [`claude/project-instructions.md`](claude/project-instructions.md) share the **same nine rules**; only the opening line differs (Custom Instructions vs Project instructions). **Cursor:** the same nine principles in [`cursor/.cursor/rules/security-vibe-coding.mdc`](cursor/.cursor/rules/security-vibe-coding.mdc).

## Czech vs English paths

| Topic | Czech templates | English templates |
|-------|-----------------|-------------------|
| Root docs | [`README.md#cesky`](README.md#cesky) | this page (top) |
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

## Česky {#cesky}

**English:** [back to top](#promptpunk) · [Releases](https://github.com/sodomak/promptpunk/releases) · [Stáhnout latest](https://github.com/sodomak/promptpunk/releases/latest)

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
| [`chatgpt/`](chatgpt/) | Custom Instructions a checklist pro ChatGPT |
| [`claude/`](claude/) | Instrukce pro Claude Projects + poznámky k Claude Code |
| [`cursor/`](cursor/) | Pravidla `.cursor/rules/`, vzor `.cursorignore` |

## Jak to použít

1. **ChatGPT:** otevřete [`chatgpt/README.md`](chatgpt/README.md), zkopírujte **celý kódový blok** z [`chatgpt/custom-instructions.md`](chatgpt/custom-instructions.md) a vložte ho do nastavení Custom Instructions.
2. **Claude (web):** nový Project → do Instructions vložte **celý kódový blok** z [`claude/project-instructions.md`](claude/project-instructions.md).
3. **Cursor:** zkopírujte obsah složky `cursor/.cursor` do kořene vlastního repozitáře a `cursor/.cursorignore.example` přejmenujte na `.cursorignore` (nebo slučte vzory). Detaily v [`cursor/README.md`](cursor/README.md).

**ChatGPT a Claude (web):** šablony v [`chatgpt/custom-instructions.md`](chatgpt/custom-instructions.md) a [`claude/project-instructions.md`](claude/project-instructions.md) mají **shodných devět pravidel**; liší se jen úvodní věta (Custom Instructions vs. Project instructions). **Cursor:** stejných devět principů v [`cursor/.cursor/rules/security-vibe-coding.mdc`](cursor/.cursor/rules/security-vibe-coding.mdc).

## Cesty CZ vs EN

| Téma | České šablony | Anglické šablony |
|------|---------------|------------------|
| Dokumentace | [`README.md#cesky`](README.md#cesky) | [horní část](#promptpunk) |
| ChatGPT | [`chatgpt/`](chatgpt/) | [`en/chatgpt/`](en/chatgpt/) |
| Claude | [`claude/`](claude/) | [`en/claude/`](en/claude/) |
| Cursor | [`cursor/`](cursor/) | [`en/cursor/`](en/cursor/) |

## Platnost a odkazy

Doporučené postupy a UI se mění. Materiál je psán s ohledem na stav k **květnu 2026**; ověřte si aktuální volby u poskytovatele:

- [Cursor — Rules](https://docs.cursor.com/context/rules)
- [OpenAI — Security](https://openai.com/security)
- [Anthropic — Claude Code security](https://docs.anthropic.com/en/docs/claude-code/security)
- Inspirace části pravidel: komunitní vlákno [Mnilax](https://x.com/mnilax/status/2053116311132155938) (agentní vibe coding), přepracováno pro všechny tři nástroje v tomto repu
