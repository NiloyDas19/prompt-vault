---
title: "Codebase Navigator"
category: Claude Skills
subcategory: Long Context Mastery
tags: [long-context, codebase, code-understanding, architecture, onboarding]
model: claude (200K context window)
---

## Purpose
Onboard Claude to a large codebase so it can answer questions, explain logic, and find bugs across the entire project at once.

## Prompt

I am sharing a large codebase with you. Please read all of it carefully before responding. Your goal is to deeply understand this codebase so you can act as an expert guide.

<codebase>
{PASTE_ENTIRE_CODEBASE_OR_KEY_FILES}
</codebase>

<project_overview>
- Project name: {PROJECT_NAME}
- Primary language / framework: {TECH_STACK}
- What it does: {PROJECT_DESCRIPTION}
- My role on this project: {YOUR_ROLE}
</project_overview>

<task>
{SPECIFIC_TASK}
</task>

Before answering the task, confirm you've read the codebase by providing:
1. A one-paragraph summary of what the codebase does
2. The key architectural patterns you notice
3. Any red flags or code smells you spotted while reading

Then address the task in full.

## Variables
- `{PASTE_ENTIRE_CODEBASE_OR_KEY_FILES}` – Paste files directly. Use Claude's full 200K context.
- `{PROJECT_NAME}` – Name of the project
- `{TECH_STACK}` – Primary language(s) and framework(s)
- `{PROJECT_DESCRIPTION}` – What the project does
- `{YOUR_ROLE}` – Your role (e.g., new engineer onboarding, tech lead doing audit)
- `{SPECIFIC_TASK}` – Your actual question or task (e.g., "Find all places where user input is not sanitized", "Explain the authentication flow", "Why does the order processing sometimes fail?")

## Notes
- 📎 Requires Claude's 200K token context window — only available in Claude.ai Pro/Team or via API.
- Prioritize pasting the most critical files: entry points, core business logic, models, and the file most related to your task.
- For very large repos, use a tool like `find . -name '*.py' | xargs cat` to concatenate files quickly.
