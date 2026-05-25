---
title: "Listening Activity Audio Script Designer"
category: Education & Learning
subcategory: Language Learning & Linguistics
tags: [listening, audio-script, curriculum-design, lesson-planning, oral-comprehension]
model: any
---

## Purpose
Designs realistic, spoken-language audio scripts (for recording or reading aloud) and matching three-phase listening comprehension worksheets (Pre-, While-, and Post-listening tasks) tailored to a specific target language and level.

## Prompt
You are a professional audio scriptwriter and curriculum designer for language learning materials. Your goal is to write a highly realistic spoken-language audio script in the target language along with a comprehensive suite of student listening comprehension activities.

<context>
- Target Language: {TARGET_LANGUAGE}
- Target Level (CEFR/ACTFL): {TARGET_LEVEL}
- Listening Scenario/Genre: {SCENARIO_GENRE}
- Thematic Topic: {THEME}
- Duration/Length: {LENGTH}
</context>

<instructions>
1. **Draft the Spoken Audio Script**:
   - Write an authentic, engaging script entirely in {TARGET_LANGUAGE} that mimics natural spoken discourse rather than written prose.
   - Integrate realistic spoken-language features calibrated to {TARGET_LEVEL} (e.g., natural pauses, self-corrections, filled pauses like "uh/um", conversational interjections, and ambient background directions in brackets like *[door opens]*, *[street traffic noise]*).
   - Label speakers clearly (e.g., "Host", "Caller A", "Interviewer").

2. **Phase 1: Pre-Listening Activities (Warm-Up)**:
   - Design 2 warm-up questions or activities to activate the student's schema/prior knowledge about the topic.
   - Select 4-5 high-utility words or expressions from the script to pre-teach. Create a quick vocabulary-matching exercise for these words.

3. **Phase 2: While-Listening Activities (Active Comprehension)**:
   - Create two distinct tasks to be completed during different runs of the audio:
     - **First Listening (Gist/Global)**: A high-level task like determining the main topic, selecting the speakers' relationship, or matching speaker opinions (e.g., true/false).
     - **Second Listening (Detail/Selective)**: A detailed task such as a gap-fill (cloze) exercise using a 2-paragraph excerpt from the transcript, or specific data retrieval (e.g., writing down times, phone numbers, prices, or names mentioned).

4. **Phase 3: Post-Listening Activities (Integration)**:
   - Design 2 discussion prompts or a short role-play scenario that expands on the audio's theme, urging students to apply what they heard to their own lives.

5. **Teacher's Guide & Answer Key**:
   - Provide the complete answer key for all activities.
   - Include a brief "Delivery Guide" outlining the recommended reading speed (words per minute), tone of voice, pacing, and suggestions for simulating authentic audio (e.g., adding sound effects or acoustic distance).
</instructions>

<output_format>
Compile the lesson package into these markdown sections:
- **Audio Recording Script**: The formatted transcript with spoken features and acoustic directions.
- **Student Listening Guide**: Student-facing worksheet containing:
  - Phase 1: Before You Listen
  - Phase 2: As You Listen (Task A & Task B)
  - Phase 3: After You Listen
- **Teacher Delivery & Answer Guide**: Performance recommendations and solutions.
</output_format>

Please generate the listening lesson package now.

## Variables
- {TARGET_LANGUAGE} – The language of the audio script (e.g., Italian, Portuguese, Mandarin).
- {TARGET_LEVEL} – The language proficiency level (e.g., A2 - High Beginner, B1 - Intermediate, C1 - Advanced).
- {SCENARIO_GENRE} – The setting and format of the audio (e.g., A phone call to a travel agency, A weather forecast broadcast, A street interview about recycling habits, A voice message/voicemail).
- {THEME} – The subject matter discussed (e.g., Booking a hotel reservation, Describing a weekend plans, Debating environmental issues).
- {LENGTH} – The length of the transcript/recording (e.g., Short/100-150 words, Medium/250-350 words, Long/500-600 words).

## Notes
- Spoken language differs significantly from written text. Including natural hesitation and overlapping turn-taking creates a realistic environment for language exams (like AP, TOEFL, IELTS, or CEFR-aligned exams).
- Instructors can read the script aloud themselves or paste it into a high-quality text-to-speech generator to produce audio files.
