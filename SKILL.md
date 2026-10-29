---
name: shapeup-illustrations
description: "Generates original explanatory images with GPT Image in the hand-drawn visual language of Shape Up. Use for article illustrations, conceptual diagrams, evolving ideas, four-panel conversations, team situations, and image edits in this style, including custom accents or project DESIGN.md colors. Excludes screenshots and screenshot-based compositions."
---

# Shape Up Illustrations

Turn one idea into an original, readable raster illustration using GPT image generation. The reference is the drawn artwork in Basecamp's Shape Up: spare black lines, simple people, visual relationships, and selective color. Screenshots, even screenshots with drawing overlays, are outside this skill's visual references and outputs.

## Workflow

1. **Extract the idea.** Identify the point the image should make, the audience, and any exact visible text. Use the user's language for labels and dialogue. Infer reasonable defaults from the supplied article or request; ask only for information that prevents a meaningful result.
2. **Choose the representation.** Read [composition-patterns.md](references/composition-patterns.md). Use a human vignette for a social tension or a diagram for a relationship. When the explanation builds an idea step by step, revises a proposal, develops a list, or describes changing states, read [progression.md](references/progression.md). Carry the same visual artifact through the explanation, make each change visible, and pair it with a brief message explaining its significance when helpful. Characters are optional in diagrams. Express the idea through an action or spatial relationship rather than a caption alone.
3. **Calibrate the drawing.** Read [style-dna.md](references/style-dna.md), including its color and DESIGN.md rules. Resolve the palette in the target project before writing the prompt. Inspect one or two relevant local examples selected from [sources.md](references/sources.md) with the available image viewer. Treat them as style references; invent the scene, wording, and metaphor for this request. Do not reuse the book's dialogue or treat its diagram values as evidence.
4. **Generate.** Build the prompt with [prompt-template.md](references/prompt-template.md) and follow [generation.md](references/generation.md). Use the native GPT image-generation tool when available. A request for an image means generate the bitmap; a request only for planning or prompts ends at that requested artifact. Do not insert an approval step between concept selection and authorized generation.
5. **Inspect and repair.** Check the generated image using [qa-checklist.md](references/qa-checklist.md). Repair a concrete defect through GPT image generation, preserving correct content. Recheck the result before delivery.
6. **Deliver.** Return the image and, when local files are available, its final path. For article sets, include each image's placement and brief alt text outside the bitmap. State material limitations without claiming checks that were not performed.

## Defaults and series

- Generate one landscape 16:9 illustration unless the user requests another count or format; follow the tool's supported dimensions and report the actual result.
- Save reference assets and generated deliverables as PNG by default. Convert other raster formats when needed, preserving dimensions and transparency; honor an explicitly requested output format.
- Use white background, black linework, and at most one or two functional accent colors unless the request or the target project's DESIGN.md specifies otherwise. Resolve each choice as described in [style-dna.md](references/style-dna.md). Preserve requested transparency on edits; use transparent generation for an explicit cutout request.
- Include no headline by default. Use only the short labels or dialogue needed to understand the idea. For prose-to-image requests, derive those words faithfully from the supplied text; for exact-text requests, copy the supplied strings verbatim.
- For narrative progression, choose linked states within one bitmap or successive illustrations at the relevant points in an article. Use [progression.md](references/progression.md) to preserve the visual frame and make each transition legible. A set of independent illustrations needs stylistic consistency but does not automatically need a temporal story.
- For a requested four-panel conversation, use the 2×2 layout and in-panel dialogue rules in [progression.md](references/progression.md). Keep other layouts available for other requests.
- Save generated assets under `assets/<topic-slug>-shapeup/` in the user's project unless they provide a destination. Use descriptive, numbered filenames for sets and versioned siblings for revisions. Keep generation outputs out of this installed skill's resource directory.

## Bundled resources

The package is usable offline for style selection: `assets/examples/` contains only drawn reference artwork, indexed with provenance in [sources.md](references/sources.md). Network access is needed for GPT generation, not for fetching style references on every invocation. Do not load the whole gallery when one example will resolve the drawing choice.
