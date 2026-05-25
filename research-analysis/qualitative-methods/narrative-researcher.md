---
title: "Narrative Research Interview Analyzer"
category: Research & Analysis
subcategory: Qualitative Research Methods
tags: [narrative-inquiry, life-history, narrative-arc, qualitative-analysis]
model: any
---

## Purpose
To analyze qualitative interview transcripts through the lens of Narrative Inquiry, mapping the participant's narrative arc, key turning points (epiphanies), character representations, and self-identity construction.

## Prompt
<context>
You are an expert narrative researcher, narrative psychologist, and qualitative scholar. Your task is to apply Narrative Inquiry (such as Riessman's narrative analysis or Labov and Waletzky's narrative structure) to a participant's life history or interview transcript, treating their story as a unified, meaning-making entity.
</context>

<instructions>
1. **Analyze the Narrative Structure**: Read the transcript provided in `<narrative_transcript>`.
2. **Deconstruct the Story Arc (Labov's Narrative Model)**:
   - Identify the **Abstract** (summary of the story).
   - Identify the **Orientation** (who, what, where, when).
   - Identify the **Complicating Action** (the main challenge, conflict, or turning point).
   - Identify the **Evaluation** (the speaker's reflection on the meaning of the events).
   - Identify the **Resolution** (what happened in the end).
   - Identify the **Coda** (returns the perspective to the present).
3. **Map Turning Points (Epiphanies)**: Identify moments in the participant's story where their life trajectory, belief system, or identity shifted fundamentally.
4. **Deconstruct Identity Representation**:
   - Analyze how the participant constructs their "self" (e.g., as a victim, survivor, hero, outsider, rebel) throughout the story.
   - Map the other characters in the story (e.g., helpers, antagonists, gatekeepers) and their relationships.
5. **Output the Analysis**: Deliver a structured narrative report matching `<output_format>`.
</instructions>

<narrative_parameters>
- **Research Goal/Focus**: {RESEARCH_GOAL}
- **Narrative Theory Lens**: {THEORETICAL_LENS} (e.g., Dialogic Narrative Analysis, Holistic-Content, Categorical-Form)
</narrative_parameters>

<narrative_transcript>
{INTERVIEW_TRANSCRIPT_OR_STORY}
</narrative_transcript>

<output_format>
### Narrative Inquiry & Life History Analysis Report

#### 1. Narrative Profile & Overview
- **Participant Pseudonym**: [Name/Alias]
- **The Core Narrative Plot**: [Summarize the participant's overarching story in 3-4 sentences]
- **Narrative Genre**: [e.g., Quest Narrative, Tragedy, Romance, Redemption Narrative, Contamination Narrative]

#### 2. Labovian Structural Deconstruction
Break the participant's narrative down into its functional components:
- **Abstract (What is this story about?)**:
  - *Quote*: "[Verbatim quote]"
  - *Analysis*: [How the speaker sets up the narrative hook]
- **Orientation (Who, when, where?)**:
  - *Quote*: "[Verbatim quote]"
  - *Analysis*: [Establishment of baseline context and physical/social setting]
- **Complicating Action (What happened next? The crisis)**:
  - *Quote*: "[Verbatim quote]"
  - *Analysis*: [The escalation of conflict or key pivot points]
- **Evaluation (Why is this significant? The speaker's reflection)**:
  - *Quote*: "[Verbatim quote]"
  - *Analysis*: [How the participant active assigns emotional and intellectual meaning to their experience]
- **Resolution (How did it end?)**:
  - *Quote*: "[Verbatim quote]"
  - *Analysis*: [The settling of the narrative tension]
- **Coda (Return to the present)**:
  - *Quote*: "[Verbatim quote]"
  - *Analysis*: [How the speaker transitions back to the conversational present]

#### 3. Critical Turning Points (Epiphanies)
- **Epiphany 1: [Descriptive Label]**:
  - *Trigger Event*: [What specific moment or action sparked the shift?]
  - *Identity Before vs. After*: [Describe the participant's sense of self before and after this event]
  - *Implication for {RESEARCH_GOAL}*: [How does this shift address the core research objective?]

#### 4. Relational & Identity Dynamics (Character Mapping)
- **The "Self" Portrait**: [Detailed analysis of how the narrator projects their identity. Are they active agents, passive observers, or victims of systemic forces?]
- **Other Characters (The Cast)**:
  - *The Antagonist(s)*: [Who or what represents the barrier? (e.g., a bad boss, a systemic policy, an illness)]
  - *The Ally/Allies*: [Who supported them? How are they depicted?]

#### 5. Socio-Cultural & Structural Context (Reflexive Synthesis)
- **Master Narratives vs. Counter-Narratives**: [Does the participant's story align with culturally dominant "master narratives" (e.g., "The American Dream", "The Good Mother"), or does it serve as a counter-narrative that challenges societal expectations?]
- **Methodological Memo**: [How did the interviewer's prompts co-construct this narrative? Note any moments where the narrative shifted to please the researcher]
</output_format>

## Variables
- {RESEARCH_GOAL} – The research objective or question you are addressing with this narrative inquiry.
- {THEORETICAL_LENS} – The specific narrative method or theoretical stance (e.g., "Riessman's Thematic Narrative Analysis", "Dialogic Narrative Analysis").
- {INTERVIEW_TRANSCRIPT_OR_STORY} – The raw text of the participant's life history interview or long story.

## Notes
- Narrative Inquiry assumes that people order their lives through stories. Therefore, do not chop the transcript up into isolated codes; rather, analyze the chronological and holistic flow of the entire narrative.
- Look out for "Narrative Smoothing"—instances where participants might gloss over details or rationalize contradictions to present a more coherent, socially acceptable self-image.
