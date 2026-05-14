# ChatGPT — where to paste the template

## Step 1: Custom Instructions

1. Open ChatGPT → **Settings**.
2. **Personalization** → **Custom instructions** (wording may vary by product tier).
3. Paste the contents of [`custom-instructions.md`](custom-instructions.md) into the field **“How would you like ChatGPT to respond?”** (or the equivalent second field in your UI).
4. In the first field (“What would you like ChatGPT to know about you?”) **do not put sensitive data** — keep a neutral role (e.g. “software engineer, prefer concise answers”).

Official help: [Custom instructions for ChatGPT](https://help.openai.com/en/articles/8096356-custom-instructions-for-chatgpt).

## Step 2: Account and data

- For **proprietary code and internal documents**, consider a business / paid tier with clear data-processing terms (e.g. ChatGPT Enterprise) if your organisation requires it.
- Review **privacy and model improvement** settings in the product (names differ by SKU and region).

## Quick checklist before sending a prompt

- [ ] No passwords, API keys, private keys, or connection strings in the prompt.
- [ ] No full production DB dumps or complete logs with personal data (names, emails, phone numbers, customer addresses, etc.).
- [ ] If I paste code, it is a **minimal repro**, not the whole monolith.
- [ ] I will **review** model output before shipping; I do not assume “secure by default.”
