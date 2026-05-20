---
title: "Unit Test Suite Generator"
category: Coding & Development
subcategory: Testing
tags: [unit-testing, TDD, test-coverage, test-cases, quality-assurance]
model: any
---

## Purpose
Generate a comprehensive unit test suite for a given function or class, covering happy paths, edge cases, and failure modes.

## Prompt
You are a senior software engineer who is an expert in test-driven development (TDD) and the {TEST_FRAMEWORK} testing framework.

I need a complete unit test suite for the following {LANGUAGE} code:

```{LANGUAGE}
{CODE}
```

**Testing requirements:**
- Framework: {TEST_FRAMEWORK} (e.g., pytest, Jest, JUnit 5, RSpec, xUnit)
- Naming convention: {NAMING_CONVENTION} (e.g., `test_<method>_when_<condition>_should_<result>`)
- Mocking library: {MOCK_LIBRARY} (e.g., unittest.mock, Sinon.js, Mockito) — use it for all external dependencies
- Coverage target: {COVERAGE_TARGET} (e.g., 90%+, all public methods)

Please:
1. Identify: the happy path, all meaningful edge cases, and failure/exception scenarios.
2. Write a test for each scenario with a clear, descriptive name.
3. Use the Arrange / Act / Assert (AAA) pattern within each test.
4. Add a comment above each test explaining what it validates and why it matters.
5. Include any necessary fixtures or test data setup.

## Variables
- {LANGUAGE} – Programming language (e.g., Python, TypeScript, Java, C#)
- {CODE} – The function, class, or module to test
- {TEST_FRAMEWORK} – The testing framework to use
- {NAMING_CONVENTION} – Test method naming pattern, or "follow {TEST_FRAMEWORK} conventions"
- {MOCK_LIBRARY} – Mocking library, or "use {TEST_FRAMEWORK}'s built-in mocking"
- {COVERAGE_TARGET} – Desired coverage level or "prioritize critical paths"

## Notes
- If the code has no dependency injection, ask the model to suggest how to refactor it to be more testable before writing tests.
- For async code, explicitly state "all tests must be async" for frameworks that require it.
- Chain with the "SOLID Refactor Advisor" if testability is the main concern.
