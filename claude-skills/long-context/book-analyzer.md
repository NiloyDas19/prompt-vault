---
title: "Full Book Analyzer"
category: Claude Skills
subcategory: Long Context Mastery
tags: [long-context, books, analysis, reading, summarization]
model: claude (200K context window)
---

## Purpose
Load an entire book or long report and get a comprehensive analysis including themes, arguments, structure, and actionable takeaways.

## Prompt

I am sharing the full text of a book with you. Read it completely before responding.

<book_text>
{FULL_BOOK_TEXT}
</book_text>

<book_metadata>
- Title: {TITLE}
- Author: {AUTHOR}
- Genre / type: {GENRE}
- Why I'm reading it: {READING_PURPOSE}
</book_metadata>

Provide a comprehensive analysis:
1. **Core thesis / central argument** — What is the author's main claim or message?
2. **Structure map** — How is the book organized? What does each section/chapter do?
3. **Key ideas** — The 7–10 most important concepts or insights, each with a supporting quote
4. **Argument evaluation** — Is the author's reasoning sound? What evidence do they use? Where is the argument weakest?
5. **Practical takeaways** — 5 specific, actionable things I can do or change based on this book
6. **Criticisms / counterarguments** — What are the strongest objections to the author's thesis?
7. **Best quotes** — 5 memorable, shareable quotes
8. **Who should read this** — and who would find it least useful
9. **Related books** — 3 books that complement or challenge this one

## Variables
- `{FULL_BOOK_TEXT}` – Paste the full text (works best for shorter books up to ~150K tokens)
- `{TITLE}` – Book title
- `{AUTHOR}` – Author name
- `{GENRE}` – Genre or category (e.g., business, science, memoir, philosophy)
- `{READING_PURPOSE}` – Why you're reading it (shapes what counts as a useful takeaway)

## Notes
- 📎 Works best for books up to ~150K tokens within Claude's 200K context window.
- For longer books, paste the most important chapters and specify "This is chapters 1–7 of a 15-chapter book."
- Add "Compare this to {OTHER_BOOK}" if you've already loaded another book in context.
