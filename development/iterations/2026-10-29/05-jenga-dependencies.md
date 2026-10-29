# Simplify with an understanding of dependencies

Core idea: the importance of a piece depends on what it supports, not its size.

- Image: [05-jenga-dependencies.png](05-jenga-dependencies.png).
- Placement: conceptual progression trial awaiting user review; not yet added to the README.
- Alt text: The same block tower intact, with a top block removed while remaining stable, then leaning after a lower right support is removed. Violet marks the current extraction.
- Output: PNG, 1672 × 940 pixels, approximately 16:9, white background.
- Route: native GPT image generation, followed by one targeted generative correction.
- Palette: [DESIGN.md](DESIGN.md), white `#FFFFFF`, near-black `#171717`, violet `#7C3AED` for the current removed piece and its extraction arrow. Hex accuracy is not verified.
- Attached style references: `assets/examples/09-hidden-effort.png` and `assets/examples/07-integrated-slice.png`, for spare conceptual drawing and simple volumes only.
- Visible text: none.

## States and continuity

| State | Visible change | Meaning |
| --- | --- | --- |
| Left | Intact initial tower | Starting structure is supported. |
| Middle | A top block is removed; tower remains upright | Some reductions preserve the structure. |
| Right | The top gap persists; a lower right support is removed and the stack leans | A similar-sized removal affects what depends on that support. |

The previously removed top block becomes black in the last state, while the
newly extracted support is violet. Existing center gaps remain recognizable
throughout. The initial design is a schematic Jenga-inspired construction,
not a representation of game rules or a quantitative stability model.

## Inspection

All three states retain recognizable layers, viewpoint and scale. The middle
tower remains upright; the final tower retains the top gap and has a visibly
missing bottom-right support. The first generated draft left that support
present, so a targeted correction removed it. No labels or extraneous objects
appear. This remains a conceptual drawing rather than measured physics.

## Generation prompt

```text
Create ONE original explanatory raster illustration: three linked states of the SAME Jenga-inspired block tower, read left to right. The central object itself evolves. No people, hands, setting, props, captions, or unrelated scenes.

Core argument: simplifying requires distinguishing optional pieces from critical supports. Removing two pieces of similar size can have very different effects because of what depends on them. Show this using visible support relationships, not text.

Layout:
One wide landscape canvas, approximately 16:9. Three equal visual states with generous white gutters, all towers at the same scale and viewpoint on the same baseline. Use a simple slightly elevated three-quarter view to make block edges and gaps readable. The first two towers share identical silhouettes and alignments except for the specified removed top piece. Keep all objects comfortably within canvas.
Use a schematic stack of elongated rectangular blocks, reminiscent of Jenga. Draw just enough shallow depth lines to recognize blocks, no wood grain, branding, textures, photorealism or shading. The base must have a visibly important support at the right edge carrying an overhanging part of the upper stack: removing it visibly removes the load path on that side. Make this support relationship legible. This is a conceptual block construction, not a diagram of game rules.

STATE 1 — intact:
A stable compact block tower with several horizontal layers. Draw every block in near-black outlines, unfilled white. Include one removable loose top-layer side piece, and the right-side lower support block. No violet, no floating pieces, no motion marks. All upper pieces have visible support.

STATE 2 — safe reduction:
Repeat exactly the same tower and viewpoint. Remove ONLY the loose top-layer side piece, leaving a precise recognizable gap at its original location. The upper silhouette changes only at that gap; the remaining tower stays vertical and stable.
Place that removed block on the ground to the right of the tower, clearly separate, with a violet outline and white interior. Draw a small violet directional arrow from the top gap toward this removed piece, away from the tower, to explain extraction. All other tower blocks stay black. Do not add any other gaps.

STATE 3 — critical dependency:
Preserve the same already-missing top piece. Its extracted block remains in the same ground location but now in black: it is historical, not the current emphasis.
Now remove ONLY the right-side lower support block, creating a conspicuous gap at its prior position near the base. Place this newly removed support on the ground farther right, outlined violet with white interior. Add a short violet extraction arrow from that base gap toward this newly removed piece.
The upper stack visibly leans modestly toward the now-unsupported right side, with a small separation between a few formerly aligned blocks. The remaining lower left support stays planted. No explosion, debris cloud or dramatic scattered collapse. Make the dependency consequence apparent with economical lines.

Visual language:
Style references attached are ONLY for sparse explanatory drawing, economical irregular pen contours and simple conceptual volumes. Do not copy their text, diagrams or accent color.
Use confident hand-drawn near-black marker lines with slightly uneven corners, modest variations in width and occasional small overshoots. White unfilled forms, simple straight-ish edges, no vector-perfect repetition or artificial distress. Black structure visually dominates. The image should feel sketched to explain a thought, not rendered as a product.
Palette from examples/DESIGN.md: white #FFFFFF, near-black #171717, violet #7C3AED only for the currently removed block and its extraction arrow in states 2 and 3. Do not color other blocks or tower outlines.
Visible text: NONE. No step numbers, headlines, labels, checkmarks, panel frames, shadows, gradients, decorative marks, logos or watermark. No arrows between states.
Output: one landscape PNG. Save locally if supported and report file path.
```

## Targeted correction prompt

```text
Edit the attached illustration with ONE targeted correction. Keep the entire LEFT and MIDDLE scenes unchanged. Preserve the white background, black hand-drawn linework, three-state layout, tower scale, top missing piece in middle and right, existing violet arrows, and both extracted pieces in the right scene. No text.

Defect: in the RIGHTMOST scene the lowest right-hand supporting block is still visibly present, even though its removed counterpart is drawn violet on the ground. The cause of instability is therefore invisible.

Correction ONLY in RIGHTMOST tower:
Completely remove the bottommost right-side supporting block, INCLUDING its front face, top face, side face and any concealed continuation. It is the block at the lowest row's right edge, directly next to the currently open center gap. The space it occupied must be visibly empty white, continuous with the center gap, so the entire lower-right footprint is now missing. Retain only the bottommost LEFT supporting block. The layer directly above must visibly overhang the empty right-side base space; do not redraw another support, leg, hidden block or plinth beneath it. Make the stack above that void lean slightly to the right while the remaining bottom-left support stays planted. Preserve the upper missing top piece from the middle scene and other recognizable layers.
The violet extraction arrow should begin near this now-empty bottom-right support position and point to the existing violet block on the ground to the right. That violet block is the removed lower support. The previously removed top block remains black beside it.
No explosion, added pieces, colored tower outlines, new effects, captions or decorative marks.
Keep the image as an economical conceptual sketch, not a physics simulation. PNG, white background, same dimensions.
```
