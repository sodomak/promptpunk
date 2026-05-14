# Claude — dva různé kontexty

## 1) Claude.ai (prohlížeč) — Projects

Projekt v Claude má vlastní **Project instructions** a často i nahrané soubory. Postup:

1. Vytvořte **Project** a do instrukcí vložte **obsah kódového bloku** ze souboru [`project-instructions.md`](project-instructions.md) (zkopírujte celý blok najednou).
2. Do projektu **nenahrávejte** `.env`, produkční exporty, smlouvy s osobními údaji ani interní dokumenty, které nesmí opustit perimetr firmy, pokud k tomu nemáte souhlas a správný typ účtu.

## 2) Claude Code (terminál / IDE)

Claude Code má vlastní model oprávnění, paměť (`CLAUDE.md`) a bezpečnostní dokumentaci od Anthropic. Přečtěte si:

- [`claude-code-hardening.md`](claude-code-hardening.md) v tomto repozitáři (stručný checklist).
- Oficiální dokumentaci: [Claude Code — Security](https://docs.anthropic.com/en/docs/claude-code/security), [Permissions](https://docs.anthropic.com/en/docs/claude-code/permissions), [Memory](https://docs.anthropic.com/en/docs/claude-code/memory).

## Společné pravidlo

**Citlivosti nepatří do gitu** — ani do sdíleného `CLAUDE.md`, README s příklady connection stringů apod. Používejte lokální soubory ignorované gitem (a týmem dohodnutý postup).
