Estás en una sesión fresca para probar la versión actualizada de un skill. No tienes el contexto de la conversación que la originó.

Usa $shapeup-illustrations. Lee su fuente actual en /Users/jeromeolverasanchez/.dotfiles/agents/skills/shapeup-illustrations/SKILL.md y las referencias que indique. Genera las TRES pruebas descritas abajo EN ESTA ÚNICA SESIÓN, secuencialmente. No abras subagentes, no invoques otro codex exec, no uses resume ni fork. No modifiques el skill ni los README. Puedes consultar los ejemplos activos como indica la skill, pero no leas development/iterations ni conversaciones anteriores. Usa DESIGN.md del directorio actual como paleta explícita para esta revisión; sus valores aplican a los tres destinos aunque estén bajo development/reviews.

Usa tu herramienta NATIVA de generación GPT de imágenes. No uses API scripts, SVG, HTML o dibujos programáticos como sustituto. Selecciona tú las referencias y el prompt real a partir de la skill; inspecciona referencias y resultados. Guarda o copia todos los bitmaps al destino indicado. Conserva el borrador si lo reparas. No vuelvas a generar solo por gusto estético: el usuario juzgará el estilo. Como máximo una reparación por defecto concreto.

Para cada caso guarda image.png y review.md con: idea que quieres explicar; solicitud del usuario; prompt EXACTO enviado al generador (no un resumen posterior); imágenes adjuntas y su función; tabla de estados si aplica; dimensiones/formato; breve inspección y limitaciones observadas. Indica cuál archivo es final si hubo reparación. Nunca declares aprobación estética del usuario ni éxito sin archivo verificable.

CASO Una idea en una imagen
Idea: Poner más trabajo en marcha no elimina un cuello de botella.
Solicitud: Genera una sola imagen que explique esa afirmación mediante una relación visual clara. Una composición estática; sin viñetas ni secuencia temporal. Elige la representación. Texto visible solo si hace falta y en español.
Destino: /Users/jeromeolverasanchez/.dotfiles/agents/skills/shapeup-illustrations/development/reviews/2026-10-29-fresh-session/01-single-idea

CASO Viñetas de interacción entre personas con texto
Idea: Acordar el criterio de urgencia permite organizar una propuesta compartida.
Solicitud: Genera una imagen con cuatro viñetas 2×2 y dos compañeros trabajando sobre el mismo artefacto. La propuesta cambia visiblemente con la conversación. Incluye estas líneas exactas dentro de sus viñetas, con el hablante claro, en orden de lectura: "¿Qué problema resolvemos?" / "Encontrar lo urgente." / "Agrupemos por prioridad." / "Probemos con estos casos."
Destino: /Users/jeromeolverasanchez/.dotfiles/agents/skills/shapeup-illustrations/development/reviews/2026-10-29-fresh-session/02-character-narrative

CASO Progresión de una idea abstracta
Idea: Acumular piezas terminadas no asegura una parte útil; hace falta completar una unidad coherente.
Solicitud: Genera una imagen con los estados necesarios para desarrollar esa afirmación mediante UN SOLO objeto conceptual que evoluciona. Elige un portador distinto de la torre de Jenga de los ejemplos. Conserva geometría, identidades y cambios reconocibles; cada transformación debe demostrar algo. Evita sustituirlo por escenas de personas o soluciones distintas. Etiquetas en español solo si hacen falta.
Destino: /Users/jeromeolverasanchez/.dotfiles/agents/skills/shapeup-illustrations/development/reviews/2026-10-29-fresh-session/03-abstract-progression

Entrega final: un índice en /Users/jeromeolverasanchez/.dotfiles/agents/skills/shapeup-illustrations/development/reviews/2026-10-29-fresh-session/index.md enlazando los tres resultados, y resumen breve. No commit ni push. Si la herramienta nativa no está disponible, informa del bloqueo en vez de abrir otra sesión.
