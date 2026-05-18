# Cursor

## Co je v této složce

| Soubor / složka | Typ nasazení | Kam / co udělat |
|-----------------|----------------|-----------------|
| [`user-rules.md`](user-rules.md) | **Kopírovat do nastavení** | **Cursor Settings → Rules** (globálně, všechny projekty) |
| [`.cursor/`](.cursor/) (složka `rules/*.mdc`) | **Uložit soubory** | Zkopírovat do **`váš-repo/.cursor/`** (vedle `package.json`, `go.mod`, …) |
| [`.cursorignore.example`](.cursorignore.example) | **Uložit soubory** | Zkopírovat / sloučit jako **`váš-repo/.cursorignore`** |
| Tento README (MCP, soukromí, checklist) | **Jen přečíst** | Doplňkové nastavení editoru |

**Doporučené pořadí:** nejdřív User Rules (jednou na počítači), pak volitelně projektové soubory (pro tým a git).

| | User Rules | Projekt `.cursor/rules/` |
|--|------------|---------------------------|
| Kde | Nastavení Cursoru | Kořen vašeho repozitáře |
| Git / tým | Ne | Ano |
| Kdy | Výchozí ve všech repozitářích | Stack-specifické pravidla + sdílení |

Při konfliktu má **projektové** pravidlo přednost před User Rules. User Rules platí pro **Agent (chat)**, ne pro Tab ani Inline Edit (Ctrl+K).

Dokumentace: [Cursor — Rules](https://cursor.com/docs/context/rules).

## Kopírovat do nastavení

1. Otevřete **Cursor Settings** (ikona ozubeného kola nebo *File → Preferences → Cursor Settings*).
2. Sekce **Rules** (někdy **Rules, Commands** nebo *Rules for AI*).
3. Do pole **User Rules** vložte **celý kódový blok** ze souboru [`user-rules.md`](user-rules.md).

Text se **neukládá z gitu sám** — vložíte ho jednou do nastavení Cursoru na tomto počítači.

## Uložit soubory do projektu

1. Zkopírujte celou složku **`.cursor`** z této složky repa promptpunk do **kořene** vašeho softwarového repozitáře → výsledek `váš-repo/.cursor/rules/*.mdc`.
2. Soubor **`.cursorignore.example`** zkopírujte do kořene projektu jako **`.cursorignore`** (nebo slučte vzory se stávajícím souborem). Cursor pak při indexaci **vynechá** uvedené cesty.

V `.cursor/rules/` jsou mimo jiné:

- `security-vibe-coding.mdc` — stejných 9 principů jako v `user-rules.md` (pro Agent v tomto projektu).
- `secrets-and-data.mdc` — přísnější pravidla u `.env`, Terraform, CI, Helm (jen při práci s těmito soubory).

## Pravidla vs. starý `.cursorrules`

- **Doporučený formát:** `.cursor/rules/*.mdc` (YAML frontmatter).
- Soubor **`.cursorrules`** v kořeni je **zastaralý** — v tomto handoutu nepoužíváme.

## Nastavení soukromí

- Zapněte režim odpovídající vašim požadavkům na **odesílání kódu** k modelu (v UI se objevuje např. *Privacy Mode* — ověřte v aktuální verzi).
- **Aktualizujte** editor průběžně.

## MCP (Model Context Protocol)

- Zapínejte jen **MCP servery, kterým důvěřujete**.
- Konfiguraci MCP nekopírujte slepě z internetu a necommitujte tajemství.

## Kontrolní seznam

- [ ] **User Rules** nastavené z [`user-rules.md`](user-rules.md).
- [ ] (Volitelně) `.cursor/rules/` v gitu bez tajemství.
- [ ] `.cursorignore` pokrývá `.env*`, klíče, zálohy.
- [ ] Před mergem AI změn proběhne **lidský review** a CI.
