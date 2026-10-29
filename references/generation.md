# Generate, inspect and deliver

## Compact generation prompt

Write instructions in English and visible text in the requested language. Include
only fields relevant to this composition. Explain the positive drawing target;
keep exclusions limited to concrete risks and the skill's visual boundaries.

```text
Claim: {one assertion the image should make understandable}
Carrier and composition: {object or shared scene; relationship; framing and order}
States, if needed: {for each, exact visible operation and what it demonstrates}
Preserve: {entity identities, scale, geometry, content and correct previous edits}
Drawing: {confident economical pen or marker, unfilled forms, compact readable
handwriting, simple people and gestures when relevant, purposeful whitespace}
Palette: {resolved background and ink; accent only where it serves the stated role}
Visible text: {exact strings, positions and speakers, or none}
References: {each image's role: style, composition guidance, continuity or edit target}
Output: {image count, supported format/aspect, background and destination}
```

Do not attach every reference. Select one or two drawings using sources.md, inspect
them, and attach through the native tool's supported mechanism. Explicitly separate
style references from a generated continuity frame or edit target. References guide
linework and visual grammar; their text, diagram values and claims are not new data.

## Route

Use the runtime's native GPT image-generation tool when callable. Follow its current
schema, supported dimensions and presentation instructions. For edits include the
target and preserve requested transparency. New images have opaque backgrounds
unless transparency is requested.

If the native tool is absent, use an installed authenticated Codex CLI with image
generation available. Check its current help, pass the selected images through its
supported flags, and request its built-in image generator. Do not require a new API
key or silently substitute another provider while an authenticated route exists.
If neither route is available, explain the missing capability and provide the prompt.
Never substitute a hand-built SVG, HTML, Canvas or screenshot for requested GPT artwork.

## Inspect the actual bitmap

- **Meaning:** the supplied claim is visible through an action or relationship.
- **Transformation:** each declared addition, removal or connection is present;
  the consequence corresponds to that edit. Compare before/after locations.
- **Continuity:** unaffected geometry, identities, framing and accent meanings persist.
- **Narrative:** panels develop the shared idea, dialogue belongs to the correct
  speaker, and required text is verbatim, legible and inside the correct panel.
- **Style:** economical hand-drawn marks, simple unfilled forms, purposeful space;
  no screenshots or realistic product interfaces.
- **Color:** resolved palette and background are followed; each accent has a role.
- **Delivery:** actual file type, dimensions, background, image count and destination
  match the request or are reported honestly. No cropped marks or invented text/data.

Repair a concrete defect through GPT generation, attaching the target. State the
observed failure, exact correction and invariants to preserve. Make at most one
targeted repair per draft before reporting remaining limitations for user review;
repeated attempts should not disguise a failed explanation. Reinspect the result.

## Local assets and records

Copy the chosen output into the destination project, keeping the generator's
original. Preserve earlier versions unless replacement was requested. When the
runtime produces only an inline image, deliver it and say no local file was saved.

Alongside the final image, keep one short Markdown record: claim, brief user
request, exact generation prompt actually submitted, references and their roles,
resolved palette, actual output dimensions/format, alt text and observed limitations.
For sequences include the state table. If repaired, retain the correction prompt
and identify which image is final. Avoid repeating the entire skill or calling a
mechanical check aesthetic approval. For sets include reading order or article
placement. Present the image using the runtime's image helper where available.
