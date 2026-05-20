---
title: "3D Render & CGI Style Art"
category: Image Generation
subcategory: Digital Art & Illustration
tags: [3D, CGI, render, blender, octane, illustration]
model: any (Midjourney, DALL-E 3, Stable Diffusion, Firefly)
---

## Purpose
Generate images that look like high-end 3D renders from tools like Blender, Cinema 4D, or Octane Renderer.

## Prompt
Photorealistic {RENDER_SOFTWARE} 3D render of {SUBJECT_DESCRIPTION}, {SURFACE_MATERIAL} surface materials with physically based rendering, {HDRI_LIGHTING} HDRI studio lighting setup with {SECONDARY_LIGHT} secondary light, {DEPTH_OF_FIELD} depth of field with bokeh on {BACKGROUND_ELEMENTS}, subsurface scattering on {SSS_ELEMENTS}, {REFLECTION_QUALITY} reflections and {REFRACTION} refractions, {POST_PROCESSING} post-processing (bloom, chromatic aberration, film grain), ultra-high resolution 4K output, {RENDER_QUALITY} render quality settings, professional 3D visualization

## Variables
- {RENDER_SOFTWARE} – Software aesthetic (e.g., "Blender Cycles", "Cinema 4D Octane", "Unreal Engine 5", "KeyShot")
- {SUBJECT_DESCRIPTION} – What to render (e.g., "a geometric abstract sculpture of interlocking metal rings", "a minimalist product on a reflective surface", "a tiny cozy cabin on a floating island")
- {SURFACE_MATERIAL} – Materials (e.g., "brushed anodized aluminum", "rough concrete and polished gold", "translucent glass and chrome")
- {HDRI_LIGHTING} – Primary light (e.g., "studio three-point", "overcast outdoor HDRI", "dramatic single spotlight", "sunset environment")
- {SECONDARY_LIGHT} – Fill light (e.g., "warm rim light", "cool fill panel", "neon accent strips", "no secondary")
- {DEPTH_OF_FIELD} – Focus (e.g., "narrow with soft bokeh", "full sharp", "extreme tilt-shift miniature effect")
- {BACKGROUND_ELEMENTS} – BG (e.g., "bokeh light circles", "gradient studio", "environment reflections", "pure white")
- {SSS_ELEMENTS} – SSS subjects (e.g., "skin, wax, marble", "translucent plastic", "none")
- {REFLECTION_QUALITY} – Reflections (e.g., "mirror-perfect", "rough diffuse", "hybrid semi-glossy")
- {REFRACTION} – Transparency (e.g., "glass lens distortion", "water caustics", "none")
- {POST_PROCESSING} – Effects (e.g., "subtle bloom and grain", "heavy cinematic", "clean minimal")
- {RENDER_QUALITY} – Quality (e.g., "final production", "preview draft with denoising", "photo mode")

## Modifiers
**Midjourney:** --ar 1:1 --v 6.1 --stylize 400
**DALL-E 3:** Add "photorealistic 3D render, CGI quality" at start
**Stable Diffusion:** Negative: (2D, flat, hand-drawn, painted, low poly unless specified)

## Notes
- For Blender diorama style: add "tiny diorama world, tilt-shift focus, miniature photography aesthetic, pastel colors"
- For product viz: add "product visualization, brand presentation, clean studio, luxury feel"
- Specifying the render engine name (e.g., "Octane render") strongly influences the model's material quality output
