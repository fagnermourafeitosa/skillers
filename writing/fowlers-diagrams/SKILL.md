---
name: fowler-diagrams
description: Create clear, minimalist, editorial technical diagrams using the local reference.png visual catalogue as the primary style reference. Apply its colors, typography, organic shapes, abstract icons, arrows, annotations, and whitespace while preserving the accuracy of the subject being explained.
---

# Fowler Diagrams

Create explanatory diagrams, architecture sketches, process illustrations, and technical article figures in the visual language documented in `reference.png`.

**This is a visual style skill, not an architecture template.** The reference controls how a diagram looks, not which systems, actors, labels, or relationships must appear.

## 1. Reference comes first

1. Locate and inspect `reference.png` alongside this `SKILL.md`, before designing anything.
2. Treat it as the **primary visual source of truth**. It is a PNG image containing the visual style catalogue. Open and inspect the image itself; do not treat it as a Markdown document.
3. Extract the visual grammar from the reference: typography, colors, spacing, icon geometry, shape vocabulary, annotation treatment, connector styles, and examples of composition.
4. Reinterpret that grammar for the requested subject. **Do not copy the catalogue's panel layout into the final diagram** unless the user specifically asks for a catalogue.
5. If the reference file cannot be opened, do not pretend to have inspected it. Use the specifications below as a fallback and disclose the missing reference when relevant.

## 2. Visual identity

The target is a **simple technical explanation drawn by a person**, not a marketing infographic, dashboard, presentation slide, UI mockup, cartoon scene, or polished corporate flowchart.

- Background: white or near-white, with abundant empty space.
- Structure: free-form, deliberately composed, lightly asymmetrical, and easy to scan.
- Shapes: flat, soft, organic, subtly irregular rectangles, pills, blobs, circles, and simple cylinders.
- Edges: restrained; favor color and spatial grouping over thick outlined cards.
- Texture: mostly solid fills; slight hand-drawn irregularity is welcome, but not noisy textures.
- Line work: thin dark brown, charcoal, or black strokes, with occasional colored arrows.
- Emphasis: one or two focal elements, not an equal-weight box for every label.
- Visual density: low. Remove decorative and repeated components before shrinking typography.

### Color palette

Use colors from the reference. The following hex values are **starting points**, not rigid requirements; choose a subset for each diagram.

| Role | Color | Hex |
| --- | --- | --- |
| Pink | Main process / highlighted element | `#F781C6` |
| Purple | Service / secondary component | `#C8B3E6` |
| Cyan | User / actor / entry point | `#8DD3C7` |
| Green | Resource / successful path | `#B2DF8A` |
| Peach | Process / code background | `#FDBF9E` |
| Pale yellow | Note / explanation | `#FFF2AE` |
| Light blue | Container / document / system | `#A6CEE3` |
| Brown | Database cylinder / arrows | `#B15928` |
| Neutral gray | Secondary / inactive / external | `#CCCCCC` |

Prefer soft, flat color areas with dark legible text. White is an intentional part of the palette.

**Avoid:** gradients, glassmorphism, neon colors, loud saturated backgrounds, 3D rendering, heavy drop shadows, glossy badges, and decorative borders.

## 3. Typography

- All diagram text should be **in English by default**, including headings, notes, legends, captions, and decision labels. Use a different language only when the user requests it.
- Use a readable, straightforward sans-serif typeface for labels and titles (e.g. Arial, Helvetica, or Source Sans 3).
- Use regular and bold weights sparingly; use *italic sans-serif* for secondary notes and explanations.
- Use a clean monospace face for code and JSON (e.g. Source Code Pro, IBM Plex Mono, or a system monospace).
- Titles, when requested, are concise and editorial rather than oversized marketing headlines.
- Text must remain readable at the final output size; keep labels outside shapes when space is tight.
- Prefer short, concrete annotations rather than long paragraphs.

**Avoid:** childish handwriting fonts, Comic Sans, display fonts, dense typography, all-caps marketing slogans, and excessive bolding.

## 4. Shape and icon vocabulary

Reuse the simple symbolic language in `reference.png`:

- **People, developers, agents, teams:** abstract two-part person glyphs, usually a circular head and a simplified curved body; distinguish roles through label or color, not facial expressions.
- **Services/components:** small, soft-edged colored blocks or organic lozenges.
- **Resources:** a smooth, pinched or bow-tie-like green blob when appropriate.
- **Databases:** simple brown cylinder with minimal strokes.
- **Documents:** stacked pastel sheets or a small rounded file shape.
- **External systems:** overlapping gray circles/blobs or a restrained neutral symbol.
- **Security/authentication:** a simple lock, no visual complexity.
- **Decision result:** small green check or red cross only when needed.
- **Containers/boundaries:** faintly filled areas or lightly dashed outlines, not oversized framed boxes.

Icons must remain abstract, flat, and recognizable. Do not invent mascots, expressive robots, human illustrations, faces, or detailed characters.

## 5. Arrows, connections, and visual grammar

Use connection style to convey meaning, consistently within each figure:

| Connection | Suggested treatment |
| --- | --- |
| Primary flow | Solid thin arrow |
| Request / call | Dashed arrow |
| Association / relationship | Curved or dotted connector |
| Event / asynchronous interaction | Dotted line, optionally with an open endpoint |
| Bidirectional exchange | Two opposed arrows or a double-headed arrow |
| Dependency | Curved dashed arrow |
| Alternate / conditional path | Branching arrows with short labels |

