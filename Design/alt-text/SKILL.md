---
name: alt-text
description: Writes clear, specific alt text for images. Use this whenever you need to describe an image accessibly — for images you're embedding in documents, websites, social media, or any output where a blind or low-vision person will encounter it. Handles everything from portraits to landscapes to diagrams to screenshots. Captures what matters. Composition, gesture, spatial relationships, context. Concise. No padding. Under 1000 words. Skips purely decorative images.
compatibility: "Image input (local file, URL, or pasted screenshot)"
---

## Why This Matters

Alt text isn't a label. It's a window. Don't write like a museum placard or overwrite it. Write clear, direct description. Specific detail without fluff.

Avoid pure inventory ("A woman with brown hair, glasses, red lipstick"). But also avoid flowery prose. The goal is to convey what matters visually—composition, gesture, spatial relationships, context—in the most efficient way possible.

## How It Works

### Input
Provide an image in one of these ways:
- **File path** (local): `/path/to/image.jpg`
- **URL**: `https://example.com/image.png`
- **Pasted screenshot**: Copy and paste directly

### Output
A single block of alt text, typically 50–300 words:
1. **Identifies what's in the image** — image type, main subject, key elements
2. **Captures spatial relationships** — foreground, background, composition
3. **Notes human detail** — if people are present, describe gesture, body language, expression
4. **Includes color and light** — only if they're essential to understanding (not atmosphere-building)
5. **Names what's absent** — if significant (empty space, cropped figures, etc.)
6. **Keeps tone matched to the image** — straightforward for diagrams, warmer for portraits, direct for screenshots

### What Counts as "Decorative"
Skip alt text for:
- Pure decorative elements (ornamental backgrounds, filler graphics, dividers)
- Icon-only buttons with adjacent text labels
- Watermarks or logos in margins

Write alt text for everything else, including icons with *no* text label, interface screenshots, data visualizations, mixed scenes, ambiguous images, and all human-present photos.

### Constraints
- **Under 1000 words** — usually 150–400 words; go longer only if the image demands it
- **No fabrication** — describe what's actually there, including uncertainty ("it's unclear whether…", "you might read this as…")
- **Screen-reader compatible** — clear, scannable structure; avoid run-on sentences; use line breaks for visual hierarchy
- **Accessible language** — concrete, not abstract; define jargon; assume no shared context

## The Voice

Be clear. Be specific. Stop when you've said what matters.

- Name details that matter (silver streaks, red lipstick, gesture) without listing everything
- If color or light is important, mention it. If it's not, skip it
- Describe spatial relationships directly (person on left, object behind, empty space right of frame)
- Name what's missing if it's significant (empty chair, cropped figure, blank wall)
- Match the image's energy: dense and urgent for crowded scenes, spare for landscapes, precise for diagrams

## Examples

**Portrait:**
"Person with long brown hair streaked with silver, wearing glasses and red lipstick against a cream background. Behind them: potted plants, roses, and a stone sculpture of two hands offering an open heart. Direct gaze, calm expression."

**Landscape:**
"A valley at golden hour. Rough grass in foreground. Rolling hills receding into hazy blue mountains. Single dark tree silhouetted on far ridge. Pale sky. No people or structures."

**Diagram:**
"Flowchart with four boxes: Input (top left) → Process (top right) ↔ Decision (bottom left, branches to Output bottom right or loops back). Blue outlined boxes, black text."

**Screenshot (Slack thread):**
"A Slack message from @jessie_dev: 'Shipped the new dashboard today after two weeks of debugging. Feels surreal.' Three replies with thumbs-up emoji. One comment: 'looks beautiful, great work.' Total 8 replies."

## Questions to Guide Your Analysis

When you sit down to write, ask:

- **What type of image is this?** (Determines tone and priority.)
- **What's the main subject?** What matters most?
- **If people are present, what are they doing?** Gesture, body language, expression.
- **How is it composed?** Foreground, background, edges. What's in frame and what's cropped?
- **Is light or color essential?** Only mention if it changes the meaning.
- **What's notably absent?** Empty space, missing figures, blank areas—mention if significant.
- **Keep it specific and brief.** Stop when you've said what matters.

---

## When NOT to Write Alt Text

- **Decorative-only**: A generic geometric pattern, a spacer, an ornamental flourish with no informational purpose
- **Redundant text**: An image that *only* contains text that's already in the document (unless the visual rendering—font, color, size—is essential to understanding)
- **Icon with text**: A button that shows an icon + adjacent text label (the text is the alt; the icon is redundant)

## When to Write Alt Text

- **Everything else**: Portraits, landscapes, screenshots, diagrams, mixed scenes, data visualizations, graphs, ambiguous images, icons standing alone, memes, social-media posts, evidence exhibits, anything that communicates through visual form
- **Uncertainty is OK**: "It's hard to tell whether…" and "You might read this as…" are honest and helpful

---

## How to Use This Skill

1. **Invoke the skill** when you have an image you need to describe accessibly
2. **Provide the image** (file path, URL, or paste)
3. **Optionally provide context** (where will this alt text live? who's the audience? any specific details you want emphasized?)
4. **The skill will analyze and write** a single, cohesive alt text block under 1000 words
5. **Copy the alt text** into your `alt=""` attribute, document metadata, image description field, or platform's accessibility field

---

## Accessibility Notes for Implementation

When you place this alt text:
- **HTML**: `<img src="path.jpg" alt="[full alt text]">`
- **Markdown**: `![alt text](image.jpg)` — paste the full alt text between the brackets
- **Word/Google Docs**: Right-click image → "Alt text" → paste the full block
- **Social media**: Use the platform's "Image description" or "Alt text" field (Twitter, Instagram, LinkedIn all have them)
- **PDF**: Add as image description in document properties
- **Obsidian/Notion**: Paste into alt text field or note caption

The alt text becomes what a screen reader announces. Make it count.

---

## A Note on Length

Aim for 50–300 words. That's the sweet spot.

Go longer only if the image is genuinely complex (a detailed diagram, crowded scene with many elements, an evidence exhibit). Go shorter if the image is simple.

Never pad. Never flowery for the sake of it. Under 1000 words absolute max; you should rarely hit that.
