# Claude Code — zkrácený hardening checklist

## Oprávnění

- V nastavení permissions používejte **deny-by-default** tam, kde to dává smysl: blokujte destruktivní příkazy a zápis mimo pracovní strom, pokud to váš workflow dovoluje.
- Čtěte náhled příkazu před schválením — **social engineering v promptu** může zkoušet obejít vaše pravidla.

Čtení: [Configure permissions](https://docs.anthropic.com/en/docs/claude-code/permissions).

## Paměť a soubory

- Soubor **`CLAUDE.md`** (a podobné) často končí v gitu. **Nepište do něj** reálné klíče, interní URL s tokeny, jména zákazníků ani jiné citlivosti.
- Pokud potřebujete lokální poznámky s citlivějším obsahem, držte je v souborech **v `.gitignore`** a v týmu si ujasněte konvenci.

Čtení: [How Claude remembers your project](https://docs.anthropic.com/en/docs/claude-code/memory).

## Síť a bash

- Před spuštěním skriptů stahujících obsah z internetu (`curl`, instalátory) zkontrolujte **zdroj a hash**; supply chain útoky cílí i na vývojáře.
- Nepředávejte do shellu neošetřený text z nedůvěryhodných vstupů.

## Shrnutí

| Oblast | Doporučení |
|--------|------------|
| Tajemství | Pouze env / vault; žádné leaky do repa |
| Schvalování | Pomalé „ano“ je lepší než rychlý incident |
| Repo | `git diff` před commitem; code review pro AI změny |

Oficiální přehled: [Claude Code — Security](https://docs.anthropic.com/en/docs/claude-code/security).
