# Bezpečnostní šablony pro vibe coding (ChatGPT, Claude, Cursor)

Materiál z přednášky **CryptoByte / promptpunk** — zkopírujte si do vlastního projektu nebo účtu jen to, co používáte.

## Struktura

| Složka / soubor | Účel |
|-----------------|------|
| [`chatgpt/`](chatgpt/) | Custom Instructions a checklist pro ChatGPT |
| [`claude/`](claude/) | Instrukce pro Claude Projects + poznámky k Claude Code |
| [`cursor/`](cursor/) | Pravidla `.cursor/rules/`, vzor `.cursorignore` |

## Jak to použít

1. **ChatGPT:** otevřete [`chatgpt/README.md`](chatgpt/README.md), vložte text z `custom-instructions.md` do nastavení Custom Instructions.
2. **Claude (web):** nový Project → Instructions podle [`claude/project-instructions.md`](claude/project-instructions.md).
3. **Cursor:** zkopírujte obsah složky `cursor/.cursor` do kořene vlastního repozitáře a `cursor/.cursorignore.example` přejmenujte na `.cursorignore` (nebo slučte vzory). Detaily v [`cursor/README.md`](cursor/README.md).

## Platnost a odkazy

Doporučené postupy a UI se mění. Materiál je psán s ohledem na stav k **květnu 2026**; ověřte si aktuální volby u poskytovatele:

- [Cursor — Rules](https://docs.cursor.com/context/rules)
- [OpenAI — Security](https://openai.com/security)
- [Anthropic — Claude Code security](https://docs.anthropic.com/en/docs/claude-code/security)

## Disclaimer

Tyto soubory **nejsou právní ani bezpečnostní audit**, nenahrazují firemní DLP, smluvní režim s dodavatelem modelu ani školení vaší organizace. Používáte je na vlastní zodpovědnost.
