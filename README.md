# 🔐 Prompt Vault

> **The largest open-source AI prompt library on GitHub.**
> Curated, structured, and ready-to-use prompts for ChatGPT, Claude, Gemini, and any capable LLM.

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Prompts](https://img.shields.io/badge/Prompts-240%2B-blue)](./coding-development/)
[![Categories](https://img.shields.io/badge/Categories-10-green)](./coding-development/)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](CONTRIBUTING.md)

---

## 📖 What is Prompt Vault?

Prompt Vault is a structured, community-maintained library of high-quality AI prompts organized by category and subcategory. Every prompt is:

- ✅ **Rewritten & improved** — Not copied verbatim from any source
- ✅ **Structured with variables** — Use `{CURLY_BRACES}` to fill in your specifics
- ✅ **Model-agnostic** — Works with ChatGPT, Claude, Gemini, and more
- ✅ **Production-tested** — Curated for real tasks, not toy examples
- ✅ **Consistently formatted** — Easy to browse, copy, and use

---

## 📂 Categories

| # | Category | Prompts | Status |
|---|---|---|---|
| 1 | [💻 Coding & Development](./coding-development/) | 15 | ✅ Available |
| 2 | [🤖 Claude Skills](./claude-skills/) | 36 | ✅ Available |
| 3 | [🎨 Image Generation](./image-generation/) | 108 | ✅ Available |
| 4 | [📣 Marketing & Sales](./marketing-sales/) | 81 | ✅ Available |
| 5 | ✍️ Writing | — | 🔜 Coming Soon |
| 6 | 🗂️ Productivity & Planning | — | 🔜 Coming Soon |
| 7 | 🔬 Research & Analysis | — | 🔜 Coming Soon |
| 8 | 🎓 Education & Learning | — | 🔜 Coming Soon |
| 9 | 💼 Business & Strategy | — | 🔜 Coming Soon |
| 10 | 🔎 SEO & Content | — | 🔜 Coming Soon |
| 11 | 📊 Data & Analytics | — | 🔜 Coming Soon |

---

## 🚀 Getting Started

**Browse prompts** directly on GitHub, or clone the repo for local access:

```bash
git clone https://github.com/NiloyDas19/prompt-vault.git
cd prompt-vault
```

**Use a prompt:**
1. Navigate to the category folder (e.g., `coding-development/debugging/`)
2. Open the prompt file
3. Copy the **Prompt** section
4. Replace all `{VARIABLE}` placeholders with your specifics
5. Paste into your preferred AI assistant

---

## 📋 Prompt Format

Every prompt in this library follows a consistent template:

```markdown
---
title: ""
category: 
subcategory: 
tags: []
model: any
---

## Purpose
[One line: what this prompt does and when to use it]

## Prompt
[The rewritten prompt with {VARIABLES}]

## Variables
- {VAR_NAME} – what to fill in here

## Notes
[Tips, variations, and caveats]
```

---

## 🤝 Contributing

We welcome contributions! To add a prompt:

1. Fork this repository
2. Create a new branch: `git checkout -b add/my-prompt-name`
3. Add your prompt file to the correct category folder using the template above
4. Open a Pull Request with a brief description

**Guidelines:**
- Never copy a prompt verbatim — rewrite and improve it
- Use `{CURLY_BRACES}` for all user-specific inputs
- Keep prompts model-agnostic unless a specific model feature is required
- One prompt per file
- Follow the existing folder naming conventions

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).

---

*Built with ❤️ by the open-source community. Star ⭐ the repo if you find it useful!*
