---
title: "Root Cause Debugger"
category: Coding & Development
subcategory: Debugging
tags: [debugging, error-analysis, root-cause, troubleshooting]
model: any
---

## Purpose
Diagnose the root cause of a runtime error or exception and receive a clear, actionable fix with an explanation.

## Prompt
You are a senior {LANGUAGE} engineer with deep expertise in diagnosing runtime errors.

I am encountering the following error in my {LANGUAGE} / {FRAMEWORK} project:

**Error / Stack Trace:**
```
{ERROR_MESSAGE}
```

**Relevant Code Snippet:**
```{LANGUAGE}
{CODE_SNIPPET}
```

**What I have already tried:**
{ATTEMPTED_FIXES}

Please do the following:
1. Identify the exact root cause of this error.
2. Explain *why* this error occurs in plain language.
3. Provide a corrected version of the code with the minimal changes needed.
4. List any related edge cases I should guard against after applying the fix.

## Variables
- {LANGUAGE} – The programming language (e.g., Python, TypeScript, Go)
- {FRAMEWORK} – The framework or runtime (e.g., FastAPI, Next.js, Express)
- {ERROR_MESSAGE} – The full error message and stack trace
- {CODE_SNIPPET} – The block of code that is failing
- {ATTEMPTED_FIXES} – What you've already tried, or write "None yet"

## Notes
- For intermittent bugs, describe the conditions under which the error appears instead of a stack trace.
- Ask the model to output only a unified diff if you have a large file.
- Works well with any general-purpose LLM; no special model required.
