---
title: "Pull Request Description Writer"
category: Coding & Development
subcategory: DevOps & Automation
tags: [git, pull-request, documentation, code-review, collaboration]
model: any
---

## Purpose
Generate a well-structured, professional pull request description from a summary of code changes.

## Prompt
You are a senior software engineer who writes exceptionally clear and thorough pull request descriptions that help reviewers understand changes quickly and confidently.

Write a professional pull request description based on the following information:

**Change type:** {CHANGE_TYPE} (e.g., Feature, Bug Fix, Refactor, Performance, Security Patch, Chore)
**Ticket / Issue reference:** {TICKET_ID} (e.g., JIRA-1234, GitHub Issue #42, or "N/A")
**What changed (your notes):** {CHANGE_SUMMARY}
**Why this change was needed:** {MOTIVATION}
**Testing done:** {TESTING_DONE}
**Deployment notes:** {DEPLOYMENT_NOTES} (e.g., requires DB migration, feature flag needed, or "None")
**Screenshots / recordings (if UI change):** {VISUAL_EVIDENCE} (describe them, or "N/A")

Write the PR description in Markdown with these sections:
### Summary
### Motivation & Context
### Changes Made
### How to Test
### Screenshots (if applicable)
### Deployment Checklist
### Risks & Rollback Plan

Keep each section concise and scannable. Use bullet points, not paragraphs, in the "Changes Made" and "Deployment Checklist" sections.

## Variables
- {CHANGE_TYPE} – The nature of the change
- {TICKET_ID} – Issue tracker reference
- {CHANGE_SUMMARY} – A plain-English description of what changed technically
- {MOTIVATION} – Why the change was needed (user pain point, bug report, performance goal)
- {TESTING_DONE} – Types of testing performed (unit, integration, manual, load test)
- {DEPLOYMENT_NOTES} – Any special deployment steps (migrations, env vars, feature flags)
- {VISUAL_EVIDENCE} – Describe any screenshots/videos you'll attach, or "N/A"

## Notes
- For code-only changes without UI, omit the Screenshots section entirely.
- Ask the model to "make the tone more formal" or "more casual" based on your team's culture.
- Pair with the "Comprehensive Code Review" prompt — have AI review your code, then write the PR description.
