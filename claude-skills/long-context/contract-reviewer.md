---
title: "Contract & Legal Document Reviewer"
category: Claude Skills
subcategory: Long Context Mastery
tags: [long-context, legal, contracts, risk, compliance]
model: claude (200K context window)
---

## Purpose
Review a full legal contract or agreement to surface obligations, risks, unusual clauses, and missing protections — in plain language.

## Prompt

Review the following legal document carefully and completely. Your goal is to help me understand my obligations, risks, and protections — in plain language.

<legal_document>
{FULL_CONTRACT_TEXT}
</legal_document>

<my_context>
- My role in this agreement: {MY_ROLE} (e.g., service provider, customer, employee, licensor)
- My primary concern: {PRIMARY_CONCERN} (e.g., liability exposure, IP ownership, termination rights)
- Industry / jurisdiction: {JURISDICTION}
</my_context>

Please provide:
1. **Plain-language summary** — What this agreement does in 5 sentences
2. **My key obligations** — What I am required to do (with section references)
3. **Their key obligations** — What the other party is required to do
4. **Risk flags** 🚩 — Clauses that create unusual risk, unlimited liability, one-sided terms, or aggressive IP assignments
5. **Missing protections** — Standard clauses I'd expect that are absent (e.g., limitation of liability, indemnification cap, IP ownership, data protection)
6. **Negotiation priorities** — The top 3 clauses I should try to change, and what to ask for
7. **Confusing clauses** — Any sections that are unusually vague, contradictory, or difficult to interpret

## Variables
- `{FULL_CONTRACT_TEXT}` – Paste the complete contract text
- `{MY_ROLE}` – Your role in the agreement
- `{PRIMARY_CONCERN}` – Your biggest worry or priority
- `{JURISDICTION}` – Country/state the contract is governed by

## Notes
- ⚠️ This prompt does not replace qualified legal counsel. Use it for initial review and to prepare informed questions for your lawyer.
- 📎 Claude can handle contracts of hundreds of pages in a single context window.
- Add "Focus specifically on Section {X}" to drill into a specific clause.
