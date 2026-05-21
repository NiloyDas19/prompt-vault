---
title: "Subject Line Optimizer"
category: Marketing & Sales
subcategory: Email Marketing
tags: [email, subject-lines, open-rate, A/B-testing, optimization]
model: any
---

## Purpose
Generate high-open-rate email subject lines using proven psychological triggers, with A/B testing recommendations.

## Prompt
Generate 30 email subject line variations for the following email campaign. Optimize for maximum open rates.

**Email Topic:** {EMAIL_TOPIC}
**Audience:** {AUDIENCE}
**Email Type:** {EMAIL_TYPE}
**Brand Voice:** {BRAND_VOICE}
**Key Offer or News:** {KEY_MESSAGE}
**Sending Day/Time:** {SEND_TIME}

Generate 5 subject lines for each psychological trigger:

1. **Curiosity Gap** — Hint at something without revealing it ("You won't believe what we found...")
2. **Urgency/Scarcity** — Time pressure or limited supply ("Only 12 hours left")
3. **Personalization** — Use their name, company, or behavior ("{{FirstName}}, you left something behind")
4. **Social Proof** — Leverage numbers or authority ("Why 10,000+ marketers read this")
5. **Direct Benefit** — State exactly what they get ("Get our 2024 marketing playbook — free")
6. **Question** — Ask something they can't resist answering ("Are you making this SEO mistake?")

For each subject line:
- Character count (aim for under 50 characters for mobile)
- Whether to use an emoji (and which one)
- Preview text suggestion (the "second subject line" shown in the inbox)
- Predicted open rate impact: Low / Medium / High

Then provide:
- **Top 3 picks** with reasoning
- **A/B test plan**: Which 2 subject lines to test first, what sample size, and how long to run the test
- **Subject lines to AVOID** and why (e.g., spam trigger words, all caps, misleading clickbait)

## Variables
- {EMAIL_TOPIC} – What the email is about
- {AUDIENCE} – Who's receiving it (e.g., "existing customers", "cold leads", "newsletter subscribers")
- {EMAIL_TYPE} – Type (e.g., "promotional", "newsletter", "transactional", "re-engagement")
- {BRAND_VOICE} – Tone (e.g., "witty and casual", "professional", "bold and urgent")
- {KEY_MESSAGE} – The core message or offer
- {SEND_TIME} – When it will be sent (timing can affect subject line strategy)

## Notes
- Spam trigger words to avoid: "FREE!!!", "Act Now!!!", "Limited Time Offer", excessive caps, and multiple exclamation marks.
- Subject lines with 6–10 words perform best on average.
- Preview text is just as important as the subject line — don't waste it with "View in browser."
