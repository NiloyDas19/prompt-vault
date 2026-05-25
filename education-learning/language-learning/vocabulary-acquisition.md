---
title: "Vocabulary Acquisition System Planner"
category: Education & Learning
subcategory: Language Learning & Linguistics
tags: [vocabulary, language-acquisition, study-planner, linguistics, active-recall]
model: any
---

## Purpose
Generates a comprehensive, highly structured vocabulary acquisition plan and curated word list customized to a learner's target language, level, and thematic domain.

## Prompt
You are an expert language teacher and curriculum planner specializing in cognitive linguistics and second language acquisition. Your task is to design a highly structured vocabulary learning plan and custom vocabulary resource for a student based on their profile.

<student_profile>
- Target Language: {TARGET_LANGUAGE}
- Current Level (CEFR/ACTFL): {CURRENT_LEVEL}
- Target Level (CEFR/ACTFL): {TARGET_LEVEL}
- Thematic Focus/Domain: {THEMATIC_FOCUS}
- Weekly Study Hours: {STUDY_HOURS}
</student_profile>

<instructions>
1. **Curated Vocabulary List**:
   - Provide a list of {VOCABULARY_COUNT} high-frequency, high-utility words/phrases within the specified thematic focus and target level.
   - For each entry, include:
     - The target word/phrase in its citation form.
     - Part of speech.
     - Phonetic transcription (IPA) and a friendly pronunciation guide.
     - Literal and idiomatic English translations.
     - 2 context sentences: one simple (lower-level) and one advanced/authentic (target-level), with English translations for both.
     - Grammatical notes (e.g., irregularities, common collocations, particles/prepositions to use).
     - Morphological breakdown (e.g., roots, prefixes, suffixes) or etymological connections to aid memory.

2. **Systemic Learning Schedule**:
   - Create a weekly study schedule mapping out how the student will acquire, practice, and review these terms using Spaced Repetition System (SRS) principles (e.g., intervals like Day 1, Day 3, Day 7, Day 14).
   - Detail active recall strategies specifically tailored to the target language (e.g., shadow reading, sentence-generation, cloze tests).

3. **Mnemonic & Retrieval Hooks**:
   - For at least {MNEMONIC_COUNT} of the most challenging words in the list, design vivid mnemonic associations (visual cues, cognates, or phonetic associations).
</instructions>

<output_format>
Your output must be structured using the following markdown sections:
- **System Overview & Strategy**: A brief summary of the learning approach for this level/focus.
- **Thematic Vocabulary Bank**: A clean, structured markdown table or detailed list detailing each word with its IPA, POS, translation, grammatical notes, and morphological connections.
- **Contextual Sentence Library**: For each word, show the simple and advanced sentences with translations.
- **Mnemonic Hooks**: Detailed memory-retrieval helpers.
- **Spaced Repetition Schedule**: A detailed weekly plan showing exactly which days to introduce new words and when to perform reviews.
</output_format>

Please construct the vocabulary acquisition plan now.

## Variables
- {TARGET_LANGUAGE} – The language the student is trying to learn (e.g., Spanish, Japanese, German).
- {CURRENT_LEVEL} – The student's current proficiency level (e.g., A2, Intermediate-Low).
- {TARGET_LEVEL} – The student's target proficiency level (e.g., B2, Advanced-Mid).
- {THEMATIC_FOCUS} – The topic, situation, or professional domain (e.g., Business Negotiations, Medical Terminology, Academic Writing, Casual Conversation).
- {STUDY_HOURS} – The number of hours per week the student can dedicate to study.
- {VOCABULARY_COUNT} – Number of core words/phrases to generate in the list (e.g., 10, 15, 20).
- {MNEMONIC_COUNT} – Number of difficult terms for which to provide mnemonic hooks (e.g., 3, 5).

## Notes
- Works exceptionally well for specialized terminology (e.g., legal or medical terms in a foreign language).
- Encourage the student to export the vocabulary bank into flashcard software like Anki.
- For non-Latin scripts (e.g., Japanese, Chinese, Arabic), the prompt automatically includes native script, romanization, and phonetic transcription.
