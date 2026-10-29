# Shape Up illustrations

[Español](README.es.md)

Create original hand-drawn illustrations for ideas, changing proposals, and team conversations in the visual language of Shape Up. The skill draws scenes and diagrams, not screenshots or screenshot-based compositions.

## Requirements

Use an agent with native GPT image generation, or an installed, authenticated Codex CLI with GPT image generation available. You do not need a new API key for an authenticated route. If neither route is available, the agent can provide a prompt but cannot generate the image.

## Use

Invoke `$shapeup-illustrations` in your agent, or ask for the `shapeup-illustrations` skill by name. Describe the idea, the audience, any exact visible text, and your desired destination. The agent selects a drawing composition, generates the image, and inspects it. By default, local images go in `assets/<topic-slug>-shapeup/` in your project, with a Markdown sidecar.

Use a single scene for one idea or a sequence when the change matters. Four-panel conversations use a 2×2 grid, but other compositions and panel counts are available. Dialogue belongs inside its panel; a brief explanatory note can also appear there when needed.

## Examples

These examples are original generated illustrations, not copies of the book. The English strings below are the requested visible text. Generation may vary between runs, and identical bitmaps are not guaranteed.

Run these prompts from this repository's root. In another project, replace the output paths and use that project's `DESIGN.md`.

### A small first version

![Two people point to a paper checklist inside a blue scope boundary.](examples/01-small-first-version.png)

The boundary selects only two actions for the first version. The requested blue overrides the sample design's violet accent without changing the ink or background.

Ask for:

```text
Use $shapeup-illustrations to show a small first version of a task app.
Draw two people pointing to a paper checklist with only "Add task" and
"Complete task". Use a blue accent, #2563EB, for the boundary around that scope.
Respect examples/DESIGN.md for the other colors. Make one landscape image,
with no headline or dialogue. Save it as examples/01-small-first-version.png.
```

The [example sidecar](examples/01-small-first-version.md) contains the detailed generation prompt and palette.

### An idea develops through conversation

![Four panels show two teammates questioning and trying a smaller task app idea.](examples/02-idea-conversation.png)

Read left to right, then down:

1. Propose a task app with a checklist and reminders.
2. Question whether reminders belong in the first version.
3. Cross out the bell and select only the checklist.
4. Try the smaller proposal by checking a box on the paper prototype.

The dialogue explains each change inside its panel. The shared whiteboard makes the revision visible, rather than relying on messages alone.

Ask for:

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

The [example sidecar](examples/02-idea-conversation.md) contains the detailed generation prompt and a table of states, dialogue, and continuity.

## Color and project design

For each color choice, an explicit request takes precedence over the applicable `DESIGN.md`, followed by the skill defaults. An accent override changes the accent, not the background. The applicable design document guides palette and background; it does not turn the drawing into a UI mockup.

Without project guidance or an explicit request, the skill uses black on white with restrained functional accents.

[examples/DESIGN.md](examples/DESIGN.md) applies to these examples only. It is not a global theme for projects using the skill. GPT may approximate a requested hex color rather than match it exactly. See [color and design rules](references/style-dna.md#custom-accents-and-designmd) for how the agent selects project guidance.

## References and rights

The Basecamp drawings in `assets/examples/` are calibration references. Their authors retain their rights. See [sources and provenance](references/sources.md). The skill creates new scenes rather than copying reference artwork.

## Maintain the repository

With access to the private repository, clone it and make commits and pushes inside the checkout:

```bash
git clone https://github.com/jerolan/shapeup-illustrations.git
cd shapeup-illustrations
```

In dotfiles, the checkout lives at `agents/skills/shapeup-illustrations`. Commit and push the skill from that directory:

```bash
git -C agents/skills/shapeup-illustrations status
git -C agents/skills/shapeup-illustrations add README.md README.es.md
git -C agents/skills/shapeup-illustrations commit -m "Update illustration documentation"
git -C agents/skills/shapeup-illustrations push origin main
```

Stage only the files you changed. After a skill commit, stage the submodule path in dotfiles to record its new commit. Commit that pointer separately when ready. A new machine needs GitHub access to initialize this private submodule.
