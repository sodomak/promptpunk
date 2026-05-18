# ChatGPT

## Co je v této složce

| Soubor | Typ nasazení | Kam / co udělat |
|--------|----------------|-----------------|
| [`custom-instructions.md`](custom-instructions.md) | **Kopírovat do nastavení** | ChatGPT → **Settings** → **Personalization** → **Custom instructions** (druhé pole) |
| Tento README (checklist níže) | **Jen přečíst** | Kontrola před odesláním promptu |

V této složce **nejsou soubory** k uložení do projektu — pravidla žijí v nastavení účtu ChatGPT.

## Kopírovat do nastavení

1. Otevřete ChatGPT → **Nastavení** (Settings).
2. **Personalization** → **Custom instructions**.
3. Do pole **„How would you like ChatGPT to respond?“** (druhé pole; název se může lišit) vložte **celý kódový blok** ze souboru [`custom-instructions.md`](custom-instructions.md).
4. První pole („What would you like ChatGPT to know about you?“) **nepište citlivé údaje** — neutrální role stačí (např. „softwarový vývojář, preferuji stručné odpovědi“).

Text z repa se **neukládá automaticky** — musíte ho vložit ručně v prohlížeči.

Oficiální nápověda: [Custom instructions for ChatGPT](https://help.openai.com/en/articles/8096356-custom-instructions-for-chatgpt).

## Účet a data

- Pro **vlastní kód a interní dokumenty** zvažte firemní / placený režim s jasnými podmínkami zpracování dat (např. ChatGPT Enterprise), pokud to vaše organizace vyžaduje.
- V nastavení zkontrolujte **volby soukromí a učení modelu** (názvy se liší podle produktu).

## Rychlý checklist před odesláním promptu

- [ ] V promptu nejsou hesla, API klíče, privátní klíče, connection stringy.
- [ ] Neposílám celé dumpy produkční databáze ani kompletní logy s osobními údaji (jména, e-maily, telefony, adresy zákazníků apod.).
- [ ] Pokud vkládám kód, je to **minimalizovaný reprodukční příklad**, ne celý monolit.
- [ ] Výstup z modelu **projdu** před nasazením; neočekávám „bezchybnou“ bezpečnost.
