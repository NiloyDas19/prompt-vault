---
title: "GitHub Actions CI/CD Pipeline Generator"
category: Coding & Development
subcategory: DevOps & Automation
tags: [CI/CD, GitHub-Actions, DevOps, automation, pipeline, deployment]
model: any
---

## Purpose
Generate a secure, production-ready GitHub Actions CI/CD pipeline with build, test, static analysis, and deployment stages.

## Prompt
You are a Senior DevOps Engineer specializing in secure CI/CD pipelines for {LANGUAGE} / {FRAMEWORK} applications.

Generate a complete GitHub Actions workflow file for my project with the following requirements:

**Project details:**
- Language / Runtime: {LANGUAGE} (e.g., Node.js 20, Python 3.11, Java 17)
- Framework: {FRAMEWORK} (e.g., Next.js, Django, Spring Boot)
- Test framework: {TEST_FRAMEWORK}
- Target deployment environment: {DEPLOY_TARGET} (e.g., AWS ECS, Vercel, Google Cloud Run, Kubernetes)

**Required pipeline stages (in order):**
1. Checkout & dependency installation
2. Linting and static analysis
3. Unit and integration tests with coverage reporting
4. Security scanning (SAST using {SAST_TOOL} e.g., Semgrep, CodeQL)
5. Docker image build and vulnerability scan (using Trivy or Snyk)
6. Deploy to {DEPLOY_TARGET} only if all prior stages pass
7. Notify {NOTIFICATION_CHANNEL} on success or failure

**Security requirements:**
- Never hardcode credentials — use GitHub Secrets for all sensitive values
- Apply least-privilege IAM/permissions on the workflow
- Fail the pipeline if any HIGH or CRITICAL security finding is detected
- Pin all action versions to a specific SHA (not `@main` or `@latest`)

Please produce:
1. The complete `.github/workflows/ci-cd.yml` file
2. A table listing every required GitHub Secret and what value it should hold
3. A brief explanation of each stage's purpose

## Variables
- {LANGUAGE} – Programming language and version (e.g., Python 3.11)
- {FRAMEWORK} – Web framework (e.g., FastAPI, Rails, Spring Boot)
- {TEST_FRAMEWORK} – Testing framework (e.g., pytest, Mocha, JUnit)
- {DEPLOY_TARGET} – Where to deploy (e.g., AWS ECS via ECR, Vercel, GCP Cloud Run)
- {SAST_TOOL} – Static analysis tool: CodeQL (free for public repos), Semgrep, or SonarCloud
- {NOTIFICATION_CHANNEL} – Where to send notifications (e.g., Slack webhook, email, PagerDuty)

## Notes
- 🚨 Flag: This prompt generates security-conscious pipelines; review IAM permissions and OIDC configuration for your specific cloud provider.
- For monorepos, add "Only trigger this workflow when files in `{SERVICE_DIRECTORY}` change" to avoid unnecessary runs.
- Ask for a separate `pr-check.yml` workflow if you want lightweight checks on pull requests.
