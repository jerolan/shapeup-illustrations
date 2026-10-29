# A concept evolves

Core idea: revise a three-feature task app proposal into an initial scope with two actions.

- Image: [02-list-progression.png](02-list-progression.png).
- Placement: second use case in both READMEs, between one simple idea and the conversation.
- Alt text: Three states of the same paper list: add, complete, and reminders; reminders crossed out outside the selected scope; only add and complete remain.
- Requested canvas: one landscape 16:9 bitmap, read left to right.
- Actual output: PNG, 1672 × 941 pixels, approximately 16:9.
- Generation route: native GPT image-generation tool, copied into this project.
- Palette source: [DESIGN.md](DESIGN.md), white `#FFFFFF`, near-black `#171717`, violet `#7C3AED` for scope and revision.
- Continuity image attached: [01-single-idea.png](01-single-idea.png), for the paper, lettering, empty checkboxes, and scope boundary.
- Calibration references inspected: `assets/examples/08-scope-map.png` and `assets/examples/16-list-sequence-02-add-actions.png`.

## States and continuity

| State | Exact visible labels | Visible change | Meaning |
| --- | --- | --- | --- |
| Left | Add task; Complete task; Reminders | Establish three empty checkbox rows. | Initial proposal. |
| Middle | Add task; Complete task; Reminders | Enclose the top two rows in violet; cross out Reminders outside that boundary. | Exclude reminders from the initial scope. |
| Right | Add task; Complete task | Remove the canceled third row, retaining the upper rows and boundary. | The resulting two-action scope. |

Keep the paper silhouette, scale, orientation, upper row positions, and lettering
recognizable. Thin rightward arrows connect successive states. Empty checkboxes
denote proposed capabilities throughout; cancellation does not mean completion.

## Generation prompt

```text
Create one original landscape 16:9 explanatory raster illustration for the second
README example: a task-app proposal revised through three states.
Use 01-single-idea.png only as a continuity/style reference: same simple paper,
readable handwritten labels, irregular near-black pen, violet scope, white background.
Layout: three equal paper sheets horizontally, two thin black rightward arrows
only in the gaps, generous white margins, labels legible at README width.
Keep the paper outline, scale, orientation, first two row positions, label sizes,
and empty checkbox shapes consistent. No people, dialogue, headline, or step numbers.
Left: empty checkboxes labeled "Add task", "Complete task", "Reminders" in order.
No violet boundary yet.
Middle: same three rows. A violet irregular boundary encloses only the top two.
The third row stays below, outside the boundary, with one violet horizontal
cancellation stroke through "Reminders", keeping it readable and its checkbox empty.
Right: same outline, top two rows, and boundary. Remove only the rejected third
row, leaving blank paper below. No checkmarks or completion claims.
Palette from examples/DESIGN.md: #FFFFFF white, #171717 near-black, #7C3AED violet
for revision and selected scope only. Flat hand-drawn marker drawing, no shading,
texture, gradients, shadows, UI chrome, realistic screens, or watermarks.
Visible text only: left and middle "Add task", "Complete task", "Reminders";
right "Add task", "Complete task". Copy exact spelling and case. No captions.
Preserve unchanged marks across snapshots. Save PNG locally.
```

## Inspection

All eight labels are correct and readable. The middle cancellation stays outside
the boundary, and its checkbox remains empty. The final state removes only the
rejected capability. The repeated paper and upper rows remain recognizable;
arrows establish reading order. Requested hex colors are not verified as pixel-exact.
