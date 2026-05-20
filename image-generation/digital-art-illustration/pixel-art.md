---
title: "Pixel Art Scene"
category: Image Generation
subcategory: Digital Art & Illustration
tags: [pixel-art, retro, game-art, 8-bit, illustration]
model: any (Midjourney, DALL-E 3, Stable Diffusion, Firefly)
---

## Purpose
Generate authentic pixel art scenes, characters, or environments in the style of classic or modern indie pixel art games.

## Prompt
{PIXEL_ART_STYLE} pixel art of {SUBJECT_DESCRIPTION}, {RESOLUTION_FEEL} resolution pixel grid, {COLOR_DEPTH} color palette (limited to {COLOR_COUNT} colors), {DITHERING} dithering technique, {ANIMATION_HINT} energy suggesting motion, {GAME_ERA} game console aesthetic, {LIGHTING_APPROACH} pixel-perfect lighting with {LIGHT_DIRECTION} direction, {BACKGROUND_COMPLEXITY} background, isometric or side-scrolling perspective, meticulous pixel placement, indie game art quality

## Variables
- {PIXEL_ART_STYLE} – Style (e.g., "classic 8-bit NES", "16-bit SNES", "modern high-res indie", "Game Boy green-screen")
- {SUBJECT_DESCRIPTION} – Subject (e.g., "a fantasy village at night", "a space station interior", "a warrior character sprite")
- {RESOLUTION_FEEL} – Scale feel (e.g., "tiny 16x16", "detailed 64x64", "large 256x256")
- {COLOR_DEPTH} – Palette (e.g., "NES 54-color", "Game Boy 4-shade green", "16 color EGA", "32 colors")
- {COLOR_COUNT} – Number of colors to limit to (e.g., "4", "16", "32", "54")
- {DITHERING} – Texture technique (e.g., "checkerboard dithering", "ordered Bayer dithering", "no dithering clean", "stipple")
- {ANIMATION_HINT} – Motion suggestion (e.g., "wind effects in foliage", "flickering torches", "static still frame")
- {GAME_ERA} – Reference era (e.g., "Famicom 1985", "Super Nintendo 1993", "modern Stardew Valley style")
- {LIGHTING_APPROACH} – Light (e.g., "hard pixel-perfect", "faked ambient occlusion", "flat no lighting")
- {LIGHT_DIRECTION} – Light direction (e.g., "top-left", "from a torch", "moonlit")
- {BACKGROUND_COMPLEXITY} – BG detail (e.g., "detailed multi-layer parallax", "simple one-color", "complex city")

## Modifiers
**Midjourney:** --ar 1:1 --v 6.1 --stylize 100 (lower stylize for pixel accuracy)
**DALL-E 3:** Add "pixel art, retro game style" and specify resolution explicitly
**Stable Diffusion:** Use pixel-art specific LoRA models. Negative: (photorealistic, smooth, blurry, 3D render)

## Notes
- For character sprite sheet: add "sprite sheet showing 4 directional frames — front, back, left, right — on transparent background"
- For animated GIF feel: describe "a single frame from a looping animation"
- Lower `--stylize` in Midjourney (e.g., 100) keeps pixel grids crisp and avoids over-smoothing
