---
title: "Diagram & Whiteboard Interpreter"
category: Claude Skills
subcategory: Vision & Document Analysis
tags: [vision, diagrams, whiteboard, architecture, flowchart, Claude-specific]
model: claude (vision-capable models only)
---

## Purpose
Interpret technical diagrams, whiteboard sketches, flowcharts, or architecture drawings and convert them into structured text, code, or digital diagram formats.

## Prompt
Carefully examine the diagram or whiteboard image I've attached. Your goal is to fully understand and digitize it.

<interpretation_task>
- Diagram type: (you determine from the image)
- What I need: {OUTPUT_GOAL} (e.g., written description, Mermaid code, PlantUML, structured text list, JSON representation)
- Domain context: {DOMAIN} (e.g., software architecture, business process, network topology, data flow, org chart)
</interpretation_task>

Please:
1. **Identify the diagram type** — What kind of diagram is this? (flowchart, ERD, sequence diagram, mind map, network diagram, etc.)
2. **Read all text** — Transcribe every label, annotation, and text element exactly as written
3. **Map the structure** — List all nodes/elements and their connections/relationships
4. **Describe the flow/logic** — Explain what this diagram depicts in plain language
5. **Generate digital format** — Convert to {OUTPUT_GOAL}:
   - If Mermaid: produce valid `mermaid` code block
   - If text: use a clear hierarchical or list format
   - If JSON: produce a valid graph/tree structure
6. **Gaps and assumptions** — Note anything illegible, ambiguous, or assumed

[ATTACH DIAGRAM / WHITEBOARD PHOTO HERE]

## Variables
- {OUTPUT_GOAL} – Desired output format (Mermaid diagram, PlantUML, plain text description, JSON, etc.)
- {DOMAIN} – The technical or business domain this diagram is from

## Notes
- 👁️ Requires vision-capable Claude model.
- For blurry or hand-drawn whiteboard photos, Claude will make its best interpretation — always review the output.
- Follow up with "Convert this to a Mermaid flowchart" or "Generate a sequence diagram from this" to reformat.
- Works well for digitizing meeting whiteboard photos before erasing.
