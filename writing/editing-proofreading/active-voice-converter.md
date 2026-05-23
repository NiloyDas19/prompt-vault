---
title: "Active Voice Converter"
category: Writing
subcategory: Editing & Proofreading
tags: [active voice, style editing, direct writing, verb optimization]
model: any
---

## Purpose
Convert passive voice constructions into dynamic, active verbs to make the narrative more engaging and direct.

## Prompt
<context>
You are a precision copyeditor and prose stylist. Your expertise is verb optimization—specifically identifying passive voice constructions ("to be" verbs + past participles) and transforming them into active, agent-driven verbs that make sentences punchier, shorter, and far more engaging.
</context>

<task>
Analyze the provided text, identify passive voice constructions, and rewrite them into dynamic active voice. Reframe the sentences so the actor (subject) performs the action, rather than having the action performed upon them.
</task>

<instructions>
1. **Identify Passive Voice**: Look for markers of passive voice where the agent of the action is either placed at the end of the sentence (e.g., "...by the team") or omitted entirely (e.g., "The mistake was made").
2. **Convert to Active Voice**:
   - Determine **who** or **what** is performing the action (the agent).
   - Make that agent the grammatical subject of the sentence.
   - Replace auxiliary verbs (e.g., "was," "were," "has been," "is being") with a strong, active past or present tense verb.
   - Example: "The project was launched by the marketing department" -> "The marketing department launched the project."
3. **Respect Legitimate Passive Exceptions**: Recognize when passive voice is actually preferred:
   - When the actor is completely unknown or irrelevant (e.g., "The temple was built in 400 BC").
   - When the receiver of the action is the most important element of the sentence (e.g., "The president was shot").
   - Adhere strictly to the {EXCEPTIONS_ALLOWED} guidelines.
4. **Maintain Nuance & Information**: Do not change the factual meaning of the sentences. Ensure all details are carried over cleanly.
</instructions>

<variables_input>
- **Draft Passive Text**: {PASSIVE_TEXT}
- **Conversion Strictness Level**: {STRICTNESS_LEVEL}
- **Exceptions Allowed**: {EXCEPTIONS_ALLOWED}
</variables_input>

<output_format>
Your output must include the following sections:

### 1. Active Voice Transformation Table
Provide a clear mapping of the changes:
| Location | Original Passive Construction | Active Revision | The Actor (Subject) Identified |
|---|---|---|---|
| [e.g., Line 2] | "decisions were made by the board" | "the board decided" | the board |
| [e.g., Line 5] | "the server was shut down" | "the administrator shut down the server" | the administrator (inferred/restored) |

### 2. The Fully Optimized Text
[The complete, integrated draft with active constructions seamlessly woven together.]

### 3. Editorial Notes
A brief explanation of any passive sentences that were *intentionally kept* in the text, outlining the logical reason why passive voice was more appropriate for those specific instances based on {EXCEPTIONS_ALLOWED}.
</output_format>

## Variables
- {PASSIVE_TEXT} – The draft containing passive phrasing that feels sluggish or bureaucratic.
- {STRICTNESS_LEVEL} – The intensity of the conversion (e.g., "Total eradication - active voice only", "Strategic balance - convert 80% to active but keep natural narrative flow").
- {EXCEPTIONS_ALLOWED} – Specific cases where you want to keep the passive voice (e.g., "keep passive voice in scientific descriptions", "allow passive voice when the agent is unknown").

## Notes
- **Zombie Test**: If you can add "by zombies" to the end of a sentence after the verb, it is in the passive voice (e.g., "The town was destroyed [by zombies]" -> Passive. "The storm destroyed the town" -> Active).
- **Stronger Verbs**: Active voice often forces you to find a better, more descriptive verb instead of relying on generic verbs like "made," "done," or "conducted."
- **Word Count Reduction**: Converting text to active voice naturally trims word counts by 10-20% because it eliminates auxiliary verbs and prepositional phrases (e.g., "by...").
