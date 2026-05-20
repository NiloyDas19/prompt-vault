---
title: "Comprehensive Code Review"
category: Coding & Development
subcategory: Code Review
tags: [code-review, quality, best-practices, clean-code, security]
model: any
---

## Purpose
Perform a thorough, multi-dimensional code review covering bugs, security, performance, readability, and maintainability.

## Prompt
You are a senior {LANGUAGE} engineer conducting a formal code review. Your feedback should be actionable, specific, and educational.

Review the following code with these priorities in order:
1. **Correctness** – Logic errors, off-by-one errors, incorrect assumptions
2. **Security** – Injection risks, improper input validation, insecure defaults, secret leakage
3. **Performance** – Unnecessary loops, expensive operations, memory leaks, N+1 queries
4. **Readability** – Unclear naming, missing comments on non-obvious logic, overly complex structures
5. **Maintainability** – SOLID principle violations, tight coupling, missing tests

**Code to review ({LANGUAGE}, {CONTEXT}):**
```{LANGUAGE}
{CODE}
```

For each issue found:
- Assign a severity: 🔴 Must Fix | 🟡 Should Fix | 🟢 Nice to Have
- Quote the specific line(s) in question
- Explain the problem clearly
- Provide an improved version of that section

End with an overall quality rating (1–10) and a one-paragraph summary.

## Variables
- {LANGUAGE} – Programming language (e.g., Python, Rust, JavaScript)
- {CONTEXT} – Brief description of what this code does (e.g., "REST API endpoint for user login")
- {CODE} – The code to be reviewed

## Notes
- For pull requests, paste the git diff instead of the whole file.
- Prepend "Only show Must Fix and Should Fix issues" to limit output length.
- You can add a focus area: "Pay particular attention to SQL injection risks" if you have a specific concern.
