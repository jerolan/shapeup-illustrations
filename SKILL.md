---
name: shapeup-illustrations
description: "Generate original explanatory GPT images in the hand-drawn visual language of Shape Up: a single visual idea, an evolving conceptual artifact, or character interactions with dialogue. Use for article illustrations, diagrams, visual metaphors, linked states, and image revisions, including project DESIGN.md colors. Excludes screenshots and screenshot-based compositions."
---

# Shape Up Illustrations

Make one claim understandable through a spare original drawing. Choose a visual
relationship that explains the claim, then use the drawn language of Shape Up:
confident pen or marker strokes, unfilled forms, expressive gestures, and purposeful
whitespace. A polished illustration of objects alone is not an explanation.

## Workflow

1. **Define the claim.** Establish the audience and what they should understand.
   Internally record: claim; visual carrier; meaningful transformation or relationship;
   and the role of any accent. For example, a removed support changes what the
   remaining structure can sustain. A topic such as “a tower” is not yet a claim.
   Infer reasonable details; ask only when missing information prevents a meaningful
   result. Use the user's language for visible text unless exact wording is supplied.
2. **Choose the composition.** Read [composition.md](references/composition.md),
   following only the relevant branch: single idea, conceptual progression, or
   character narrative. Match layout and image count to the request. A series of
   article images can share a style without forming a progression.
3. **Calibrate.** Read [style.md](references/style.md), resolve the destination
   project's palette, then use [sources.md](references/sources.md) to select and
   inspect one or two relevant drawings. Attach them to the generator when supported,
   explicitly identifying them as style references. For continuity or repairs, the
   previous generated image is a separate reference with a different role.
4. **Generate.** Follow [generation.md](references/generation.md) for the compact
   prompt, native GPT route or authenticated Codex fallback, verification and delivery.
   Generate when images are requested; stop at a proposal or prompt when that is the
   requested artifact. Do not insert an approval step into authorized generation.
5. **Inspect the explanation.** Check the bitmap against the claim and planned
   transformation. Each asserted edit must exist visibly, and its consequence must
   correspond to it. Repair a concrete defect while preserving correct content.
6. **Deliver.** Return the image and actual local path when available. For a set,
   include reading order or placement and brief alt text. State verification limits.

## Defaults

- One landscape image, approximately 16:9; adapt to explicit format requests and
  the tool's supported sizes, reporting actual dimensions. Use a compact framing
  that keeps the explanation legible rather than filling space with extra objects.
- PNG, opaque white background, near-black ink. Accent is optional: use it for a
  specific emphasis, decision, revision, dependency or identity distinction.
- No headline by default; use only necessary labels or requested in-panel dialogue.
- Save project deliverables under `assets/<topic-slug>-shapeup/` unless given another
  destination. Preserve prior versions. Keep a short Markdown record with the image.
  Ordinary user outputs belong in the destination project, not this installed skill.

## Resources

`assets/references/` contains original drawn calibration references with provenance
in `references/sources.md`. `examples/` contains three approved generated examples
for optional composition guidance. Neither is a source of factual data for a new
request. Inspect only what the task needs. `development/` holds exploration history
and review runs; it is not routine generation context.
