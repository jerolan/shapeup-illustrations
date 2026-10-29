# Drawing and semantic emphasis

## Line, space and people

Use confident economical pen contours with rounded ends, modest variations in
weight, slightly uneven corners and occasional small overshoots. Keep forms flat
and unfilled on the resolved background. Natural irregularity comes from drawing
with intent; avoid mechanically repeated geometry and artificial jitter.

Use medium pen lines for people and conceptual volumes. Use a heavier felt-tip
marker for rough lists and structural sketches. Keep lettering compact, informal
and readable, with modest baseline and spacing variations. Match lettering weight
to the drawing. Leave purposeful whitespace and frame the actual content closely
enough to read at article size.

People have blank oval heads, outlined torsos, thin limbs and small hands. Posture,
leaning, pointing and gesture carry reaction. Make props schematic and necessary:
a shared board can carry a proposal; an extra page border may add nothing to a list.
Use a few depth edges when needed to explain support or containment, without
rendered lighting, shading, gradients or decorative textures.

The visual references are drawn artwork. Outputs are original drawings, excluding
screenshots, screenshot overlays, realistic product screens, photorealism, polished
stock-vector people, branding and watermarks. A rough drawn interface concept can
be appropriate when it explains the idea.

## Give color a job

Black or the resolved ink carries the structure. Accent is optional, not a quota.
Before using it, identify what deserves emphasis: a questioned feature, an edit,
a selected scope, a critical dependency or an entity whose identity must be tracked.
Keep ordinary structure, people, bubbles and incidental props in ink unless color
has a reason there. Fully monochrome output is valid.

In a sequence, keep the accent's semantic role stable. If it means “current change,”
a previous change can return to ink in the next state while remaining visible.
If it identifies an entity or selected scope, preserve that identity across states.
Completion and cancellation need distinct marks; a colored checkbox alone is
ambiguous. Multiple colors are appropriate when distinct identities need tracking.

## Resolve project colors independently

For background, ink and accent separately, use: **explicit request → applicable
project DESIGN.md → defaults**. An accent override changes only the accent.
Defaults are white background and near-black ink with a restrained accent only
when it serves the explanation; violet is not a global default.

Read an explicitly requested DESIGN.md. Otherwise inspect the destination project
root and directories along the output path. The nearest scoped document wins
conflicts. Resolve linked palette files only as needed. Use the destination
project's guidance, not this installed skill's sample palette.

Apply relevant colors and background while preserving the drawing language. On
dark backgrounds use contrasting ink. If a requested accent has poor contrast,
use a contrasting outline or placement. Report an unreadable requested document
instead of inventing values. Carry resolved colors and roles into the prompt and
image record; GPT may approximate hex colors, so do not promise exact matching.
