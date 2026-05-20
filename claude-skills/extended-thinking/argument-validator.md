---
title: "Logical Argument Validator"
category: Claude Skills
subcategory: Extended Thinking
tags: [logic, critical-thinking, reasoning, argumentation, fallacies]
model: claude (Extended Thinking recommended)
---

## Purpose
Rigorously analyze a written argument for logical validity, soundness, hidden assumptions, and logical fallacies.

## Prompt

Analyze the following argument for logical rigor. Work through it carefully, step by step.

<argument>
{ARGUMENT_TEXT}
</argument>

<claimed_conclusion>
{CONCLUSION}
</claimed_conclusion>

Please:
1. **Reconstruct the argument** — State the premises and conclusion in standard logical form (P1, P2 → C)
2. **Check validity** — Is the conclusion logically entailed by the premises? (Does the form hold, ignoring truth of premises?)
3. **Check soundness** — Are the premises actually true or well-supported? What evidence would be needed?
4. **Identify hidden assumptions** — What unstated assumptions does the argument rely on? Are they reasonable?
5. **Identify fallacies** — Name any logical fallacies present (e.g., straw man, false dichotomy, ad hominem, slippery slope)
6. **Overall verdict** — Is this a strong, weak, or invalid argument? Summarize in 2–3 sentences.
7. **Steelman** — Provide the strongest possible version of this argument, even if the original is weak.

## Variables
- {ARGUMENT_TEXT} – The argument to analyze (paste the full text)
- {CONCLUSION} – The main claim or conclusion the argument is trying to establish

## Notes
- 🧠 Requires Extended Thinking — Extended Thinking significantly improves fallacy detection in complex, multi-paragraph arguments.
- Use this for evaluating research paper arguments, political claims, business proposals, or debate prep.
- The "Steelman" step is especially valuable for productive disagreement.
