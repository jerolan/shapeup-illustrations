# One simple idea — marker style trial

Core idea: a task app's first version includes adding and completing tasks.

- Image: [01-single-idea-v2.png](01-single-idea-v2.png).
- Placement: style trial awaiting user review; the README still uses the original.
- Alt text: Two small empty checkboxes and bold handwritten action labels inside an irregular violet scope loop, with no outer paper outline.
- Exact visible text: `Add task`, `Complete task`.
- Actual output: PNG, 1672 × 941 pixels, approximately 16:9, opaque white background.
- Route: native GPT image generation.
- Palette: [DESIGN.md](DESIGN.md), background `#FFFFFF`, ink `#171717`, accent `#7C3AED`. Hex accuracy is not verified.
- Attached style references: `assets/examples/16-list-sequence-02-add-actions.png` for marker weight and list grammar; `assets/examples/08-scope-map.png` for organic containment. Reference content was not reused.
- Inspection: both labels are correct and fully inside the canvas; both checkboxes are empty; no outer paper, people, headline, or extra text. The trial has bolder marker lettering and a more organic boundary than the original. The violet loop remains prominent.

## Generation prompt

```text
Create ONE original explanatory raster illustration, a style trial for the first example in a README.
Core idea: a task app's initial scope contains just two actions.
Input images: image 1 is a marker list sketch; image 2 is an irregular containment diagram. Use both ONLY to calibrate the confident economical marker line, compact lettering and purposeful whitespace. Invent this new composition; copy no wording, scene, or layout from the reference drawings.
Composition: compact two-row list floating directly on a plain white landscape canvas, centered with comfortable margins. One small empty checkbox beside each label. Enclose both rows in a loose violet scope loop, shaped by the content rather than a rounded rectangle. No paper contour, card, frame, people, speech bubbles or headline. Make the whole two-row drawing comfortably readable at README width, occupying about the middle two thirds of canvas width, with a modest gap between rows.
Visual language: an explanatory sketch drawn confidently by hand with a felt-tip marker, in the spare visual language of Shape Up's drawn diagrams. Near-black strokes have modest organic thickness changes, imperfect square corners and occasional slight overshoots at joins. Shapes are schematic and unfilled. Black ink is visually dominant. Checkboxes are small relative to labels, each a few decisive thick marker strokes. Write the labels in compact bold readable informal handwriting, with slightly varying letter spacing and baseline. The writing should feel made with the same marker as the shapes.
Accent: draw a single violet annotation loop around the two rows in one quick asymmetric gesture. Its shape is not geometrically regular and not a polished pill outline. The stroke is confident rather than artificially shaky. Use the violet boundary only to indicate scope.
Palette from examples/DESIGN.md: background #FFFFFF, near-black ink and text #171717, violet #7C3AED for the scope annotation. Flat unfilled drawing with crisp solid ink, clean white background. No texture, distress, shading, shadows, gradient, ornamental lettering, mechanically repeated shapes, oversized checkboxes, perfectly rounded rectangle, uniform vector strokes, realistic product UI, screenshots or watermark.
Exact visible text, and no other text: "Add task", "Complete task", in that order. Preserve case, spelling and both empty checkboxes. Do not translate or add headings. Keep all marks inside the canvas. Landscape roughly 16:9, PNG. Save output locally if supported and report its path.
```
