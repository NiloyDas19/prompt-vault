---
title: "SOLID Refactor Advisor"
category: Coding & Development
subcategory: Refactoring
tags: [refactoring, SOLID, clean-code, design-patterns, maintainability]
model: any
---

## Purpose
Refactor a code block to follow SOLID principles, with a clear explanation of every change made.

## Prompt
You are a senior software engineer and clean code advocate. Refactor the following {LANGUAGE} code to align with SOLID principles and modern best practices.

**Original Code:**
```{LANGUAGE}
{CODE}
```

**Refactoring Goals:**
- Improve adherence to: {PRINCIPLES} (e.g., Single Responsibility, Open/Closed, Dependency Inversion)
- Target readability level: {AUDIENCE} (e.g., junior devs on our team, any engineer)
- Constraints: {CONSTRAINTS} (e.g., cannot change the public API, must stay in one file)

Please:
1. Show the fully refactored code.
2. For each significant change, add an inline comment starting with `// REFACTOR:` explaining what changed and why.
3. List any design patterns you applied (e.g., Strategy, Factory, Repository).
4. Describe the trade-offs — what did this refactor cost vs. what did it gain?
5. Suggest what unit tests should be written to validate the refactored behavior.

## Variables
- {LANGUAGE} – Programming language (e.g., Java, C#, Python, TypeScript)
- {CODE} – The original code to refactor
- {PRINCIPLES} – Specific SOLID principles to target, or "all" for a full review
- {AUDIENCE} – Who will maintain this code (affects how verbose comments should be)
- {CONSTRAINTS} – Any limitations (public API stability, framework versions, file structure)

## Notes
- If you only want cosmetic improvements (naming, formatting), say so explicitly to avoid structural rewrites.
- Chain this with the "Comprehensive Code Review" prompt — review first, then refactor.
- For large files, ask the model to refactor one class or function at a time.
