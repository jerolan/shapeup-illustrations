# A small first version

Core idea: a task app can start with adding and completing tasks.

- Image: [01-small-first-version.png](01-small-first-version.png).
- Placement: the first example in each README.
- Alt text: Two people point to a paper checklist with Add task and Complete task inside a blue scope boundary.
- Visible text: `Add task`, `Complete task`.
- Requested canvas: one landscape image, 16:9 if supported.
- Actual output: PNG, 1672 × 941 pixels, approximately 16:9.
- Generation route: Codex CLI using its native `image_gen` tool.
- Palette: explicit blue accent `#2563EB` overrides the violet in [DESIGN.md](DESIGN.md). Ink `#171717` and white background `#FFFFFF` come from that document.
- Style references: `assets/examples/01-team-tension.png` and `assets/examples/16-list-sequence-01-groups.png`, for linework and simplicity only.

Visual inspection confirmed both exact labels, two people pointing to the same checklist, the blue scope boundary, and content inside the canvas. Hex values were requested but are not verified as pixel-exact.

## User prompt

```text
Use $shapeup-illustrations to show a small first version of a task app.
Draw two people pointing to a paper checklist with only "Add task" and
"Complete task". Use a blue accent, #2563EB, for the boundary around that scope.
Respect examples/DESIGN.md for the other colors. Make one landscape image,
with no headline or dialogue. Save it as examples/01-small-first-version.png.
```

## Generation prompt

```text
Use case: an original README illustration about keeping a first version small.
Asset type: one raster drawing, PNG, landscape 16:9 if supported.
Primary request: show two simple people considering the two core actions of a task app.
Input images: 01-team-tension.png and 16-list-sequence-01-groups.png are style
references only. Copy no scene, dialogue, layout, or wording from them.
Composition: two unfilled oval-headed people stand on either side of one large
paper checklist. Both point toward the same paper. On it, two empty checkboxes
have the exact labels below. A loose blue hand-drawn boundary encloses both rows,
making the selected first scope visible. Keep the paper and text large and
leave generous whitespace. No speech bubbles or additional features.
Style: irregular black pen contours, simple outlined torsos, thin limbs,
small oval hands, blank faces, readable handwritten lettering, flat unfilled forms.
Palette: ink and text #171717, background #FFFFFF, explicit accent #2563EB
only for the scope boundary. This overrides DESIGN.md's violet accent only.
Text, verbatim and only on the paper:
"Add task"
"Complete task"
Constraints: drawn artwork only, no screenshot, realistic UI, branding,
headline, watermark, shading, gradients, extra text, or numerical claims.
Copy both strings verbatim, including case. Keep all content inside the canvas.
```
