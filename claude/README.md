# Claude

## Co je v této složce

| Soubor | Typ nasazení | Kam / co udělat |
|--------|----------------|-----------------|
| [`project-instructions.md`](project-instructions.md) | **Kopírovat do nastavení** | Claude.ai → **Project** → pole **Instructions** |
| [`claude-code-hardening.md`](claude-code-hardening.md) | **Jen přečíst** | Checklist pro Claude Code (oprávnění, paměť, bash) |
| (volitelně) stejný text jako v `project-instructions.md` | **Uložit soubory** | Soubor `CLAUDE.md` v **kořeni** repozitáře, pokud používáte **Claude Code** v terminálu |

## Kopírovat do nastavení (Claude.ai — Projects)

1. V Claude.ai vytvořte **Project**.
2. Do **Project instructions** vložte **celý kódový blok** ze souboru [`project-instructions.md`](project-instructions.md).
3. Do projektu **nenahrávejte** `.env`, produkční exporty, smlouvy s osobními údaji ani interní dokumenty, které nesmí opustit perimetr firmy (pokud k tomu nemáte souhlas a správný typ účtu).

Text z repa se **neukládá automaticky** — vložíte ho v UI projektu.

## Uložit soubory (volitelně — Claude Code)

Pokud používáte **Claude Code** v terminálu / IDE:

- Můžete zkopírovat obsah code bloku z [`project-instructions.md`](project-instructions.md) do souboru **`CLAUDE.md`** v kořeni vašeho softwarového repozitáře (stejných 9 pravidel).
- **Nepište** do `CLAUDE.md` reálná tajemství — soubor často končí v gitu.

## Claude Code — jen přečíst

Claude Code má vlastní oprávnění, paměť a bash. Přečtěte:

- [`claude-code-hardening.md`](claude-code-hardening.md) (checklist v tomto repu).
- [Claude Code — Security](https://docs.anthropic.com/en/docs/claude-code/security), [Permissions](https://docs.anthropic.com/en/docs/claude-code/permissions), [Memory](https://docs.anthropic.com/en/docs/claude-code/memory).

Stejných **devět bezpečnostních pravidel** platí jako u ChatGPT a Cursoru v repu promptpunk.

## Společné pravidlo

**Citlivosti nepatří do gitu** — ani do sdíleného `CLAUDE.md`, ani do README s reálnými connection stringy.
