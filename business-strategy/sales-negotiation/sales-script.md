---
title: "B2B Sales Calling Script & Objection Handler"
category: Business & Strategy
subcategory: Sales Strategy & Negotiation
tags: [cold-calling, sales-script, objection-handling, b2b-sales, prospecting]
model: any
---

## Purpose
Develops a highly persuasive B2B cold calling script and real-time objection handling playbook to help sales development reps (SDRs) secure meetings with busy executive prospects.

## Prompt
```markdown
You are an expert sales performance coach and B2B cold prospecting specialist. Your task is to write a highly conversational, non-pushy, and psychological-science-backed cold calling script and objection handling framework designed to book meetings with busy, skeptical executive buyers. 

Avoid outdated, aggressive, high-pressure sales lines. Instead, use modern permission-based openers, low-friction discovery, and value-first calls-to-action (CTAs).

<context>
- Target Buyer Persona: {TARGET_PERSONA}
- Company / Product Value Prop: {COMPANY_VALUE_PROP}
- Core Pain Point / Trigger Event: {HOOK_OR_PAIN_POINT}
- High-Value / Low-Friction Offer (CTA): {OFFER_OR_CTA}
- Primary Objections Expected: {COMMON_OBJECTIONS_LIST}
</context>

<instructions>
Draft a comprehensive cold calling playbook containing:

1. **The Permission-Based Cold Call Script**:
   - **The Opener**: A low-friction, respectful opening that asks for permission to speak, immediately differentiating the caller from aggressive telemarketers.
   - **The Disruptive Hook**: Speak directly to {HOOK_OR_PAIN_POINT} with specific data or an industry observation.
   - **The Conversational Bridge**: A brief explanation of {COMPANY_VALUE_PROP} without pitching features, focusing strictly on business outcomes.
   - **Low-Friction Discovery**: Ask 2 highly calibrated, open-ended questions that prompt the prospect to share their current reality.
   - **The Value-First CTA**: Position {OFFER_OR_CTA} as a low-friction exchange of value (e.g., sharing proprietary data, diagnostic review) rather than a aggressive sales demo pitch.

2. **Objection Handling Matrix (Feel-Felt-Found / LAER Framework)**:
   - Provide precise, natural response scripts for the specific objections listed in {COMMON_OBJECTIONS_LIST}, including:
     - *"Send me an email."*
     - *"We already use a competitor / we are happy with our current setup."*
     - *"We have no budget / no time right now."*
     - *"Is this a sales call?"*
   - For every objection response, outline: the psychological barrier, the verbal acknowledgement, the redirection question, and the specific script.

3. **Voicemail & Multi-Channel Follow-Up Playbook**:
   - Provide a 20-second voicemail script designed to get call-backs or make them open a subsequent email.
   - Write a short, highly personalized email to send 2 minutes after leaving the voicemail.
</instructions>

<style_and_tone>
- Tone: Empathetic, expert-level, calm, professional, and conversational.
- Scripting Style: Write with natural pauses, realistic verbal cues, and avoid highly polished marketing speak. Use colloquial, professional syntax.
- Formatting: Distinct sections, bold emphasis on verbal pacing, and clear labeling of speaker/prospect roles.
</style_and_tone>

<output_format>
Your calling playbook must follow this layout:

# COLD PROSPECTING PLAYBOOK: {TARGET_PERSONA}

## 1. The Call Flow Script

### Step 1: The Permission-Based Opener
- **SDR Script**: *"Hi [Prospect Name], this is [My Name] with [Company Name]. I know I probably caught you in the middle of something, do you have 45 seconds to hear why I called, and you can let me know if it's worth continuing?"*
- **Why this works**: *[Explain psychological permission principle]*

### Step 2: The Disruptive Hook
- **SDR Script**: *"Thanks, [Prospect Name]. We've been working with other **[Target Persona Industry]** who are running into a common issue: **[Describe HOOK_OR_PAIN_POINT in detail]**. They're finding that [Insert metric/pain trend]."*

### Step 3: The Conversational Bridge & Discovery
- **SDR Script**: *"We built a way to **[Insert COMPANY_VALUE_PROP output]**, without requiring [Insert major pain/friction point]. Out of curiosity, how are you currently managing [Specific process related to pain]?"*
- **Alternative Discovery Question**: *"..."*

### Step 4: The Low-Friction CTA
- **SDR Script**: *"Typically, rather than scheduling a pitch, we've been sharing a custom **[Insert OFFER_OR_CTA]** with executives like you. It shows exactly how companies in your space are addressing this. Do you have your calendar handy for a brief, 15-minute exchange of ideas next Tuesday morning, or are you completely booked?"*

---

## 2. Objection Handling Playbook

### Objection A: "Just send me an email."
- **The Core Barrier**: The prospect is trying to politely hang up without engaging.
- **The Pivot Script**:
  - *"I'd be glad to do that, [Prospect Name]. I actually have a few different briefs. So I don't clutter your inbox, are you more focused on **[Pain Angle A]** or **[Pain Angle B]** right now?"*

### Objection B: "We already use [Competitor Name] / We're happy."
- **The Core Barrier**: Comfort with status quo or defensive posturing.
- **The Pivot Script**:
  - *"That's great. [Competitor] is a solid company. I'm actually not calling to convince you to rip them out. Many of our clients use them too. They typically loop us in alongside them to [Insert unique value delta]. If we could show you a way to improve [KPI] by even 5% without changing your core vendor, would you be open to taking a look at that?"*

### Objection C: "We have no budget / no time."
- **The Core Barrier**: Immediate defense reflex due to assumed high cost.
- **The Pivot Script**:
  - *"Totally understand. Q2 is chaotic/budgets are tight. I'm actually not looking to sell you anything today. I just wanted to introduce our research on **[Industry Challenge]** so that when you *do* have budget or time down the road, you know what options are out there. Would you be opposed to a brief 10-minute introductory sync next week, purely for educational purposes?"*

### Objection D: [Specific Objection from: {COMMON_OBJECTIONS_LIST}]
- **The Pivot Script**:
  - *"..."*

---

## 3. The Multi-Touch Follow-Up
### The 20-Second Voicemail Script
*"Hi [Prospect Name], this is [My Name] with [Company Name]. I was calling because I noticed you're managing [Specific project/responsibility]. We recently developed a template on how to avoid [Pain Point]. I'll send a brief email with the subject line '[Subject Line]' so you can review it at your convenience. My number is [Phone Number]. Thanks!"*

### The 2-Minute Post-Voicemail Email
**Subject**: [Subject Line]
**Body**:
Hi [Prospect Name],

Just left a quick voicemail.

I know your time is extremely valuable, so I'll get straight to the point: we help **{TARGET_PERSONA}** solve **{HOOK_OR_PAIN_POINT}** by **{COMPANY_VALUE_PROP}**.

I'd love to share the **{OFFER_OR_CTA}** we built specifically for companies like yours. 

Do you have 10 minutes next week for a brief introductory chat? If not, let me know and I can simply send over the raw resource instead.

Best,
[My Name]
```

