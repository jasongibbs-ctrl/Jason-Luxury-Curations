---
name: jason-luxury-instructions
summary: "Reusable instructions for editing Jason Luxury Curations site; prefer inline image embedding and minimal CSS changes."
applyTo: "index.html"
---

## Purpose
- Give the agent explicit guidance for this repository to modify `index.html`.
- Prioritize in-HMTL base64 image embedding over external image references.

## When to use
- User request mentions `jason.jpg`, inline image, base64 embed, or hero image edits.
- User request says “no separate file” or “embed picture in HTML.”

## Guideline
1. Replace external `<img src="...">` with `src="data:image/jpeg;base64,{base64text}"`.
2. Keep layout/CSS changes minimal and consistent with existing dark luxury style.
3. Validate as HTML and ensure no external image file dependency.

## Example
- "Embed `jason.jpg` in `index.html` as inline data URI."
- "Update hero text and color while keeping image inline."