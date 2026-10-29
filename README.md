# Shape Up illustrations

[Español](README.es.md)

Make an idea understandable through an original hand-drawn illustration: confident
simple lines, purposeful whitespace, and color when something deserves emphasis.
Explain one claim, develop an abstract concept, or show people working through an idea.

## Use cases

These original generated examples show three compositions. Reuse the explanatory
mechanism for your subject; the skill chooses a representation to fit the claim.
Generation varies between runs. Run these prompts at this repository's root;
in another project, change output paths and use that project's DESIGN.md.

### 1. One idea, one image

**Starting more work does not remove a bottleneck.** Work cards crowd a wide
channel before a narrow throat. Violet emphasizes the constraint, while the
single-file outlet shows why adding more cards only increases the queue.

![Work cards accumulate before a narrow violet-marked throat and pass through one at a time.](examples/simple-idea/image.png)

```text
Use $shapeup-illustrations to explain that starting more work does not remove
a bottleneck. Make one static image with a clear visual relationship, without
panels or a time sequence. Choose the representation; add Spanish labels only
if needed. Use examples/DESIGN.md. Save under examples/simple-idea/.
```

[Exact generation prompt](examples/simple-idea/generation-prompt.txt) ·
[Generation details](examples/simple-idea/example.md).

### 2. People develop an idea

**Agreeing on an urgency criterion helps organize a shared proposal.** Two
coworkers develop the same whiteboard through four panels: loose cards, an
explicit urgency criterion, priority groups, and a trial with cases. The violet
clock marks preserve the criterion as the board changes.

![Four panels show two coworkers agreeing on urgency, grouping the same cards by priority, and trying the arrangement with cases.](examples/character-narrative/image.png)

```text
Use $shapeup-illustrations for four panels in a 2x2 grid with two coworkers
working on the same artifact. Explain that agreeing on an urgency criterion
helps organize their proposal. Make the shared drawing change visibly.
Include these exact Spanish lines in speech bubbles, in reading order:
"¿Qué problema resolvemos?"
"Encontrar lo urgente."
"Agrupemos por prioridad."
"Probemos con estos casos."
Use examples/DESIGN.md. Save under examples/character-narrative/.
```

[Exact generation prompt](examples/character-narrative/generation-prompt.txt) ·
[Dialogue, composition and inspection](examples/character-narrative/example.md).

### 3. One abstract concept evolves

**A piece's importance depends on what it supports, not its size.** The same
Jenga-inspired tower stands after the large cap A is removed, then tips when its
small support B is removed. Violet tracks B across all states. The changing
object carries the argument, while short Spanish notes guide the reading.

![The same block tower stands after cap A is removed and tips when its small violet support B is removed.](examples/conceptual-progression/image.png)

```text
Use $shapeup-illustrations to explain that a piece's importance depends on what
it supports, not its size. Show an abstract progression of the same Jenga-inspired
block tower. Keep the object and its identities recognizable; use accent only
for meaningful emphasis. No people. Choose the states and any necessary Spanish
text. Use examples/DESIGN.md. Save under examples/conceptual-progression/.
```

[Exact generation prompt](examples/conceptual-progression/generation-prompt.txt) ·
[States, targeted correction and observed limitations](examples/conceptual-progression/example.md).

## Setup and compatibility

Invoke `$shapeup-illustrations` or ask for the skill by name. Describe the idea,
audience, exact visible text if needed, and destination. Local deliverables default
to `assets/<topic-slug>-shapeup/` in your project, with a Markdown generation record.

Use an agent with native GPT image generation, or an installed authenticated Codex
CLI with that capability. An authenticated route needs no new API key. Without
an available route the agent can provide a prompt, but cannot generate the image.
Outputs are drawn artwork; screenshots and screenshot-based compositions are excluded.

### Colors and DESIGN.md

For each choice independently: **explicit request → applicable project DESIGN.md →
skill defaults**. The nearest scoped document along the output path takes precedence
when project values conflict. Defaults are white background and near-black ink.
An accent is optional and must have an explanatory role; the examples' violet is
not a global theme.

```text
Use this project's DESIGN.md for the palette.
```

```text
Respect DESIGN.md, but use blue #2563EB to emphasize the revised scope.
```

Changing the accent preserves the other palette choices. DESIGN.md guides colors
and background while the drawing retains its visual language. Requested hex colors
may be approximated by GPT. [examples/DESIGN.md](examples/DESIGN.md) applies only
to this gallery. See [style and color guidance](references/style.md).

## References and rights

Original Basecamp drawings in `assets/references/` calibrate style; their rights
remain with their authors. [Sources and provenance](references/sources.md) explain
which references to select. Approved generated examples are in `examples/`.
Development iterations and review runs are separate and are not default generation
context. See [development notes](development/README.md) when maintaining the skill.

## Attribution & disclaimer

This is an independent, unofficial project inspired by the visual language of [Shape Up](https://basecamp.com/shapeup), written by Ryan Singer and published by Basecamp (37signals). It is not affiliated with, sponsored by, or endorsed by Ryan Singer, Basecamp, or 37signals.

The skill is intended to generate original illustrations rather than copy the book's artwork. This repository currently includes copies of original Shape Up drawings in `assets/references/` as visual references. Those drawings and any associated trademarks remain the property of their respective rights holders. They are **not** covered by this project's MIT License. Attribution does not grant permission to copy, adapt, or redistribute third-party artwork.

See [sources and provenance](references/sources.md) for links to the original drawings. Rights holders can [open a GitHub issue](https://github.com/jerolan/shapeup-illustrations/issues) to raise concerns or request a review of the material.

## License

The [MIT License](LICENSE) applies only to original material that the project author owns or has the right to license. It does not apply to the bundled Shape Up reference artwork or other third-party materials.

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
