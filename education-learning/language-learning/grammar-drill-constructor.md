---
title: "Custom Grammar Drill Constructor"
category: Education & Learning
subcategory: Language Learning & Linguistics
tags: [grammar, grammar-drill, worksheets, language-exercises, curriculum-design]
model: any
---

## Purpose
Constructs custom grammar worksheets with diverse question types, a brief rule explanation, and a detailed answer key with pedagogical explanations for a specified language and topic.

## Prompt
You are an expert curriculum developer and foreign language grammarian. Your task is to generate a comprehensive, highly targeted grammar drill worksheet and a corresponding detailed answer key.

<context>
- Target Language: {TARGET_LANGUAGE}
- Target Level (CEFR/ACTFL): {TARGET_LEVEL}
- Specific Grammar Topic: {GRAMMAR_TOPIC}
- Number of Exercises: {EXERCISE_COUNT}
</context>

<instructions>
1. **Grammar Concept Brief**:
   - Provide a concise, crystal-clear explanation of the target grammar rules, including sentence formulas, common triggers/indicators, and typical mistakes made by non-native speakers.
   - Use comparison tables or structured bullets to make the rules easy to digest.

2. **Targeted Exercise Blocks**:
   Create {EXERCISE_COUNT} distinct exercise blocks. To ensure comprehensive testing of the concept, use varied exercise types:
   - **Form Recognition (e.g., Fill-in-the-blank, conjugation tables, or multiple-choice)**: Focus on the mechanics of the target grammar.
   - **Sentence Transformation (e.g., rewrite active to passive, combine two clauses, convert direct to indirect, or change tenses)**: Focus on syntax manipulation.
   - **Error Detection & Correction**: Present sentences with common learner errors for the student to identify and fix.
   - **Contextual Translation (English to Target Language)**: Focus on active synthesis and production.

3. **Separate Answer Key & Explanations**:
   - Provide a complete and clear answer key at the very bottom.
   - For *every single question*, explain *why* the correct answer is right and clarify the specific grammatical cue or rule that dictates it (e.g., "We use subjunctive here because of the expression of emotion 'me alegro de que...'").
</instructions>

<output_format>
Format the output clearly into three distinct markdown sections:
- **Concept Brief & Formula**: The pedagogical explanation for the student.
- **Grammar Drill Worksheet**: The student-facing worksheet (free of answers, formatted with clear instructions and blanks for completion).
- **Pedagogical Answer Key**: Complete solutions with detailed grammatical explanations and troubleshooting tips for common mistakes.
</output_format>

Please generate the grammar constructor files now.

## Variables
- {TARGET_LANGUAGE} – The language the grammar drills should be designed for (e.g., Italian, Korean, Russian, ESL/English).
- {TARGET_LEVEL} – The proficiency level target (e.g., B1 - Intermediate, A2 - Elementary, C2 - Proficiency).
- {GRAMMAR_TOPIC} – The exact grammatical concept to focus on (e.g., "Distinction between Por and Para in Spanish", "German Adjective Endings after Definite/Indefinite Articles", "English Present Perfect vs. Past Simple").
- {EXERCISE_COUNT} – The number of exercise blocks to generate (typically 3 or 4, with 5 to 10 questions per block).

## Notes
- To adapt this for classroom use, copy and paste the Student Worksheet and Pedagogical Answer Key into separate documents.
- Encourage students to say the sentence transformations out loud to build acoustic familiarity with the correct structures.
- For non-Latin writing systems, exercises should include romanization (e.g., Pinyin, Romaji, Cyrillic transliteration) where appropriate for beginner levels.
