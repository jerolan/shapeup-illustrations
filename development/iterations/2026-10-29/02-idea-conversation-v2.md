# Narrative character trial

Core idea: two teammates question reminders, narrow a task app's scope, and test a paper prototype.

- Image: [02-idea-conversation-v2.png](02-idea-conversation-v2.png).
- Placement: style trial for review; the README still uses the original conversation.
- Alt text: Four panels show two teammates proposing a checklist with reminders, questioning the bell, selecting the checklist and canceling the bell, and testing a separate paper checklist.
- Output: PNG, 1672 × 941 pixels, approximately 16:9; opaque white background.
- Route: native GPT image generation.
- Palette: [DESIGN.md](DESIGN.md), white `#FFFFFF`, near-black `#171717`, violet `#7C3AED`. Hex accuracy is not verified.
- Attached style references: `assets/examples/01-team-tension.png` and `assets/examples/02-shared-discovery.png`. Used only for sparse pen contours, proportions, gestures, and lettering; no source dialogue reused.

## Narrative states

| Panel | Visible development | Exact dialogue | Speaker |
| --- | --- | --- | --- |
| Top left | Checklist and bell proposed in black. | Let's build a task app. | A, left |
| Top right | Violet circle identifies the questioned bell. | Do we need reminders now? | B, right |
| Bottom left | Violet cancellation over the bell; violet scope around the checklist. | Start with add and complete. | A, left |
| Bottom right | Revised board remains visible; B marks a separate paper checklist in black. | Let's try this first. | B, right |

## Inspection

All four dialogue strings are correct and inside their respective panels. The
characters retain their left/right identities and the shared proposal changes
visibly. Violet is confined to the questioned bell and scope decision; the
paper-trial checkmark is black. In the final panel A moves toward the prototype
and partly overlaps the board, with the selected scope and canceled bell still
recognizable. No README or skill instruction changes accompany this trial.

## Generation prompt

```text
Create one original narrative illustration with four panels in a 2×2 grid. Read top left, top right, bottom left, bottom right. Landscape approximately 16:9, PNG.

Core idea: two teammates develop a task app proposal, question reminders, reduce the initial scope, and test the smaller idea on paper.

Input images: attached drawings are STYLE REFERENCES ONLY for economical pen lines, simple unfilled people, expressive gestures and informal lettering. Invent the scene below, copying no reference dialogue or composition.

Visual language:
Use the spare hand-drawn language of Shape Up's explanatory illustrations. Draw confident near-black pen and marker strokes with natural variations in thickness, slightly uneven corners, and simple unfilled forms. Use compact, readable handwritten lettering. Keep human contours lighter than bold marker annotations; no polished vector finish or artificial jitter.

Characters:
Keep the same two people in all four panels. Person A stands on the left; person B stands on the right. Use blank oval heads, simple outlined torsos, thin limbs, and small hands. Communicate reactions through posture, leaning, pointing, and hand gestures. Keep their proportions consistent.

Shared scene:
Keep the same whiteboard between the characters, at the same scale and angle. On it, a two-row checklist represents adding and completing tasks. A separate bell icon on the right represents reminders. Use generous whitespace and subtle hand-drawn panel dividers. Make the whiteboard contents and gestures clearly legible.

Panel 1 — Proposal:
A points toward the checklist and bell on the whiteboard. B leans toward the proposal, listening. Everything is drawn in black. A says: "Let's build a task app."

Panel 2 — Question:
Preserve the same checklist and bell. B points at the bell with a questioning gesture. Add a quick violet circle around that bell to identify the disputed feature. A pauses, with one hand near their chin. B says: "Do we need reminders now?"

Panel 3 — Revision:
Preserve the checklist in the same position. Replace the questioning circle with a violet cancellation mark over the bell. Add a loose violet boundary around only the checklist to show the chosen scope. A points to the selected checklist while B looks at the revision. A says: "Start with add and complete."

Panel 4 — Paper trial:
Keep the revised whiteboard visible, including the canceled bell and scope boundary. B holds a separate simple paper version of the checklist and marks its first box in black with a marker. A leans toward the paper to observe the trial. Do not add another colored emphasis mark. B says: "Let's try this first."

Color:
White background #FFFFFF; near-black ink #171717. Use violet #7C3AED only to identify the questioned feature and the scope decision. Retain those annotations in later panels for continuity. Do not color characters, speech bubbles, panel dividers, paper trial checkmark, or incidental props. This palette comes from examples/DESIGN.md. Accent is semantic emphasis, not decoration.

Exact text:
Put each dialogue string exactly as supplied inside its corresponding panel, in a speech bubble clearly connected to its speaker. Keep the text legible at README width. Use abstract short black strokes for checklist entries. Add no headline, captions, extra dialogue, numbers or other readable text. Do not translate.

Constraints:
The drawing must change with the story; dialogue alone must not carry progression. Keep all bubbles and marks inside the canvas and within the corresponding panel. Avoid polished vector people, perfect geometry, artificial distress, shading, gradients, shadows, realistic screens, screenshots, and watermarks. Save locally if supported and report output path.
```
