# ChatGPT — kam vložit šablonu

## Krok 1: Custom Instructions

1. Otevřete ChatGPT → **Nastavení** (Settings).
2. Sekce **Personalization** → **Custom instructions** (Custom instructions for ChatGPT).
3. Do pole pro **„How would you like ChatGPT to respond?“** (nebo obdobného druhého pole podle verze UI) vložte obsah souboru [`custom-instructions.md`](custom-instructions.md).
4. První pole („What would you like ChatGPT to know about you?“) **nepište citlivé údaje** — držte se neutrální role (např. „softwarový vývojář, preferuji stručné odpovědi“).

Oficiální nápověda: [Custom instructions for ChatGPT](https://help.openai.com/en/articles/8096356-custom-instructions-for-chatgpt).

## Krok 2: Účet a data

- Pro práci s **vlastním kódem a interními dokumenty** zvažte firemní / placený režim s jasnými podmínkami zpracování dat (např. ChatGPT Enterprise), pokud to vaše organizace vyžaduje.
- V nastavení zkontrolujte **volby soukromí a učení modelu** (historické názvy se liší podle produktu).

## Rychlý checklist před odesláním promptu

- [ ] V promptu nejsou hesla, API klíče, privátní klíče, connection stringy.
- [ ] Neposílám celé dumpy produkční databáze ani kompletní logy s osobními údaji (jména, e-maily, telefony, adresy zákazníků apod.).
- [ ] Pokud vkládám kód, je to **minimalizovaný reprodukční příklad**, ne celý monolit.
- [ ] Výstup z modelu **projdu** před nasazením; neočekávám „bezchybnou“ bezpečnost.