- Keep arrows away from text and icon interiors.
- Favor simple bends and gently curved paths over rigid orthogonal routing everywhere.
- Make direction and sequence unambiguous.
- Label connections only when their meaning is not obvious from nearby components.
- Do not use animation cues, thick neon arrows, or decorative arrowheads.

## 6. Notes, code, and supporting material

- **Annotations:** small italic explanations near the relevant element, sometimes on a pale yellow organic highlight.
- **Callouts:** a short label with a curved or dashed pointer; avoid speech balloons unless requested.
- **Code:** small, pale peach or cream region containing accurate, minimal monospace snippets.
- **JSON:** show only the fields needed for the idea; preserve exact syntax when code is meant to be valid.
- **Boundaries:** a faint pastel region or dashed outline to indicate responsibility or context.
- **Legends:** include only if symbols or colors cannot be understood directly from labels.

Do not let snippets, diagrams-within-diagrams, or explanatory paragraphs take over the illustration. For a cover image, favor symbols and relationships over code or detailed architecture.

## 7. Composition patterns

Choose the composition from the concept, rather than forcing one standard flowchart.

- **Process:** a small number of elements linked left-to-right or top-to-bottom.
- **Before/after:** two loose regions connected by a prominent directional change.
- **Comparison:** two balanced areas, each showing the key difference in the objects or flows themselves.
- **Architecture:** small labeled components, meaningful arrows, and boundaries only where technically needed.
- **Decision:** one request or event diverging into clearly labeled outcomes.
- **Conceptual explanation:** a few symbols, directional relationships, and one concise note.
- **Visual catalogue:** separate examples of colors, type, icons, boxes, arrows, notes, and combinations; only when explicitly requested.

Whitespace is preferable to filler, repeated labels, duplicated infrastructure, or decorative cards. Slight asymmetry is desirable when it improves reading order.

## 8. Technical fidelity

Style must never compromise the correctness of the explanation.

1. Identify the subject, key entities, and actual relationships before drawing.
2. Distinguish **actors**, **systems**, **protocols**, **policy decisions**, and **data sources**; do not treat them as interchangeable just because a tidy diagram would be easier.
3. Show direction of data flow accurately. Do not invent service calls or dependencies.
4. Use exact spelling, capitalization, and syntax for standards, protocol names, identifiers, JSON keys, method names, and interface labels.
5. Do not imply that an authorization decision executes a workload if execution occurs elsewhere.
6. Keep trust and data provenance explicit when they are essential to the concept.
7. In comparisons, make the difference visible in the corresponding structures, not only in prose below the figure.
8. If source details are incomplete, simplify the diagram instead of hallucinating specifics.

The diagram should make sense to an informed reader even without a long explanatory caption.

## 9. Production workflow

### Step A — Understand

Write a private one-sentence statement of the concept the diagram must convey. Identify the entities, directional relationships, required text, and optional details. Confirm whether the request is for a cover, article figure, comparison, architecture, or catalogue.

### Step B — Inspect the style reference

Open `reference.png` as an image and inspect the visual catalogue directly. Determine the smallest useful palette, icon types, typography hierarchy, connection styles, and spacing for this particular figure.

### Step C — Sketch the visual story

Lay out a small number of elements with a clear reading order. First establish the visual relationships, then add only the labels required to explain them. Avoid adding a title or subtitle unless explicitly requested; especially avoid repeating article titles already rendered above an image on a page.

### Step D — Render

Prefer an **editable SVG** for diagrams with important text or technical syntax, and export a high-resolution PNG when needed. If using raster image generation, inspect all text and structural relationships carefully. Keep both versions visually consistent when delivering multiple formats.

### Step E — Quality check

Review the output against `reference.png` and the checklist below. Fix the actual image, not just the description of the intended image.

## 10. Acceptance checklist

A finished Fowler-style diagram should satisfy all of the following:

- [ ] The actual `reference.png` was consulted, or its absence was acknowledged.
- [ ] The figure uses the reference's editorial, minimal, flat visual language.
- [ ] Labels are in English unless another language was requested.
- [ ] Typography is straightforward sans-serif, with italics for small notes and monospace for code.
- [ ] Icons are abstract; no cartoon characters or smiling robots.
- [ ] Palette uses a restrained selection of the reference pastels.
- [ ] Shapes feel organic and uncluttered, not like a dashboard component library.
- [ ] Arrows accurately communicate relationship type and direction.
- [ ] Empty space and reading order are intentional.
- [ ] Technical terms, code, and data provenance are accurate.
- [ ] No unnecessary title, subtitle, marketing copy, extra systems, or unrelated details were added.
- [ ] The figure remains legible at its intended display size.

## 11. Default instruction for image creation

When generating a figure, use this design directive as a base and adapt it to the actual topic:

> Create an editorial technical diagram following the visual grammar in `reference.png`: white background, generous whitespace, a restrained pastel palette, flat organic blobs and rounded shapes, simple abstract user and data icons, thin solid/dashed/curved arrows, clear sans-serif labels, small italic annotations, and minimal accurate monospace snippets only when essential. Use English labels. Show the specific requested concept faithfully, with no characters, gradients, dashboard UI, marketing decorations, or unrequested title. The diagram should look like a concise explanation drawn for a technical article, not a corporate infographic.

## 12. Delivery

Deliver the requested image or diagram itself, not only a description of it. When exporting files, use explicit filenames and include a viewable PNG or SVG when the environment supports it. Do not make claims about the diagram being accurate without checking its visible labels, arrows, and relationships.
