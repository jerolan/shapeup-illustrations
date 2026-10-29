# An idea develops through conversation

Core idea: two teammates question a task app's scope, defer reminders, and try the smaller idea on paper.

- Image: [02-idea-conversation.png](02-idea-conversation.png).
- Placement: the third use case in each README, after the simple idea and list progression.
- Alt text: Four panels show the same two teammates proposing a task app, questioning reminders, narrowing the idea to adding and completing tasks, and trying that paper prototype.
- Requested canvas: one landscape image, 16:9 if supported, with a 2×2 grid.
- Actual output: PNG, 1672 × 941 pixels, approximately 16:9.
- Generation route: Codex CLI using its native `image_gen` tool.
- Palette: [DESIGN.md](DESIGN.md) supplies violet `#7C3AED` for questions and revisions, ink `#171717`, and white background `#FFFFFF`. No explicit accent override.
- Style references: `assets/examples/01-team-tension.png` and `assets/examples/16-list-sequence-01-groups.png`, for linework and simplicity only.

## States and continuity

Read top left, top right, bottom left, then bottom right. Keep teammate A on the left, teammate B on the right, and the same whiteboard between them.

| Panel | Visible development | Exact dialogue | Speaker |
| --- | --- | --- | --- |
| Top left | Establish a checklist and a bell icon as parts of a broad idea. | Let's build a task app. | A |
| Top right | B points to the same bell, now circled in violet as a question. | Do we need reminders now? | B |
| Bottom left | Cross out the bell and put a violet boundary around the checklist. | Start with add and complete. | A |
| Bottom right | Keep the reduced scope and check one box while trying the paper prototype. | Let's try this first. | B |

The final checkmark demonstrates a proposed interaction on paper, not a shipped product or a measured result. The dialogue explains the scope change, so this example needs no extra explanatory caption inside the panels.

Visual inspection confirmed the 2×2 reading order, all four exact dialogue strings, clear speakers, the recurring whiteboard, the circled and crossed-out bell, the narrowed scope, and the final checked box. Content remains inside each panel. Hex values were requested but are not verified as pixel-exact.

## User prompt

```text
Use $shapeup-illustrations to show two teammates developing a task app idea.
Make one image with four panels in a 2x2 grid. Keep the same people and whiteboard.
Show the idea, an objection about reminders, a narrower scope, and a paper trial.
Put this dialogue inside speech bubbles, in reading order:
"Let's build a task app."
"Do we need reminders now?"
"Start with add and complete."
"Let's try this first."
Use examples/DESIGN.md for the palette. Save examples/02-idea-conversation.png.
```

## Generation prompt

```text
Use case: an original README example of an idea developing through conversation.
Asset type: one raster PNG illustration, landscape 16:9 if supported, with four panels.
Primary request: two teammates narrow a task app idea to adding and completing
tasks, defer reminders, and try that smaller proposal as a paper prototype.
Input images: 01-team-tension.png and 16-list-sequence-01-groups.png are style
references only. Invent this scene; copy none of their wording or arrangements.
Composition: a clear 2x2 grid with whitespace gutters and light hand-drawn dividers.
Reading order is top left, top right, bottom left, bottom right. Repeat the same
two unfilled oval-headed people, A on the left and B on the right, with one
whiteboard between them in every panel. Preserve framing and object identity.
Panel 1: A proposes the idea. The board shows a paper checklist with two empty
checkboxes and short abstract row strokes, plus a separate outlined bell icon.
A's speech bubble says exactly "Let's build a task app."
Panel 2: preserve the board. B points at the same bell, now circled in violet.
B's speech bubble says exactly "Do we need reminders now?"
Panel 3: A crosses out the bell with violet strokes and draws a violet boundary
around the same checklist, keeping the checklist and its rows recognizable.
A's speech bubble says exactly "Start with add and complete."
Panel 4: keep the reduced-scope boundary and crossed-out bell. B checks the first
box on the same paper checklist to try the proposed interaction.
B's speech bubble says exactly "Let's try this first."
Style: spare irregular pen contours, simple outlined torsos, thin limbs, small
oval hands, blank faces, readable handwritten lettering, generous whitespace.
Palette from examples/DESIGN.md: ink and text #171717, background #FFFFFF,
accent #7C3AED for the question circle, scope boundary, revision, and checkmark.
Text: only the four exact dialogue strings above, one bubble per panel.
Keep each bubble's tail directed at its named speaker and all text inside its panel.
Constraints: drawn artwork throughout, no screenshot, realistic interface, chat
app chrome, headline, panel numbers, watermark, gradient, shading, or extra words.
Show the changes in the drawing, not only through different dialogue. Copy every
visible string verbatim, including apostrophes, case, and punctuation.
```
