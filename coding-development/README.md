# 💻 Coding & Development Prompts

> **18 production-grade prompts** for software engineers — from debugging and code review to architecture design, CI/CD, documentation, and AI security guardrails.

---

## 📂 Subcategories

| Subcategory | Prompts | Description |
|---|---|---|
| [Debugging](#-debugging) | 2 | Root cause analysis, log interpretation |
| [Code Review](#-code-review) | 2 | Quality review, security auditing |
| [Refactoring](#-refactoring) | 2 | SOLID principles, performance optimization |
| [Testing](#-testing) | 1 | Unit test suite generation |
| [Architecture & Design](#-architecture--design) | 2 | REST API design, system architecture |
| [Databases](#-databases) | 2 | Schema design, SQL optimization |
| [DevOps & Automation](#-devops--automation) | 2 | CI/CD pipelines, PR descriptions |
| [Documentation](#-documentation) | 2 | Docstring generation, README creation |
| [Code Generation](#-code-generation) | 2 | MVP scaffolding, legacy modernization |
| [Security & AI Guardrails](#️-security--ai-guardrails) | 3 | Agent system guardrails, prompt injection shields |


---

## 🐛 Debugging

### [Root Cause Debugger](./debugging/root-cause-debugger.md)
Diagnoses the exact root cause of a runtime error and provides a minimal corrected code fix with a clear explanation.
> **Best for:** Runtime exceptions, stack traces, unexpected behavior

### [Log Analyzer & Failure Interpreter](./debugging/log-analyzer.md)
Parses raw application or server logs to identify the failure chain and prioritize remediation steps.
> **Best for:** Production incidents, distributed system debugging, log-heavy environments

---

## 🔍 Code Review

### [Comprehensive Code Review](./code-review/comprehensive-code-review.md)
Multi-dimensional review covering correctness, security, performance, readability, and maintainability — with severity ratings.
> **Best for:** Pre-PR review, knowledge sharing, catching bugs before they ship

### [Security Vulnerability Auditor](./code-review/security-vulnerability-auditor.md)
OWASP-mapped security audit with proof-of-concept attack scenarios and hardened code replacements.
> **Best for:** Auth code, file handlers, input-processing endpoints, compliance reviews

---

## ♻️ Refactoring

### [SOLID Refactor Advisor](./refactoring/solid-refactor-advisor.md)
Refactors code to align with SOLID principles, naming the design patterns applied and explaining every change inline.
> **Best for:** Tightly coupled code, god classes, procedural-to-OOP migrations

### [Performance Optimizer](./refactoring/performance-optimizer.md)
Annotates code with Big-O complexity, identifies the top bottlenecks, and provides an optimized version with trade-off analysis.
> **Best for:** Slow algorithms, N+1 issues in application code, memory-intensive operations

---

## 🧪 Testing

### [Unit Test Suite Generator](./testing/unit-test-suite-generator.md)
Generates a complete, framework-specific unit test suite using the Arrange/Act/Assert pattern, covering happy paths, edge cases, and exceptions.
> **Best for:** Achieving coverage targets, TDD bootstrapping, hardening critical logic

---

## 🏗️ Architecture & Design

### [REST API Designer](./architecture-design/rest-api-designer.md)
Produces a complete API specification with endpoint tables, request/response schemas, error formats, and an OpenAPI 3.0 YAML stub.
> **Best for:** Greenfield APIs, API-first design, team alignment before implementation

### [System Architecture Critic](./architecture-design/system-architecture-critic.md)
Critiques a system design for SPOFs, failure modes, and security risks, then generates MADR-format ADRs for the top recommendations.
> **Best for:** Pre-launch reviews, scaling planning, architecture funding pitches

---

## 🗄️ Databases

### [SQL Schema Designer](./databases/sql-schema-designer.md)
Designs a normalized relational schema with DDL, indexes, a relationships table, and a Mermaid ER diagram.
> **Best for:** New data models, domain modeling, schema documentation

### [SQL Query Optimizer](./databases/sql-query-optimizer.md)
Diagnoses slow SQL queries, explains the performance bottlenecks, rewrites the query, and recommends precise index changes.
> **Best for:** Slow report queries, N+1 in the DB layer, pre-production load testing prep

---

## 🔧 DevOps & Automation

### [GitHub Actions CI/CD Pipeline Generator](./devops-automation/github-actions-cicd-generator.md)
Generates a secure, multi-stage CI/CD pipeline YAML with linting, testing, SAST scanning, container scanning, and deployment.
> **Best for:** New repositories, replacing legacy Jenkins/CircleCI pipelines, shift-left security

### [Pull Request Description Writer](./devops-automation/pull-request-description-writer.md)
Creates a structured, scannable PR description with summary, changes, testing notes, deployment checklist, and rollback plan.
> **Best for:** Saving time on PR descriptions, improving review clarity, team documentation

---

## 📚 Documentation

### [Code Documentation Generator](./documentation/code-documentation-generator.md)
Generates complete inline documentation (docstrings, JSDoc, JavaDoc) for any code block plus a module-level summary for READMEs.
> **Best for:** Undocumented legacy code, public library APIs, onboarding new engineers

### [README Generator](./documentation/readme-generator.md)
Produces a professional, GitHub-ready README.md with badges, features, installation steps, usage examples, and contributing guide.
> **Best for:** Open-source projects, internal tools, portfolio projects

---

## ⚡ Code Generation

### [MVP Project Scaffolder](./code-generation/mvp-project-scaffolder.md)
Generates a complete project structure, DB schema, API routes, authentication, and error handling for a new MVP with a quick-start guide.
> **Best for:** Hackathons, side projects, rapid prototyping, greenfield services

### [Legacy Code Modernizer](./code-generation/legacy-code-modernizer.md)
Migrates legacy code to modern syntax or framework versions, producing a change log, breaking-change report, and testing checklist.
> **Best for:** Python 2→3 migrations, ES5→ES2022, class components→hooks, jQuery removal

---

## 🛡️ Security & AI Guardrails

### [AI Agent System Guardrail](./security-guardrails/agent-system-guardrail.md)
A robust system prompt template to secure AI coding agents, preventing access or alteration of credentials and defending against codebase-embedded prompt injections.
> **Best for:** Coding agents, system prompts, automated pipelines, security guardrails

### [Code Prompt Injection Detector](./security-guardrails/prompt-injection-detector.md)
A specialized analysis prompt to scan code comments, documentation, issues, and user-generated text files for hidden prompt injection payloads or unauthorized instruction overrides.
> **Best for:** Pre-commit hooks, CI/CD safety scanners, agent input sanitation

### [Credential Exposure & Leakage Scanner](./security-guardrails/credential-exposure-guard.md)
A codebase scanner prompt designed to detect hardcoded credentials, API keys, passwords, and private tokens within code, proposing secure environment-variable-based refactoring.
> **Best for:** Secret detection, security auditing, safe code refactoring

---

## 💡 Usage Tips

1. **Always provide context** — The more specific your variables, the better the output.
2. **Chain prompts** — Use "Code Review" → "Refactor" → "Write Tests" as a workflow.
3. **Validate AI output** — Never blindly copy-paste generated code into production.
4. **Iterate** — Follow up with "Focus more on X" or "Show only the changed lines."
5. **Model-agnostic** — All prompts work with ChatGPT, Claude, Gemini, and other capable LLMs.

---

*Part of the [Prompt Vault](../../README.md) open-source prompt library.*
