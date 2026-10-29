# Una idea en una imagen

## Idea

Poner más trabajo en marcha no elimina un cuello de botella.

## Solicitud del usuario

Genera una sola imagen que explique esa afirmación mediante una relación visual clara. Una composición estática; sin viñetas ni secuencia temporal. Elige la representación. Texto visible solo si hace falta y en español.

## Referencias e imágenes adjuntas

Referencia inspeccionada: `/Users/jeromeolverasanchez/.dotfiles/agents/skills/shapeup-illustrations/assets/references/03-overwhelming-work.png`.

Función: Calibración de contornos de marcador, repetición de elementos de trabajo y acumulación espacial. No se reprodujeron su personaje ni su diálogo.

## Generación y verificación

Herramienta nativa GPT `image_gen__imagegen`, con `transparent_background: false`. Generaciones secuenciales en esta sesión, sin subagentes ni otras sesiones. Archivo final: [image.png](image.png). Sin reparación ni borrador descartado; se conservó el original del generador.

Formato verificado mediante firma/cabecera PNG: **1672 × 941 px**, RGB de 8 bits, sin canal alfa. Fondo blanco observado. Paleta de `/private/tmp/shapeup-fresh-review-20261029/DESIGN.md`: fondo #FFFFFF, tinta #171717 y acento #7C3AED con función semántica. Los hex son objetivos del prompt, no una certificación colorimétrica del bitmap.

No se adjuntaron imágenes: la instrucción vigente de la herramienta nativa exige omitir `referenced_image_paths` y `num_last_images_to_include` para imágenes nuevas. Las referencias indicadas se abrieron e inspeccionaron con `view_image`; funcionaron como calibración visual previa. No se consultaron iteraciones ni conversaciones anteriores. La inspección aquí es de contenido y cumplimiento observable; no expresa aprobación estética del usuario.

## Prompt EXACTO enviado al generador

```text
Claim: Starting more work does not remove a bottleneck.
Carrier and composition: One static landscape drawing of a work channel running left to right. Two continuous hand-drawn channel walls form a wide inlet on the left, taper into a very narrow throat at center-right, and continue as a single-file outlet. Many small unfilled rectangular work cards crowd the wide upstream space, visibly queued at the throat; one card fits through it at a time, and only two separated cards are downstream. A short simple arrow from the left shows additional cards entering the already crowded inlet. The narrow opening is the cause of the queue. No panels, comparison scenes or time sequence.
Drawing: Confident economical pen and marker contours, rounded ends, slightly uneven corners, flat unfilled forms, generous purposeful whitespace, compact framing. Original explanatory hand drawing in the spare visual grammar of Shape Up, not a polished vector diagram. No people, shading or textures.
Palette: Opaque white #FFFFFF background, near-black #171717 ink. Violet #7C3AED only on the two short wall segments defining the narrow throat; all cards and other structure in ink.
Visible text: None.
References: The original Shape Up drawing 03-overwhelming-work.png was inspected for spare marker contours, repeated outlined work items and spatial accumulation. It is style calibration only, not content to reproduce; no reference bitmap is attached because the native new-image route requires omitting image attachments.
Output: One landscape PNG, approximately 16:9, opaque white background. Intended final destination: /Users/jeromeolverasanchez/.dotfiles/agents/skills/shapeup-illustrations/development/reviews/2026-10-29-fresh-session/01-single-idea/image.png.
```

## Relación e inspección

Un canal ancho se estrecha; muchas fichas se acumulan aguas arriba, una ocupa el paso y dos quedan separadas después. Una flecha introduce más fichas hacia la acumulación. El violeta identifica únicamente el estrechamiento. Composición única, sin estados temporales ni texto.

Se observan la cola, el paso de una ficha de ancho y la salida escasa. No se detectó un defecto concreto que justificara reparación. Limitación: la relación es una metáfora cualitativa de capacidad, sin medida de velocidad ni prueba temporal del efecto de añadir trabajo.

Alt: Fichas se amontonan en un canal antes de un paso angosto violeta mientras siguen entrando más.

Original conservado: `/Users/jeromeolverasanchez/.codex/generated_images/01a18981-b806-79a0-a844-2bddf40b88b0/exec-47d9fa33-b4a1-4813-8eb0-5c66cb2559df.png`.