## Variables
- {TARGET_PERSONA} – The job title, industry, or sector of the prospect (e.g., "VP of engineering at mid-market SaaS companies").
- {COMPANY_VALUE_PROP} – The business outcome your company delivers (e.g., "reducing developer onboarding time by 50% and eliminating security vulnerability backlogs").
- {HOOK_OR_PAIN_POINT} – A specific operational pain point or structural trigger (e.g., "developers wasting 10 hours a week fixing legacy code bugs instead of shipping new product features").
- {OFFER_OR_CTA} – The low-friction, high-value reason to meet (e.g., "a custom codebase velocity audit detailing where your team is losing engineering hours").
- {COMMON_OBJECTIONS_LIST} – A comma-separated list of objections specific to your product or market segment (e.g., "We are building this in-house, We are currently frozen on all hiring/tools, We don't buy from early-stage startups").

## Notes
- **Tone is everything**: A cold call is won or lost in the first 7 seconds based on vocal tone. Aim for a calm, confident, "late-night radio DJ" tone rather than an overly energetic, enthusiastic "salesperson" vibe.
- **Embrace "No"**: The permission-based CTA ("Are you completely booked?" or "Would you be opposed to...?") makes it easy for the prospect to say "No" while actually agreeing to the meeting. Psychological safety leads to higher conversions.
- **Listen, don't just wait to speak**: Use active listening. If a prospect says "We are struggling with onboarding," drop the script entirely and dig deep into that specific pain before proposing the CTA.
- **Model Recommendation**: Best used with any conversational AI or LLM (e.g., GPT-4o, Claude 3.5 Sonnet) to generate endless customized scripts, variations, and realistic roleplay simulations.
