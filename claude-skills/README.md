# 🤖 Claude Skills

> **36 prompts purpose-built for Claude's unique capabilities** — extended thinking, 200K context, vision, agentic workflows, prompt engineering, and more.

> [!IMPORTANT]
> **This category is Claude-specific.** While most prompts in this vault are model-agnostic, Claude Skills prompts are designed to leverage Claude's unique features. Prompts that require specific Claude capabilities are flagged with icons (see legend below).

---

## 🏷️ Capability Icons

| Icon | Meaning |
|---|---|
| 🧠 | Requires **Extended Thinking** mode (Claude 3.7 Sonnet+) |
| 📎 | Requires **Long Context** window (200K tokens — Claude.ai Pro/Team or API) |
| 👁️ | Requires **Vision** capability (Claude 3 Sonnet, Opus, Haiku+) |
| ⚡ | **Agentic** prompt — designed for multi-step autonomous workflows |
| 🔧 | **Prompt Engineering** — a meta-prompt for building better Claude prompts |

---

## 📂 Subcategories

| Subcategory | Prompts | Key Capability |
|---|---|---|
| [Extended Thinking](#-extended-thinking) | 6 | 🧠 Deep reasoning before answering |
| [Long Context Mastery](#-long-context-mastery) | 5 | 📎 200K token window |
| [Prompt Engineering for Claude](#-prompt-engineering-for-claude) | 6 | 🔧 Better Claude prompts |
| [Vision & Document Analysis](#-vision--document-analysis) | 4 | 👁️ Image and visual inputs |
| [Agentic Workflows](#-agentic-workflows) | 4 | ⚡ Multi-step automation |
| [Persona & Role Design](#-persona--role-design) | 4 | Claude as any expert |
| [Conversation Design](#-conversation-design) | 3 | Structured multi-turn dialogues |
| [Writing with Claude](#-writing-with-claude) | 4 | Writing and editing workflows |

---

## 🧠 Extended Thinking

> Enable Extended Thinking in Claude 3.7 Sonnet for best results on these prompts. It gives Claude a dedicated reasoning budget — like letting it think before speaking.

### [Deep Problem Solver](./extended-thinking/deep-problem-solver.md) 🧠
Multi-step structured approach to complex, multi-variable problems with visible reasoning and confidence scoring.
> **Best for:** Wicked problems, strategic decisions, complex analysis that needs more than a surface answer

### [Ethical Dilemma Reasoner](./extended-thinking/ethical-dilemma-reasoner.md) 🧠
Reasons through ethical dilemmas from four moral frameworks (consequentialism, deontology, virtue, care ethics) to a nuanced position.
> **Best for:** Business ethics decisions, policy design, philosophy, moral questions with real stakes

### [Decision Matrix Builder](./extended-thinking/decision-matrix-builder.md)
Builds a weighted, scored decision matrix with sensitivity analysis to reveal what would flip the decision.
> **Best for:** High-stakes decisions with multiple options and competing criteria

### [Logical Argument Validator](./extended-thinking/argument-validator.md) 🧠
Reconstructs an argument in formal logic, checks validity and soundness, names fallacies, and provides a steelman version.
> **Best for:** Evaluating arguments, debate prep, research paper review, catching manipulative reasoning

### [Research Hypothesis Generator](./extended-thinking/research-hypothesis-generator.md) 🧠
Generates 8–10 candidate hypotheses, screens for testability and novelty, and produces full H₀/H₁ pairs for the top 3.
> **Best for:** Academic research, UX research, market research, scientific investigation

### [Multi-Angle Analyst](./extended-thinking/multi-angle-analysis.md) 🧠
Analyzes any situation from multiple stakeholder perspectives simultaneously, surfacing hidden agendas and synthesizing common ground.
> **Best for:** Pre-negotiation prep, policy design, product launches, stakeholder management

---

## 📎 Long Context Mastery

> These prompts are designed to use Claude's full 200K token context window — paste entire codebases, books, or document sets at once.

### [Codebase Navigator](./long-context/codebase-navigator.md) 📎
Load an entire codebase into context, get architectural analysis, code smell detection, and expert answers about any part of it.
> **Best for:** New engineer onboarding, security audits, understanding inherited code

### [Document Distiller](./long-context/document-distiller.md) 📎
Extract executive summary, key findings, quantitative data, action items, and missing information from any long document.
> **Best for:** Long reports, white papers, research documents, lengthy emails or memos

### [Cross-Document Synthesizer](./long-context/cross-document-synthesizer.md) 📎
Load multiple documents simultaneously and synthesize themes, contradictions, and unique contributions across all of them.
> **Best for:** Literature reviews, competitive intelligence, due diligence, multi-source research

### [Contract & Legal Document Reviewer](./long-context/contract-reviewer.md) 📎
Review a full contract in plain language — surfacing obligations, risk flags, missing protections, and negotiation priorities.
> **Best for:** Service agreements, NDAs, employment contracts, SaaS terms — *before signing*

### [Full Book Analyzer](./long-context/book-analyzer.md) 📎
Load an entire book for comprehensive analysis: thesis, structure map, key ideas, argument evaluation, and actionable takeaways.
> **Best for:** Non-fiction analysis, research, book clubs, extracting value from dense texts quickly

---

## 🔧 Prompt Engineering for Claude

> Meta-prompts for building, debugging, and optimizing your Claude prompts. Claude helps you become a better Claude user.

### [System Prompt Architect](./prompt-engineering/system-prompt-architect.md) 🔧
Design a complete, production-ready system prompt for a Claude-powered application with persona, guidelines, hard limits, and stress tests.
> **Best for:** Building Claude-powered products, APIs, chatbots, or custom assistants

### [XML Structured Prompt Builder](./prompt-engineering/xml-structured-prompt-builder.md) 🔧
Convert an underperforming prompt into a well-structured, XML-tagged Claude prompt with a before/after comparison and rationale.
> **Best for:** Improving any Claude prompt that's producing inconsistent or low-quality outputs

### [Few-Shot Example Designer](./prompt-engineering/few-shot-example-designer.md) 🔧
Design high-quality, diverse few-shot examples that lock in the exact tone, format, and quality level you need from Claude.
> **Best for:** Any task requiring consistent format, tone, or structure across many outputs

### [Prompt Debugger & Optimizer](./prompt-engineering/prompt-debugger.md) 🔧
Diagnose why a Claude prompt is underperforming, identify root causes, and produce an improved version with a full change log.
> **Best for:** Prompts that produce wrong tone, wrong format, ignored instructions, or inconsistent results

### [Chain-of-Thought Prompt Designer](./prompt-engineering/chain-of-thought-prompter.md) 🔧
Design a step-by-step CoT prompt that forces Claude to reason visibly before answering, dramatically improving accuracy on complex tasks.
> **Best for:** Classification, mathematical reasoning, multi-step logic, any accuracy-critical task

### [Claude Persona Designer](./prompt-engineering/role-persona-designer.md) 🔧
Design a richly detailed, consistent Claude persona with behavioral rules, edge case handling, sample dialogue, and a ready-to-paste system prompt block.
> **Best for:** Building AI-powered products, chatbots, or custom assistants with a specific character

---

## 👁️ Vision & Document Analysis

> Prompts for Claude's multimodal vision capabilities. Attach images, screenshots, diagrams, or charts.

### [Deep Image Analyzer](./vision-document-analysis/image-analyzer.md) 👁️
Thorough, structured image analysis — subject description, text extraction, contextual interpretation, and confidence flags.
> **Best for:** Analyzing any image with precision and structured output

### [Screenshot to Code](./vision-document-analysis/screenshot-to-code.md) 👁️
Convert a UI screenshot or design mockup into clean, functional HTML/CSS/JS or any framework code with color token extraction.
> **Best for:** Rapid frontend prototyping, digitizing Figma/Sketch mockups without exporting

### [Chart & Graph Data Extractor](./vision-document-analysis/chart-data-extractor.md) 👁️
Extract all data points from charts and graphs into a clean table, with trend analysis and CSV-ready format.
> **Best for:** Working with charts in PDFs, slide decks, or reports where you need the underlying data

### [Diagram & Whiteboard Interpreter](./vision-document-analysis/diagram-interpreter.md) 👁️
Interpret technical diagrams, whiteboard photos, or flowcharts and convert them to Mermaid code, PlantUML, JSON, or text.
> **Best for:** Digitizing whiteboard sessions, interpreting inherited diagrams, converting drawings to code

---

## ⚡ Agentic Workflows

> Prompts designed for multi-step autonomous operation — Claude plans, executes, evaluates, and iterates without constant human intervention.

### [Agentic Task Decomposer](./agentic-workflows/agentic-task-decomposer.md) ⚡
Break a complex goal into an ordered plan of atomic tasks with dependencies, failure modes, checkpoints, and a rollback plan.
> **Best for:** Complex projects, automation planning, building agentic Claude pipelines

### [Self-Critic & Output Refiner](./agentic-workflows/self-critic-output-refiner.md) ⚡
Claude generates an output, rigorously critiques it against your criteria, then produces an improved version — all in one prompt.
> **Best for:** Reducing human review cycles, high-quality content generation, enforcing quality standards

### [Iterative Research Workflow](./agentic-workflows/iterative-research-workflow.md) ⚡
A six-stage research workflow: scoping → foundation → deep analysis → synthesis → gaps → final deliverable.
> **Best for:** Comprehensive research on complex topics requiring structured, multi-layered analysis

### [Prompt Chain Orchestrator](./agentic-workflows/prompt-chain-orchestrator.md) ⚡
Design a multi-step prompt chain where each Claude call feeds the next, with data flow design, error handling, and implementation pseudocode.
> **Best for:** Building production Claude pipelines, multi-stage content workflows, automated research systems

---

## 🎭 Persona & Role Design

> Prompts that turn Claude into a specific expert, character, or facilitator for specialized conversations.

### [Socratic Teacher](./persona-role-design/socratic-teacher.md)
Claude teaches any topic through strategic questions rather than direct explanation — guiding you to insights through your own reasoning.
> **Best for:** Deep conceptual understanding, exam prep, philosophy, any topic where insight > memorization

### [Devil's Advocate](./persona-role-design/devils-advocate.md)
Claude argues the strongest possible case AGAINST your idea or plan — with evidence, assumption attacks, and a worst-case scenario.
> **Best for:** Stress-testing plans, pitch preparation, publishing controversial views, major decisions

### [Expert Panel Simulator](./persona-role-design/expert-panel-simulator.md)
Simulate a panel of 3–5 domain experts giving simultaneous perspectives on a problem, with cross-expert dialogue.
> **Best for:** Multi-domain decisions, getting diverse expert input in one session, advisory board simulation

### [Interview Simulator](./persona-role-design/interview-simulator.md)
Realistic job interview simulation with probing follow-ups, then detailed feedback on every answer and coaching tips.
> **Best for:** Job interview preparation, practicing behavioral and technical questions, building confidence

---

## 💬 Conversation Design

> Structured multi-turn conversation templates for coaching, discovery, and debate.

### [Requirements Gathering Conversation](./conversation-design/requirements-gatherer.md)
Claude acts as a consultant and systematically uncovers all project requirements through smart, progressive questioning.
> **Best for:** Project scoping, product discovery, client onboarding, defining deliverables before execution

### [Coaching Session Facilitator](./conversation-design/coaching-session-facilitator.md)
Claude runs a GROW-model (or other framework) coaching session — asking powerful questions, reflecting, and securing action commitments.
> **Best for:** Career decisions, leadership challenges, goal-setting, personal development

### [Structured Debate Partner](./conversation-design/structured-debate-partner.md)
Claude argues a specific position with full rigor following formal debate rules, then gives post-debate coaching.
> **Best for:** Debate prep, sharpening persuasive arguments, exploring controversial topics, presentation rehearsal

---

## ✍️ Writing with Claude

> Prompts that leverage Claude's writing capabilities with precision and consistency.

### [Writing Voice Matcher](./writing-with-claude/voice-matcher.md)
Analyzes your writing samples across 7 dimensions and writes new content in your exact voice — indistinguishable from your own work.
> **Best for:** Ghostwriting, scaling content creation, maintaining brand voice consistency

### [Multi-Format Content Repurposer](./writing-with-claude/multi-format-repurposer.md)
Takes one source piece and produces multiple format-optimized versions simultaneously (LinkedIn, newsletter, thread, script, etc.).
> **Best for:** Content strategy, maximizing reach of a single piece, consistent cross-platform messaging

### [Tone & Audience Adapter](./writing-with-claude/tone-audience-adapter.md)
Rewrites content for a completely different audience or reading level, with a vocabulary change log and structural rationale.
> **Best for:** Technical docs → executive summaries, academic → blog, legal text → plain language

### [Style Guide Enforcer](./writing-with-claude/style-guide-enforcer.md)
Edits content to perfectly conform to AP, Chicago, APA, or your custom style guide, flagging every change with a rule citation.
> **Best for:** Final editing pass, maintaining brand consistency, learning a new style guide

---

## 💡 Pro Tips for Claude-Specific Prompting

1. **Use XML tags** — Claude is fine-tuned to parse `<instructions>`, `<context>`, `<task>` tags reliably
2. **Enable Extended Thinking** — For 🧠 prompts, toggle Extended Thinking in Claude.ai or set `thinking: {budget_tokens: N}` in the API
3. **Max out the context window** — For 📎 prompts, paste entire files — Claude handles 200K tokens
4. **Chain prompts** — Combine prompts sequentially for complex workflows (e.g., Requirements → API Design → Code Review)
5. **Be direct** — Claude performs best with explicit, specific instructions rather than hints

---

*Part of the [Prompt Vault](../../README.md) open-source prompt library.*
