# An abstract idea develops

Core idea: having all the pieces is different from having a connected system.

- Image: [03-abstract-progression.png](03-abstract-progression.png).
- Placement: abstract progression trial for user review; not yet added to the README.
- Alt text: Three repeated stacks labeled Entrada, Proceso, and Resultado: isolated blocks, a partial black connection, then a complete route with the final connection highlighted in violet.
- Output: PNG, 1672 × 941 pixels, approximately 16:9, opaque white background.
- Route: native GPT image generation.
- Palette: [DESIGN.md](DESIGN.md), white `#FFFFFF`, near-black `#171717`, violet `#7C3AED` only for the decisive connection. Exact pixel colors are not verified.
- Attached style references: `assets/examples/05-interaction-flow.png` and `assets/examples/07-integrated-slice.png`, for sparse linework, meaningful connections, and functional accent; no source content reused.

## States

| Position | Preserved structure | Change | Implication |
| --- | --- | --- | --- |
| Left | Entrada, Proceso, Resultado, stacked vertically | No connections | Components remain isolated. |
| Middle | Same blocks, labels, and positions | Black arrow from Entrada to Proceso | The route remains incomplete. |
| Right | Same blocks and existing black arrow | Violet arrow from Proceso to Resultado | The final connection completes the route. |

## Inspection

The nine labels match the requested Spanish strings. There are no arrows in the
left state, one black arrow in the middle, and a black plus violet arrow in the
right. Repeated structures and row positions remain recognizable. Violet is
confined to the last connection. Labels and marks remain inside the canvas.

## Generation prompt

```text
Create ONE original explanatory raster illustration showing an abstract idea developing through three successive states. One wide landscape PNG, approximately 16:9, white background.

Core idea: Having all the pieces is different from having a connected system.

Input images: two attached drawings are STYLE REFERENCES ONLY for economical hand-drawn lines, compact lettering, meaningful connections and restrained semantic accent. Invent the specified composition. Do not reuse their diagrams, text, colors, or claims.

Composition:
Three equally spaced visual states arranged horizontally, read left to right. In EACH state, repeat exactly the same three small unfilled schematic blocks in a vertical stack. Each block contains one exact Spanish label, top to bottom:
"Entrada"
"Proceso"
"Resultado"
Keep the blocks, labels, positions within each state, scale, orientation, and vertical spacing consistent. Leave enough room between blocks for short, clear downward arrows. Separate the three states with generous whitespace only. No outer frame, no panel borders, and no arrows between states: those could be confused with system connections.

LEFT STATE:
Draw three near-black blocks and labels with NO connecting arrows. The components exist but remain isolated. No violet anywhere in this state.

MIDDLE STATE:
Preserve the identical three blocks. Add exactly ONE near-black downward arrow from the bottom edge of Entrada to the top edge of Proceso. Resultado remains disconnected; the space between Proceso and Resultado is blank. No violet anywhere in this state.

RIGHT STATE:
Preserve the identical three blocks and the existing black Entrada-to-Proceso arrow. Add exactly ONE violet downward arrow from the bottom edge of Proceso to the top edge of Resultado. This new connection completes the route. Only this decisive connection receives violet. All boxes, labels, and the first connection stay black.

Drawing:
Confident economical hand-drawn felt-tip pen and marker strokes, slightly uneven corners, naturally varied stroke weight, unfilled shapes, compact readable informal handwriting. Modest overshoots at joins are acceptable; no artificial jitter or distress. Keep black ink visually dominant. Fit the drawing to the canvas with comfortable whitespace and readable labels at article width. Boxes are schematic hand-drawn enclosures, not polished UI cards.

Palette from examples/DESIGN.md:
White background #FFFFFF, near-black structure and text #171717. Violet #7C3AED only for the final connection from Proceso to Resultado in the rightmost state. No other colored element.

Exact visible text only: "Entrada", "Proceso", "Resultado", each repeated once per state, for nine labels total. Preserve case, spelling and language verbatim. Do not add words, numbers, captions, headlines, icons, checkmarks, people, paper sheets, decorative marks, shadows, gradients, screenshots, watermarks or vector-perfect geometry.
The visual change must explain the progression without relying on captions. Keep all marks within the canvas. Save PNG locally if supported and report its path.
```
