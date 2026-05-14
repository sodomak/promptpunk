# Cursor — nasazení šablony do vlastního projektu

## Co zkopírovat

1. Zkopírujte celou složku **`.cursor`** z tohoto adresáře do **kořene** svého softwarového repozitáře (vedle `package.json`, `go.mod` apod.).
2. Soubor **`.cursorignore.example`** zkopírujte do kořene projektu jako **`.cursorignore`** (nebo slučte řádky se stávajícím souborem). Cursor pak při indexaci kontextu **vynechá** uvedené cesty — snižuje riziko náhodného „naleptání“ tajemství do promptu.

## Pravidla vs. starý `.cursorrules`

- **Doporučený formát:** projektová pravidla v **`.cursor/rules/*.mdc`** (YAML frontmatter, viz soubory v tomto balíčku).
- Soubor **`.cursorrules`** v kořeni je **zastarávající varianta**; pro účastníky přednášky držíme jeden kanonický způsob právě přes `.cursor/rules/`.

Dokumentace: [Cursor — Rules](https://docs.cursor.com/context/rules).

## Nastavení soukromí

- V nastavení Cursoru zapněte režim, který odpovídá vašim požadavkům na **odesílání kódu** k modelu (historicky označovaný jako např. *Privacy Mode* — název v UI ověřte v aktuální verzi).
- **Aktualizujte** editor průběžně; bezpečnostní opravy se týkají i kanálu MCP a konfigurace.

## MCP (Model Context Protocol)

- Zapínejte jen **MCP servery, kterým důvěřujete**; čtěte, jaké nástroje server registruje (síť, souborový systém).
- Konfigurace MCP je citlivé místo — nekopírujte ji slepě z internetu a nenechávejte v repu tajemství.

## Kontrolní seznam

- [ ] `.cursor/rules/` je v gitu (sdílený tým), ale bez tajemství.
- [ ] `.cursorignore` pokrývá `.env*`, klíče, zálohy, velké binárky.
- [ ] Před mergem AI změn proběhne **lidský review** a CI.
