# GPT generation and delivery

## Native GPT image tool

Discover the runtime's native GPT/OpenAI image-generation tool (`image_gen`, `image_generation`, or equivalent) and use it directly. Respect its current schema and tool instructions rather than hardcoding a model version or unsupported resolution.

Inspect local image references before use. When the tool supports local reference paths, attach only the selected drawings. Otherwise use its supported conversation-image mechanism with the smallest set containing those references. For an edit, include the target and preserve its requested characteristics.

Generate the actual bitmap with GPT. Do not substitute SVG, HTML, Canvas, Pillow drawing, or a screenshot renderer. Local file tools may copy, inspect, or package assets; generative changes go through GPT.

Return native generated-image results through the runtime's image presentation helper. If the tool produces local files, copy the chosen result to the user's destination and verify the copied file. If only an inline image is available, return it and state that no local file was saved; never invent a download path.

## Authenticated Codex fallback

When the native tool is absent, use an installed, authenticated Codex CLI that has GPT image generation available. Check `codex --help` and `codex exec --help` locally for current flags. Run in the target project, supply selected references using the supported image flags, and ask Codex to use its built-in image generator and save the result at the exact requested destination. Check the result with an image viewer rather than trusting a text response.

If neither route is available, state the missing capability and retain a ready-to-use prompt. Do not claim an image was generated. Do not silently replace GPT with a different provider or require a new API key while an authenticated route is available.

## Files

Keep each final bitmap together with a short Markdown sidecar recording its core idea, exact visible text, aspect ratio, generation route, alt text, and style-reference filenames when local delivery is requested. Preserve existing files with versioned names. Store article images in the requested project rather than only in the generator cache.

For progression spread across files, include the ordered state table and continuity reference in one sequence sidecar. Inspect the sequence in reading order as well as checking each bitmap independently.
