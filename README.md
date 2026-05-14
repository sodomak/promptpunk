# promptpunk

Bezpečnostní šablony pro vibe coding (ChatGPT, Claude, Cursor).

Materiál z přednášky **CryptoByte** — zkopírujte si do vlastního projektu nebo účtu jen to, co používáte.

## English / Anglicky

Kompletní anglický mirror stejné struktury: **[`en/README.md`](en/README.md)**. Při úpravách držte CZ a EN stromy v souladu (stejné názvy souborů).

| Téma | Česky | English |
|------|-------|---------|
| Kořen | [`README.md`](README.md) (tato stránka) | [`en/README.md`](en/README.md) |
| ChatGPT | [`chatgpt/`](chatgpt/) | [`en/chatgpt/`](en/chatgpt/) |
| Claude | [`claude/`](claude/) | [`en/claude/`](en/claude/) |
| Cursor | [`cursor/`](cursor/) | [`en/cursor/`](en/cursor/) |

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

**ChatGPT a Claude (web):** šablony v [`chatgpt/custom-instructions.md`](chatgpt/custom-instructions.md) a [`claude/project-instructions.md`](claude/project-instructions.md) mají **shodných šest pravidel** (včetně konkrétní zmínky Terraform, Helm, CI, Docker); liší se jen úvodní věta podle toho, jestli píšete Custom Instructions nebo Project instructions.

## Platnost a odkazy

Doporučené postupy a UI se mění. Materiál je psán s ohledem na stav k **květnu 2026**; ověřte si aktuální volby u poskytovatele:

- [Cursor — Rules](https://docs.cursor.com/context/rules)
- [OpenAI — Security](https://openai.com/security)
- [Anthropic — Claude Code security](https://docs.anthropic.com/en/docs/claude-code/security)
