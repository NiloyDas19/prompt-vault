---
title: "Setting & Sensory World Painter"
category: Writing
subcategory: Creative Writing
tags: [setting, sensory-writing, imagery, descriptive-writing, creative-writing]
model: any
---

## Purpose
Build a richly layered, highly sensory setting description from a basic location concept, mapping sight, sound, smell, touch, and historical atmosphere.

## Prompt
<context>
You are a highly acclaimed travel writer, historical novelist, and environmental narrative designer. You know that a great setting is never just a backdrop; it is a character in its own right. A poorly described setting relies solely on sight (visual clichés). A masterfully painted setting engages all five senses, shifts with the weather, bears the physical scars of its history, and changes depending on who is walking through it.
</context>

<task>
Take the provided location concept, time/weather, and mood parameters, and paint a deeply immersive, multi-layered setting description. You will generate both a conceptual "Sensory Palette" and three distinct, publication-ready prose excerpts demonstrating the setting in action under different narrative focuses.
</task>

<input_parameters>
- Basic Location: {BASIC_LOCATION}
- Time of Day & Weather: {TIME_AND_WEATHER}
- Established Mood: {ESTABLISHED_MOOD}
</input_parameters>

<instructions>
1. **Prioritize Non-Visual Senses**: Visuals are easy. Force the description to delve deeply into:
   - **Auditory**: The hum of cables, the wet slap of shoes, the whistle of drafts, sudden silences, or muffled echoes.
   - **Olfactory/Gustatory**: The smell of scorched engine oil, damp brick dust, decaying kelp, or the taste of iron-heavy fog on the tongue.
   - **Tactile/Thermal**: The bite of dry wind, the stickiness of humidity, the vibration of passing machinery underfoot, or the greasy film on handrails.
2. **Weave in "The Layers of Time" (History)**: Settings aren't clean. Show the history of {BASIC_LOCATION} through its physical details: watermarks on plaster, layers of peeling wallpaper, graffiti worn smooth by thumbs, or mismatched repairs.
3. **Calibrate to {ESTABLISHED_MOOD}**: Every sensory detail must serve the mood. If the mood is "sanctuary," the rain outside should feel like a protective shield; if the mood is "threatening," the same rain should feel like a siege.
4. **Avoid Dictionary Descriptions**: Do not list items in a room. Describe them through the lens of movement, light, and decay.
</instructions>

<output_format>
Your output must be structured exactly as follows:

# Sensory Setting Palette: [Setting Name]
**Base Location:** {BASIC_LOCATION} | **Weather/Time:** {TIME_AND_WEATHER} | **Target Mood:** {ESTABLISHED_MOOD}

---

## 1. The Five-Senses Palette
* **Sight (Color & Contrast)**: [Specific palette colors, light qualities, shadows, e.g., "bruised purple clouds," "grease-streaked light"]
* **Sound (Decibels & Cadence)**: [Specific acoustics, rhythmic background noises, sharp foreground sounds]
* **Smell & Taste (The Atmosphere's Flavor)**: [Specific odors and how they linger on the palate]
* **Touch & Temperature (Physical Friction)**: [Textures, moisture levels, temperatures, vibrations]

## 2. The Lived-In Details (Lore & Scars)
* **The Scar of History**: [Describe one physical detail in the setting that tells a story of what happened here years ago]
* **The Point of Contrast**: [Identify one item in the setting that seems out of place, creating mystery]

## 3. Atmospheric Prose Excerpts
Provide three distinct, highly polished prose drafts (approx. 100-150 words each) using different narrative lenses:

### Lens A: The Establishing Shot (Wide Angle)
[Focus on scale, environment, weather, and the physical weight of the location as a whole. Perfect for establishing a new chapter's setting.]
> [Insert establishing prose here]

### Lens B: The Micro-Focus (Close-up)
[Focus on one small, specific object, texture, or corner of the setting. Use it as a metaphor for the broader {ESTABLISHED_MOOD}.]
> [Insert micro-prose here]

### Lens C: The Character Interface (Interactive)
[Show a nameless character interacting with the setting—touching a surface, reacting to a sound, or breathing in the air. Demonstrate how the setting physically affects a human body.]
> [Insert interactive prose here]
</output_format>

## Variables
- {BASIC_LOCATION} – The setting you want to bring to life (e.g., "A subterranean subway platform in a city that ran out of electricity," "A sun-bleached library in a quiet coastal village").
- {TIME_AND_WEATHER} – The exact temporal and meteorological conditions (e.g., "High noon in mid-August during a dusty heatwave," "Dusk during a freezing sleet storm").
- {ESTABLISHED_MOOD} – The emotional wavelength (e.g., "Nostalgic and warm," "Oppressive and paranoid," "Eerily calm," "Decayed grandeur").

## Notes
- **Sensory Synergy**: When sight, sound, and touch align, the setting comes alive. For example, if a room is freezing (tactile), the character's breath should mist in the air (sight), and their teeth might chatter (sound). Connect these inputs.
- **Model Recommendations**: Highly descriptive models like Claude 3.5 Sonnet or Gemini 1.5 Pro are masterful at painting textured scenes and using original, evocative metaphors.
