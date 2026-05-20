---
title: "Legacy Code Modernizer"
category: Coding & Development
subcategory: Code Generation
tags: [modernization, refactoring, migration, legacy-code, upgrade]
model: any
---

## Purpose
Migrate or modernize legacy code to a newer syntax, framework version, or language paradigm while preserving all existing behavior.

## Prompt
You are a senior {LANGUAGE} engineer with deep expertise in both legacy {FROM_VERSION} patterns and modern {TO_VERSION} best practices.

Modernize the following legacy code:

**Original code ({FROM_VERSION}):**
```{LANGUAGE}
{CODE}
```

**Modernization target:** {TO_VERSION} (e.g., ES5 → ES2022, Python 2 → Python 3.11, jQuery → Vanilla JS, class components → React Hooks, callbacks → async/await)

**Constraints:**
- {CONSTRAINTS} (e.g., "must not change public function signatures", "TypeScript strict mode required", "must run on Node.js 18+")

Please:
1. **Modernized code** — The full updated version using modern idioms, syntax, and patterns
2. **Change log** — A table listing every change made: what it was → what it became → why
3. **Breaking changes** — Flag anything that changes behavior, even subtly (return type changes, exception handling differences, etc.)
4. **Dependency updates** — List any package upgrades or replacements required
5. **Migration testing checklist** — 5–10 specific things to test to ensure behavior is preserved

## Variables
- {LANGUAGE} – Programming language (e.g., JavaScript, Python, Java, PHP)
- {CODE} – The legacy code to modernize
- {FROM_VERSION} – Current version or paradigm (e.g., JavaScript ES5, Python 2.7, React Class Components, PHP 5)
- {TO_VERSION} – Target version or paradigm (e.g., JavaScript ES2022, Python 3.11, React Hooks, PHP 8.2)
- {CONSTRAINTS} – Restrictions on what can or cannot change

## Notes
- For large codebases, modernize one module or function at a time.
- Ask the model to output only a unified diff (`diff -u` format) if you need something easy to apply with `git apply`.
- Pair with "Unit Test Suite Generator" before modernizing to create a safety net of tests.
