---
title: "Ethical Dilemma Reasoner"
category: Claude Skills
subcategory: Extended Thinking
tags: [ethics, reasoning, philosophy, decision-making, extended-thinking]
model: claude (Extended Thinking recommended)
---

## Purpose
Reason through genuine ethical dilemmas from multiple moral frameworks, arriving at a nuanced, well-justified position.

## Prompt

Reason carefully through the following ethical dilemma. Do not jump to a conclusion — instead, work through the problem from multiple moral frameworks before reaching a considered position.

<dilemma>
{DILEMMA_DESCRIPTION}
</dilemma>

<stakeholders>
{AFFECTED_PARTIES}
</stakeholders>

<additional_context>
{CONTEXT}
</additional_context>

Analyze this dilemma through each of these lenses:
1. **Consequentialism** — What outcome produces the greatest good for the greatest number? Who is harmed, and how much?
2. **Deontology** — What duties, rights, or rules apply? Are any absolute principles at stake?
3. **Virtue Ethics** — What would a person of excellent character do? What virtues are relevant?
4. **Care Ethics** — What does this situation demand in terms of relationships and responsibilities to specific people?

After applying all frameworks:
5. **Identify the core tension** — Where do the frameworks agree? Where do they conflict?
6. **Your considered position** — Taking all perspectives into account, what is the most defensible course of action, and why?
7. **Caveats** — What information would change your answer?

## Variables
- {DILEMMA_DESCRIPTION} – Describe the ethical situation in detail
- {AFFECTED_PARTIES} – Who is involved and what are their interests?
- {CONTEXT} – Any background, cultural, legal, or organizational context

## Notes
- 🧠 Requires Extended Thinking — Extended Thinking mode gives Claude the reasoning space this type of deep analysis requires.
- This prompt is excellent for business ethics decisions, policy design, and moral philosophy coursework.
- Ask for a "minority view" at the end to stress-test the conclusion.
