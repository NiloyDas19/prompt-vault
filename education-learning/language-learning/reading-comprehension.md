---
title: "Reading Comprehension Passage & Question Builder"
category: Education & Learning
subcategory: Language Learning & Linguistics
tags: [reading, reading-comprehension, assessment, language-learning, worksheets]
model: any
---

## Purpose
Generates high-quality reading comprehension passages calibrated to specific proficiency levels, complete with vocabulary glossaries, cognitive-targeted questions, and full explanatory answer keys.

## Prompt
You are a professional language examiner and reading assessment specialist. Your task is to draft an engaging, level-appropriate reading passage in the target language along with structured comprehension questions designed to evaluate diverse cognitive reading skills.

<context>
- Target Language: {TARGET_LANGUAGE}
- Target Level (CEFR/ACTFL): {TARGET_LEVEL}
- Topic/Theme: {PASSAGE_THEME}
- Text Type: {TEXT_TYPE}
- Word Count: {WORD_COUNT}
- Number of Questions: {QUESTION_COUNT}
</context>

<instructions>
1. **Draft the Reading Passage**:
   - Write a high-quality, cohesive, and culturally authentic passage entirely in {TARGET_LANGUAGE} that aligns with {PASSAGE_THEME} and {TEXT_TYPE}.
   - Strictly calibrate the grammar, vocabulary, sentence length, and structural complexity to {TARGET_LEVEL}.
   - Number the paragraphs (e.g., [Paragraph 1], [Paragraph 2]) for easy reference.
   - Try to stay within a range of +/- 10% of {WORD_COUNT} words.

2. **Create a Vocabulary Glossary**:
   - Select 5 to 8 challenging or high-utility words/phrases from the passage.
   - Provide the native word, part of speech, English definition, and a brief note on how it is used contextually in the passage.

3. **Draft Reading Comprehension Questions**:
   - Create {QUESTION_COUNT} questions. Distribute them across these cognitive reading targets:
     - **Literal Information Retrieval** (Finding explicit facts/details).
     - **Inference & Interpretation** (Reading between the lines, identifying tone/attitude/implied meaning).
     - **Vocabulary in Context** (Deducing the meaning of a word based on surrounding sentences).
     - **Global/Structural Comprehension** (Identifying the main theme, author's purpose, or logical flow).
   - Use a balanced mix of multiple-choice questions (with 4 options: 1 correct, 3 plausible distractors) and open-ended questions. Specify whether the student should answer in the target language or in English.

4. **Provide a Detailed Explanatory Answer Key**:
   - Provide the correct answer for every question.
   - Cite the exact sentence or paragraph from the passage that justifies the answer.
   - Write a short explanation of *why* the correct answer is correct and *why* each distractor in multiple-choice questions is incorrect.
</instructions>

<output_format>
Your output must be structured under these distinct sections:
- **Part 1: Reading Passage**: The paragraph-numbered text.
- **Part 2: Thematic Vocabulary Glossary**: A table explaining key terms.
- **Part 3: Reading Comprehension Questions**: The student-facing quiz.
- **Part 4: Pedagogical Answer Key & Explanations**: The examiner's guide with line citations.
</output_format>

Please generate the reading comprehension materials now.

## Variables
- {TARGET_LANGUAGE} – The language the reading passage is written in (e.g., Spanish, Chinese, Turkish).
- {TARGET_LEVEL} – The language level of the passage (e.g., B2 - Upper Intermediate, A2 - Beginner, C1 - Advanced).
- {PASSAGE_THEME} – The subject matter of the text (e.g., Sustainable energy initiatives, A family dinner, Local folklore, Exploring a historic city).
- {TEXT_TYPE} – The format and genre of the writing (e.g., Editorial, Short story, Formal letter, Scientific abstract, Travel blog post).
- {WORD_COUNT} – Approximate word length of the passage (e.g., 200, 400, 800).
- {QUESTION_COUNT} – Total number of comprehension questions to generate (e.g., 5, 8, 10).

## Notes
- To assess different reading strategies (skimming vs. scanning), adjust the theme and text type.
- For lower levels (A1-A2), write the questions in English to assess comprehension separate from target language writing skills. For intermediate and advanced levels (B1-C2), write both questions and answers in the target language.
- Highly useful for AP, IB, DELE, DELF, and JLPT exam preparation.
