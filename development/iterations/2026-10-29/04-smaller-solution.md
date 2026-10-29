# Reduce the solution without losing the purpose

Core idea: a small working solution can meet an immediate need while a larger unfinished solution cannot.

- Image: [04-smaller-solution.png](04-smaller-solution.png).
- Placement: alternative conceptual progression trial for user review; not yet added to the README.
- Alt text: A person gets wet in the rain, remains exposed under an oversized unfinished shelter, then stays dry beneath a small violet-outlined umbrella while the shelter remains unfinished.
- Visible text: none.
- Output: PNG, 1672 × 941 pixels, approximately 16:9, opaque white background.
- Route: native GPT image generation.
- Palette: [DESIGN.md](DESIGN.md), white `#FFFFFF`, near-black `#171717`, violet `#7C3AED` emphasizing the working umbrella. Exact hex accuracy is not verified.
- Attached style references: `assets/examples/01-team-tension.png` and `assets/examples/02-shared-discovery.png`, for simple people, gestures, linework and whitespace only.

## States and purpose

| State | Visible change | Relation to the goal |
| --- | --- | --- |
| Exposed | Hunched person in rain | Staying dry is the unresolved need. |
| Ambitious attempt | Large shelter frame with a roof gap directly above the person | Construction exists but does not yet protect the person. |
| Smaller answer | Same frame remains unfinished; person holds an open umbrella | The immediate need is met with a smaller solution. |

## Inspection

The person's identity and scale remain recognizable. The incomplete shelter and
unused boards persist in the final state. Rain continues around the umbrella,
while its protected interior is clear and the person stands relaxed. Violet is
confined to the umbrella and small deflection marks at its canopy. There is no
readable text. All principal objects remain inside the canvas.

## Generation prompt

```text
Create ONE original explanatory hand-drawn raster illustration with three linked scenes read left to right. Landscape approximately 16:9, white background, PNG.

Meaning to communicate: reduce the solution's scope without losing its purpose. A small working protection can meet the immediate need while an ambitious unfinished shelter cannot. The same visible goal governs all scenes: keep one person dry in the rain. This must be a visual argument, not three unrelated illustrations or a generic flowchart.

Style references: attached drawings calibrate simple unfilled people, confident economical pen lines, informal expressive posture and generous whitespace ONLY. Do not copy their composition, wording or scene.

Layout and continuity: three equal scenes separated by ample white gutters, no enclosing panel frames. Repeat the SAME simple oval-headed faceless person at the SAME scale and ground position in each scene. Maintain the SAME sparse rainfall intensity, height and slant, and a short ground stroke. No arrows, captions, labels, numbers, speech bubbles or readable text.

LEFT — the need:
Rain falls directly onto the person. The person hunches with raised shoulders and arms over their head, visibly trying unsuccessfully to stay dry. Use a few small black drops at the shoulders and feet to show exposure. No shelter or umbrella. Black ink only.

MIDDLE — an oversized attempt:
Keep the person in the rain, still hunched and unprotected.
Around them stands the skeletal frame of a disproportionately broad unfinished shelter: two tall posts, a high crossbeam and only ONE short roof segment at the far side, far from above the person's head. Leave a very obvious open roof gap directly over the person, so rain still reaches them. A few unused roof planks lie to one side. Keep construction schematic, only essential lines, no tools, no extra workers. Black ink only. It must be obvious the structure exists but does not yet solve the need.

RIGHT — a smaller useful answer:
Keep the SAME unfinished shelter frame and unused planks, with the SAME missing roof gap, at the SAME positions as the middle scene. Do NOT complete its roof.
The same person now stands upright and relaxed holding ONE small open umbrella directly above their head. Make its canopy wide enough to protect the person's head and shoulders. Rain still falls around and onto the umbrella, but NO rain strokes or drops appear in the protected space between the umbrella and the person.
Draw only the umbrella canopy contour in violet #7C3AED; shaft, hand, person, shelter, unused planks and rain remain black. The canopy must be unfilled white with a violet outline. This sole accent identifies the useful protection, not decoration.

Drawing: spare naturally varied near-black pen contours, unfilled oval heads and simple outlined torsos, thin limbs and small hands. Use posture to express discomfort versus relief. Schematic recognizable props, imperfect joins and rounded pen ends. Confident irregularity, no artificial distress. Plain white background, no gray wash, texture, shading, gradients or shadows. Avoid polished vector icons or realistic anatomy.
Palette from examples/DESIGN.md: white #FFFFFF, near-black #171717; violet #7C3AED ONLY on the functional umbrella canopy in the last scene.
Visible text: NONE.
Keep all people, rain, structures and umbrella inside the canvas. Preserve rain conditions across states: the final person is dry because of the umbrella, not because the rain stopped. Save locally if supported and report the PNG path.
```
