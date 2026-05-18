# Cursor — User Rules (global)

**Deployment type:** copy into settings (not stored in git). Paste the text into **Cursor Settings → Rules** (in some versions *Rules, Commands* or *Rules for AI*). Applies to **Agent (chat)** in all projects; not Tab or Inline Edit (Ctrl+K).

Steps: see [`README.md`](README.md). Optional project rules (files in the repo) live under [`.cursor/`](.cursor/).

> Copy **the entire fenced block** below into the User Rules field in Cursor settings.

## Template (9 principles)

```text
Code and data security when generating and editing:

- Secrets: Never store or suggest API keys, passwords, private keys, OAuth tokens, or connection strings with embedded passwords. Use environment variables, a secret manager, or templates with placeholders (YOUR_SECRET_HERE as literal text only, never a real value).
- Sensitive data: Do not log or repeat personal or other sensitive data unnecessarily; anonymise in examples.
- Secure code: Input validation, parameterised queries, CSRF where applicable, HTTPS, least privilege. Critical controls (policy, permissions) as code, not vague “be careful” wording. No deliberately vulnerable examples without warning.
- Infra and config: For Terraform, Helm values, CI YAML, docker-compose — no secrets in commits; vault / placeholders. Private-by-default networking, TLS, least privilege for IAM and DB roles.
- Dependencies: Do not add random packages; pin versions; mention supply-chain risk.
- Review and checkpoints: Write small, reviewable diffs; assume review and CI. For multi-step security-sensitive work, summarise done / verified / remaining. Ask when context is missing (auth, threat model).
- Honesty about status: Do not claim done if a test, migration, or step was skipped — state what was not verified.
- Context before change: Before editing auth, authorisation, encryption, or validation, read the related code.
- One pattern, surgical diffs: Do not mix two competing security approaches; change only necessary lines; do not break neighbouring protections with opportunistic refactors.
```

Same nine principles as [`chatgpt/custom-instructions.md`](../chatgpt/custom-instructions.md) and [`claude/project-instructions.md`](../claude/project-instructions.md).
