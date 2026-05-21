---
title: "Microcopy & UX Writing"
category: Marketing & Sales
subcategory: Copywriting
tags: [copywriting, ux-writing, microcopy, interface, product]
model: any
---

## Purpose
Write clear, helpful, and on-brand microcopy for app interfaces, error messages, tooltips, onboarding flows, and empty states.

## Prompt
Write microcopy for the following product interface. The copy should feel human, helpful, and reduce friction — not robotic or corporate.

**Product:** {PRODUCT_NAME}
**Brand Voice:** {BRAND_VOICE}
**Screen/Context:** {UI_CONTEXT}
**User's emotional state at this moment:** {USER_EMOTION}
**Constraints:** {CONSTRAINTS}

Generate microcopy for each of the following UI elements:

1. **Empty State** — What the user sees when there's no data yet (make it inviting, not depressing)
2. **Loading State** — What they see while waiting (make the wait feel shorter)
3. **Success Message** — Confirmation after completing an action (celebrate appropriately)
4. **Error Message** — When something goes wrong (be helpful, not blaming)
5. **Tooltip / Helper Text** — Explain a confusing feature in plain language
6. **Onboarding Step** — Guide the user through first-time setup
7. **Upgrade Prompt** — Nudge a free user toward a paid plan (without being annoying)
8. **Confirmation Dialog** — "Are you sure?" but better
9. **404 / Page Not Found** — Turn a frustrating moment into a brand moment
10. **Placeholder Text** — Input field placeholder that guides without confusing

For each, provide:
- The copy itself (keep it short — max 2 sentences per element)
- A brief note on the UX writing principle used (clarity, empathy, brevity, actionability)
- One alternative variation with a different tone

## Variables
- {PRODUCT_NAME} – Your product name
- {BRAND_VOICE} – Tone (e.g., "friendly and playful like Slack", "professional and calm like Linear", "quirky and fun like Mailchimp")
- {UI_CONTEXT} – The specific screen or feature (e.g., "project dashboard", "settings page", "checkout flow")
- {USER_EMOTION} – How they likely feel (e.g., "frustrated because something broke", "excited because they just signed up")
- {CONSTRAINTS} – Any limits (e.g., "max 50 characters for button text", "must include a link to support docs")

## Notes
- Microcopy is the difference between an app that feels frustrating and one that feels delightful.
- The golden rule of UX writing: "Would a helpful friend say it this way?"
- Error messages should always: (1) say what happened, (2) say why, (3) suggest what to do next.
