---
name: generate-logo
description: Create or refine logos from user inputs such as brand name, style, color theme, business type, and intended use. Use for logo concepts, wordmarks, monograms, symbols, and logo-generation prompts; not for a full brand identity package unless requested.
---

# Generate Logo

Turn a user's brief into a usable logo or, when requested, a ready-to-use image-generation prompt. Preserve explicit choices; do not turn a simple request into a branding questionnaire.

## Interpret the brief

Accept ordinary prose or structured inputs:

| Input | Treatment |
| --- | --- |
| Brand name | Preserve spelling, capitalization, punctuation, and script exactly. |
| Tagline | Include only if supplied and requested; never invent one. |
| Business and audience | Guide symbols, typography, and tone. |
| Style | Minimal, geometric, elegant, playful, vintage, hand-drawn, or user-specified. |
| Color theme | Preserve given colors and hex values as design targets. |
| Logo type | Wordmark, lettermark, monogram, symbol, combination, emblem, or mascot. |
| Symbols | Respect required motifs and avoid lists. |
| Typography | Follow serif, sans-serif, handwritten, or other preferences. |
| Use and layout | Website, profile icon, packaging, sign; horizontal, stacked, or square. |
| Background and format | Transparent or solid; raster or actual editable vector. |
| References | Distinguish a style reference from an existing logo to edit. |
| Quantity | Produce the requested number of concepts or variants. |

Ask only for missing information that prevents success: for example, the exact name when lettering is essential, or the missing source for a requested edit. Icon-only requests do not require a name. Do not repeat answered questions.

For optional omissions, proceed with a brief statement of assumptions. Default to one concept, simple composition, legible lettering where requested, and a restrained palette suited to the brief. If no color direction exists, monochrome is a reasonable starting point. Do not add unrelated motifs or extra deliverables.

## Choose the deliverable

- **Generate a logo:** Use the host’s built-in image-generation tool for raster logos, following its available tool instructions. No external image service or API key is required. Make the image, not just a description.
- **Edit an existing logo:** Inspect the source first. State what changes and what stays fixed. Use the image-editing tool for raster edits, preserving transparency unless instructed otherwise. Edit an existing SVG in its native vector format.
- **Editable vector:** Create real SVG geometry and text when the design can be represented faithfully. Never wrap a PNG in SVG and call it vector. Explain any need for vector reconstruction if a complex concept cannot be delivered faithfully. Do not claim text is outlined when it remains live text.
- **Prompts only:** Deliver prompts without image generation. Read [references/example-prompts.md](references/example-prompts.md) when the user wants examples or a fill-in template.

If the image tool is unavailable or fails, report that clearly and provide the usable prompt; do not claim an image was generated. Do not silently switch to an API or paid external service.

## Build the generation prompt

Use relevant fields from this scaffold and replace placeholders before generation:

```text
Use case: logo-brand
Primary request: Create a logo for [business and audience].
Exact brand text: "[name]"
Exact tagline: "[only when requested]"
Logo type: [type]
Style: [style and personality]
Symbol: [required motif or brief-appropriate direction]
Typography: [preferences]
Color palette: [colors and supplied hex values]
Composition: [layout, use, and clear spacing]
Background: [actual transparency or requested solid color]
Constraints: [must preserve and must avoid]
```

For conventional flat logos, request clean contours, deliberate negative space, balanced spacing, and recognition at small sizes. Avoid incidental mockups, paper textures, presentation labels, and watermarks unless requested. User-requested gradients, dimensional effects, or illustration take precedence over a flat treatment.

Quote requested lettering verbatim. Never translate or transliterate without instruction. For icon-only marks, specify no lettering. For transparency, use the tool's transparency setting, not a checkerboard drawn behind the logo. Hex values in generated bitmaps are targets, not guarantees of exact pixels.

For multiple concepts, vary meaningful design decisions such as symbol construction, type treatment, or layout while preserving shared requirements. Generate separate images for separately requested assets; a concept board does not substitute for usable individual files.

## Check and deliver

Inspect the output for exact text, palette, style, recognizable shapes, spacing, and unwanted elements. Check transparency and file properties when accessible. Evaluate small-size legibility when relevant. Do not present checks you could not perform as verified.

Correct clear mismatches with targeted revisions, preserving successful features. Avoid an open-ended regeneration loop; after two repair attempts, explain remaining limitations and show the best available result.

Show the logo inline when possible and link saved deliverables. Use the user's destination or the host's supported attachment/output storage; provide downloadable artifacts when supported. Save revisions as new versions unless replacement was requested. Report the actual format, brief design rationale, and final generation prompt. Do not describe bitmaps as scalable vectors, promise trademark uniqueness, or label unverified concepts print-ready.

On follow-up, retain the latest accepted brief and change only requested attributes. Generate additional lockups, monochrome versions, or mockups only when requested.
