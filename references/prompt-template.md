# GPT image prompt

Fill only the fields relevant to the request. Send the generation instructions in English and preserve visible text in the user's language.

```text
Create one original explanatory raster illustration.
Purpose: {intended use and audience}
Core idea: {one sentence faithful to the source}
Representation: {human vignette, conceptual diagram, marker sketch, or short sequence}
Composition: {specific placement, action, relationships, and generous whitespace}
Progression, when relevant: {ordered states, the visible change at each transition,
the stable shared frame and entity identities, and reading order; omit for isolated images}
Guided explanation, when relevant: {what each step establishes, adds, questions,
or revises; exact short accompanying message and its placement; preserve the message
when the conclusion remains unchanged}
Drawing: black hand-drawn pen contours on white, naturally irregular strokes,
unfilled simple forms, sparse details, readable handwritten lettering.
People, if needed: blank oval heads, outlined torsos, thin limbs, small oval hands;
communicate emotion through posture and gesture.
Color: {functional accent and precisely what it identifies}
Visible text: {exact quoted strings and their placement, or "none"}
Canvas: {requested aspect ratio and background}
Reference images: {each attached reference and its role, if any}
Boundaries: drawn artwork only; exclude screenshots, browser chrome, realistic
product interfaces, screenshot overlays, branding, watermarks, and decorative titles.
Use references for linework, simplicity, and spacing; invent an original scene.
Preserve all stated relationships. Copy visible strings verbatim, including accents.
Add no extra text or numerical claims.
```

When using a local reference with a tool that accepts only recent conversation images, forward the viewed reference into the conversation and select the smallest recent-image window that includes the intended references. Do not accidentally include unrelated screenshots from conversation history.

## Targeted repair

Describe the observed defect and the specific correction. Restate the invariant idea, exact text, palette, character proportions, and composition that should remain. Supply the generated image as the edit target; distinguish it from any style-only reference.

For a sequence, identify the affected state and compare it with its neighbors. Preserve the shared frame, entity mapping, and correct states while fixing the transition. A moved dot, new boundary, or added checkmark must correspond to the planned change.

For evolving lists and diagrams, specify the edit operations explicitly: which exact entry is added, crossed out, renamed, moved, checked, or reconnected, and which content stays. Keep the accompanying message consistent with what the edited diagram actually demonstrates.
