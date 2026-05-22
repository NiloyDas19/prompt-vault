---
title: "Credential Exposure & Leakage Scanner"
category: Coding & Development
subcategory: Security & AI Guardrails
tags: [security, credentials, secrets, scanning, leak-prevention]
model: any
---

## Purpose
A codebase scanner prompt designed to detect hardcoded credentials, API keys, passwords, and private tokens within code, proposing secure environment-variable-based refactoring.

## Prompt
```markdown
Analyze the following code snippet or configuration file for exposed credentials, hardcoded secrets, API keys, private keys, or sensitive configuration details.

<code_to_scan>
{CODE_TO_SCAN}
</code_to_scan>

Please perform a comprehensive credential scan:

1. **Exposed Secret Detection**: Identify any hardcoded strings that appear to be:
   - API Keys or Tokens (e.g., Bearer tokens, Stripe keys, AWS access keys, GitHub tokens, Slack Webhooks)
   - Database Connection Strings containing passwords or usernames
   - Private Cryptographic Keys (e.g., RSA, Elliptic Curve, SSL certificates)
   - Plaintext passwords, SSH keys, or administrative credentials
2. **Confidence Level**: Rate the likelihood that the detected string is an active/real credential (versus a placeholder, test key, or public identifier):
   - **CONFIRMED LEAK**: High confidence (looks like a real key/hash with high entropy)
   - **SUSPECTED LEAK**: Medium confidence (needs verification, standard format but might be expired or local test creds)
   - **FALSE POSITIVE / PLACEHOLDER**: Low confidence (explicitly labeled like "your-key-here" or local fallback config)
3. **Location**: Specify the exact line number and variable name where the secret is declared.
4. **Refactoring Code (Hardening)**: Provide the refactored code that:
   - Removes the hardcoded secret entirely.
   - Replaces it with a secure loading mechanism using environment variables, system environment configurations, or a secure secrets manager (e.g., AWS Secrets Manager, Vault, `.env` files).
   - Shows the exact key-value configuration that should be added to the `.env.template` file.

Structure your response with:
- **Scan Summary Table** (Exposed Secret, Variable Name, Confidence, Severity)
- **Refactoring Solution** (How to secure the code)
- **Recommended `.env.template` Additions**
```

## Variables
- `{CODE_TO_SCAN}` – The source code, configuration files, or script templates you want to audit for credential leaks.

## Notes
- 🔑 **Shift Left Security**: Excellent for running on staged files in a Git hook before committing code to public or shared repositories.
- 💡 **Entropy and Formats**: Remind the developer that modern secrets scanning looks for specific high-entropy string patterns and common API key prefixes (like `sk_live_`, `AIzaSy`).
- 🤖 **Agent Integration**: If an AI agent has the ability to read files, run this scanner first to ensure no credentials are accidentally fed into the LLM context.
