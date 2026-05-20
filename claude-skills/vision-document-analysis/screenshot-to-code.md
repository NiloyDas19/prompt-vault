---
title: "Screenshot to Code Converter"
category: Claude Skills
subcategory: Vision & Document Analysis
tags: [vision, screenshot-to-code, UI, multimodal, frontend, Claude-specific]
model: claude (vision-capable models only)
---

## Purpose
Convert a UI screenshot or design mockup into clean, functional HTML/CSS/JavaScript (or other framework) code that matches the design as closely as possible.

## Prompt
Look at the attached UI screenshot carefully. Your goal is to convert it into production-quality code that faithfully replicates the layout, colors, typography, spacing, and interactive elements shown.

<code_requirements>
- Target framework / language: {TARGET_FRAMEWORK} (e.g., HTML + vanilla CSS, React + Tailwind, Vue 3 + SCSS, Flutter)
- Responsiveness: {RESPONSIVENESS} (e.g., desktop-only, mobile-first responsive, fixed 375px mobile)
- Interactivity level: {INTERACTIVITY} (e.g., static HTML only, basic hover states, fully interactive with state management)
- Accessibility: {ACCESSIBILITY} (e.g., WCAG 2.1 AA compliant, semantic HTML only, not a requirement)
</code_requirements>

<observations_first>
Before writing any code, describe what you see:
1. Overall layout structure (grid, flex, columns)
2. Color palette (list hex/rgb estimates for each color)
3. Typography (font size estimates, weights, families if identifiable)
4. All interactive elements (buttons, inputs, dropdowns, toggles)
5. Spacing patterns (margins, padding, gaps)
</observations_first>

Then write the complete code:
- Use semantic HTML elements
- Extract colors and font sizes as CSS custom properties / design tokens
- Add placeholder text/images where content is shown
- Comment non-obvious layout decisions
- Ensure the result is self-contained and runnable

[ATTACH SCREENSHOT HERE]

## Variables
- {TARGET_FRAMEWORK} – What code to generate (HTML/CSS, React, Vue, Flutter, SwiftUI, etc.)
- {RESPONSIVENESS} – How responsive the code should be
- {INTERACTIVITY} – Level of interactivity to implement
- {ACCESSIBILITY} – Accessibility requirements

## Notes
- 👁️ Requires vision-capable Claude model.
- For complex multi-screen apps, analyze one screen at a time.
- If design tokens / a design system are in use, add "Use these design tokens: {TOKEN_LIST}" to ensure consistency.
- Claude estimates colors visually — always verify hex codes against your actual design file.
