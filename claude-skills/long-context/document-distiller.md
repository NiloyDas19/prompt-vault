---
title: "Document Distiller"
category: Claude Skills
subcategory: Long Context Mastery
tags: [long-context, summarization, document-analysis, insights, research]
model: claude (200K context window)
---

## Purpose
Extract the most important insights, decisions, and action items from a long document or report without losing critical nuance.

## Prompt

Read the following document carefully and completely before responding. Do not skim.

<document>
{FULL_DOCUMENT_TEXT}
</document>

<document_metadata>
- Document type: {DOCUMENT_TYPE} (e.g., annual report, strategy memo, research paper, legal contract)
- My role / reason for reading: {READER_ROLE}
- What I specifically need from this: {SPECIFIC_NEED}
</document_metadata>

After reading, provide:
1. **Executive Summary** (3–5 sentences) — The essence of the document
2. **Key Findings / Decisions / Arguments** — The 5–10 most important points, each explained in 1–2 sentences
3. **Quantitative Data** — All significant numbers, dates, percentages, or statistics mentioned
4. **Action Items** — Any explicit or implied tasks, recommendations, or next steps
5. **Unanswered Questions** — Important questions the document raises but does not answer
6. **What's Missing** — Information you'd expect to see in this type of document that is absent
7. **Direct Quotes** — 2–3 verbatim quotes that best capture the document's core message

## Variables
- `{FULL_DOCUMENT_TEXT}` – Paste the complete document
- `{DOCUMENT_TYPE}` – What kind of document this is
- `{READER_ROLE}` – Your role and why you're reading it (shapes what counts as "important")
- `{SPECIFIC_NEED}` – What you need to get out of this (e.g., "identify legal risks", "understand the financial position", "find the methodology")

## Notes
- 📎 Claude's 200K context window handles books, annual reports, and lengthy contracts in a single pass.
- For legal documents, add "Flag every clause that creates an obligation, liability, or risk for my organization."
- Pair with "Cross-Document Synthesizer" when working across multiple documents.
