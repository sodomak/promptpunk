# Claude Code — short hardening checklist

## Permissions

- Where it fits your workflow, prefer **deny-by-default** in permission settings: block destructive commands and writes outside the working tree when possible.
- Read the command preview before approving — **prompt social engineering** may try to bypass your rules.

Read more: [Configure permissions](https://docs.anthropic.com/en/docs/claude-code/permissions).

## Memory and files

- **`CLAUDE.md`** (and similar) often ends up in git. **Do not** put real keys, internal URLs with tokens, customer names, or other sensitive data in it.
- For local notes with more sensitive content, keep them in **`.gitignore`d** files and agree a convention with your team.

Read more: [How Claude remembers your project](https://docs.anthropic.com/en/docs/claude-code/memory).

## Network and shell

- Before running scripts that download from the internet (`curl`, installers), verify **source and hash**; supply-chain attacks target developers too.
- Do not pass untrusted raw text into the shell.

## Summary

| Area | Recommendation |
|------|----------------|
| Secrets | Env / vault only; no leaks into the repo |
| Approvals | A slow “yes” beats a fast incident |
| Repo | `git diff` before commit; code review for AI-driven changes |

Official overview: [Claude Code — Security](https://docs.anthropic.com/en/docs/claude-code/security).
