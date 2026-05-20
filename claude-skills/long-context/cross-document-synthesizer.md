---
title: "Cross-Document Synthesizer"
category: Claude Skills
subcategory: Long Context Mastery
tags: [long-context, synthesis, research, multi-document, analysis]
model: claude (200K context window)
---

## Purpose
Load multiple documents simultaneously and synthesize insights, contradictions, and themes across all of them at once.

## Prompt

I am sharing multiple documents with you. Read all of them carefully before synthesizing. Your goal is to find connections, contradictions, and themes across the full set.

<document_1 label="{DOC_1_LABEL}">
{DOCUMENT_1}
</document_1>

<document_2 label="{DOC_2_LABEL}">
{DOCUMENT_2}
</document_2>

<document_3 label="{DOC_3_LABEL}">
{DOCUMENT_3}
</document_3>

<synthesis_goal>
{SYNTHESIS_GOAL}
</synthesis_goal>

After reading all documents, provide:
1. **Individual summaries** — 2–3 sentences per document capturing its core argument or content
2. **Common themes** — What ideas, findings, or concerns appear across multiple documents?
3. **Contradictions** — Where do documents directly or indirectly disagree? Which is better supported?
4. **Unique contributions** — What does each document contribute that the others don't?
5. **Synthesis** — Combine the insights from all documents into a unified view addressing {SYNTHESIS_GOAL}
6. **Evidence gaps** — What question do all documents fail to answer?

## Variables
- `{DOC_1_LABEL}`, `{DOC_2_LABEL}`, `{DOC_3_LABEL}` – Short labels for each document (e.g., "2023 Annual Report", "Competitor Analysis", "Customer Survey")
- `{DOCUMENT_1}`, `{DOCUMENT_2}`, `{DOCUMENT_3}` – The full text of each document. Add more `<document_N>` blocks as needed.
- `{SYNTHESIS_GOAL}` – What you want the synthesis to answer or produce

## Notes
- 📎 Claude's 200K window allows loading entire books, reports, and research papers together.
- Add more document blocks freely — the pattern scales to as many documents as fit in context.
- Great for literature reviews, competitive intelligence, and due diligence.
