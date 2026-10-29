# One simple idea

Core idea: a task app's first version includes only adding and completing tasks.

- Image: [01-single-idea.png](01-single-idea.png).
- Placement: first use case in both READMEs.
- Alt text: A paper list with Add task and Complete task inside a violet scope boundary.
- Exact visible text: `Add task`, `Complete task`.
- Requested canvas: landscape 16:9, opaque white background.
- Actual output: PNG, 1672 × 941 pixels, approximately 16:9.
- Generation route: native GPT image-generation tool, copied into this project.
- Palette source: [DESIGN.md](DESIGN.md), white `#FFFFFF`, near-black `#171717`, violet `#7C3AED` for selected scope.
- Calibration references inspected: `assets/examples/08-scope-map.png` and `assets/examples/16-list-sequence-02-add-actions.png`. Used for containment, sparse linework, and list grammar only; not attached to generation.

## Generation prompt

```text
Create one original explanatory raster illustration for the simplest README example.
Core idea: a first version of a task app has exactly two actions.
Composition: landscape 16:9, one modest hand-drawn paper sheet centered with generous
white margins. On the sheet, two vertically stacked empty square checkboxes with
handwritten labels "Add task" and "Complete task". One irregular violet outline
encloses both rows, comfortably inside the black paper contour, showing scope.
Style: sparse naturally irregular pen/marker contours, flat unfilled forms,
readable casual handwriting. White #FFFFFF, near-black #171717, violet #7C3AED
only for the scope boundary, from examples/DESIGN.md.
Visible text exactly and only: "Add task", "Complete task".
No people, dialogue, headline, shading, gradients, texture, shadows, decorative
marks, realistic product interface, screenshots, or watermark.
Keep labels large and all marks inside the canvas. Empty checkboxes represent
proposed capabilities, not completed work. Save as a local PNG.
```

## Inspection

Both labels are correct and readable. The two empty checkboxes and violet scope
boundary are contained within the paper. There are no characters or extra text.
Requested hex colors are not verified as pixel-exact.
