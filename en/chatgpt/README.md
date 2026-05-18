# ChatGPT

## What is in this folder

| File | Deployment type | Where / what to do |
|------|-----------------|-------------------|
| [`custom-instructions.md`](custom-instructions.md) | **Copy into settings** | ChatGPT → **Settings** → **Personalization** → **Custom instructions** (second field) |
| This README (checklist below) | **Read only** | Pre-prompt checklist |

There are **no files** here to save into a project — rules live in your ChatGPT account settings.

## Copy into settings

1. Open ChatGPT → **Settings**.
2. **Personalization** → **Custom instructions**.
3. Paste **the entire fenced block** from [`custom-instructions.md`](custom-instructions.md) into **“How would you like ChatGPT to respond?”** (or the equivalent second field).
4. In the first field (“What would you like ChatGPT to know about you?”) **do not put sensitive data** — a neutral role is enough (e.g. “software engineer, prefer concise answers”).

Text from this repo is **not saved automatically** — you paste it manually in the browser.

Official help: [Custom instructions for ChatGPT](https://help.openai.com/en/articles/8096356-custom-instructions-for-chatgpt).

## Account and data

- For **proprietary code and internal documents**, consider a business / paid tier with clear data-processing terms (e.g. ChatGPT Enterprise) if your organisation requires it.
- Review **privacy and model improvement** settings in the product (names differ by SKU and region).

## Quick checklist before sending a prompt

- [ ] No passwords, API keys, private keys, or connection strings in the prompt.
- [ ] No full production DB dumps or complete logs with personal data (names, emails, phone numbers, customer addresses, etc.).
- [ ] If I paste code, it is a **minimal repro**, not the whole monolith.
- [ ] I will **review** model output before shipping; I do not assume “secure by default.”
