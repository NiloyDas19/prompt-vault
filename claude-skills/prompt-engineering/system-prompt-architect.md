---
title: "System Prompt Architect"
category: Claude Skills
subcategory: Prompt Engineering for Claude
tags: [prompt-engineering, system-prompt, Claude-API, configuration, personas]
model: claude
---

## Purpose
Design a production-ready system prompt for a Claude-powered application, setting persona, behavior, boundaries, and output format.

## Prompt

You are an expert prompt engineer specializing in Claude's behavior and capabilities. Design a complete, production-ready system prompt for the following application.

<application_details>
- Application name: {APP_NAME}
- What it does: {APP_DESCRIPTION}
- Target users: {TARGET_USERS}
- Tone and persona: {DESIRED_TONE} (e.g., formal and authoritative, warm and friendly, concise and technical)
- Core capabilities it should have: {CAPABILITIES}
- Hard limits (what it must never do): {OFF_LIMITS}
- Output format preferences: {OUTPUT_FORMAT}
</application_details>

Design a system prompt that:
1. Opens with a clear persona definition (who Claude is in this app)
2. States the primary mission and capabilities
3. Specifies behavioral guidelines (tone, length, format)
4. Defines hard limits with specific, unambiguous language
5. Handles edge cases (what to do when asked something out of scope)
6. Uses XML tags to separate distinct instruction blocks
7. Ends with a brief self-check instruction

Also provide:
- A one-paragraph explanation of your key design decisions
- 3 test prompts that would stress-test this system prompt
- Potential failure modes and how the system prompt addresses them

## Variables
- `{APP_NAME}` – Name of the application
- `{APP_DESCRIPTION}` – What the application does and its context
- `{TARGET_USERS}` – Who will interact with this application
- `{DESIRED_TONE}` – The persona and communication style
- `{CAPABILITIES}` – What the AI should be able to help with
- `{OFF_LIMITS}` – What the AI must never do or discuss
- `{OUTPUT_FORMAT}` – Preferred output style (e.g., always use bullet points, respond in under 150 words, always include a call to action)

## Notes
- Claude responds especially well to XML-structured system prompts with clear section delimiters.
- Test your system prompt with adversarial inputs (jailbreak attempts, off-topic questions) before deploying.
- Add a `<examples>` section in the system prompt for few-shot behavior shaping.
