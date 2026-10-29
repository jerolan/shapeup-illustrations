# Ilustraciones Shape Up

[English](README.md)

Crea ilustraciones originales con el lenguaje visual de Shape Up: trazos simples, espacio en blanco y color para dirigir la atención. Explica una idea, muestra cómo evoluciona o cuenta cómo un equipo la desarrolla.

## Casos de uso

Estos tres ejemplos exploran la misma app de tareas con una complejidad visual creciente. Son ilustraciones originales generadas. Los prompts piden el texto en inglés que aparece en las imágenes; la generación puede variar entre ejecuciones.

Ejecuta los prompts desde la raíz de este repositorio. En otro proyecto, cambia las rutas de salida y usa el `DESIGN.md` de ese proyecto.

### 1. Una idea simple

Una sola imagen hace visible una decisión de alcance: la primera versión incluye agregar y completar tareas. El límite violeta encierra únicamente esas dos acciones. No hacen falta personajes ni diálogo.

![Una lista de papel con Add task y Complete task dentro de un límite violeta.](examples/01-single-idea.png)

```text
Usa $shapeup-illustrations para representar el alcance inicial de una app de tareas.
Dibuja una lista de papel con solo "Add task" y "Complete task", ambas con casillas
vacías, dentro de un límite violeta. Sin personajes, título ni diálogo.
Usa examples/DESIGN.md para la paleta. Haz una imagen horizontal.
Guárdala en examples/01-single-idea.png.
```

[Detalles de generación y paleta](examples/01-single-idea.md).

### 2. Un concepto que evoluciona

La misma lista cambia de izquierda a derecha: propone tres acciones, tacha los recordatorios mientras selecciona las otras dos y conserva solo el alcance inicial. La hoja y las entradas sin cambios siguen siendo reconocibles para que el lector pueda seguir la revisión.

![Tres estados de una lista: agregar, completar y recordatorios; recordatorios tachados fuera del alcance seleccionado; solo agregar y completar permanecen.](examples/02-list-progression.png)

```text
Usa $shapeup-illustrations para mostrar una propuesta de app de tareas en tres pasos.
Haz una imagen horizontal con tres listas de papel, de izquierda a derecha:
1. Casillas vacías con "Add task", "Complete task" y "Reminders".
2. La misma lista, con "Reminders" tachado y un límite violeta que encierre
   solo "Add task" y "Complete task".
3. La misma hoja y límite, conservando solo "Add task" y "Complete task".
Mantén la hoja, las posiciones de las filas y la letra. Sin personajes ni diálogo.
Usa examples/DESIGN.md para la paleta. Guarda examples/02-list-progression.png.
```

[Detalles de generación y tabla de estados](examples/02-list-progression.md).

### 3. Una conversación que transforma la idea

Los personajes, gestos y diálogos añaden las razones de cada cambio. Lee de izquierda a derecha y después hacia abajo: proponer la app, cuestionar los recordatorios, acotar el alcance y probar el prototipo en papel. La pizarra compartida cambia con la conversación.

![Cuatro viñetas muestran a dos compañeros proponiendo una app de tareas, cuestionando recordatorios, acotando el alcance y probando el prototipo en papel.](examples/02-idea-conversation.png)

```text
Usa $shapeup-illustrations para mostrar a dos compañeros desarrollando una idea de app de tareas.
Haz una imagen de cuatro viñetas en una cuadrícula de 2x2. Mantén las mismas personas y pizarra.
Muestra la idea, una objeción sobre recordatorios, un alcance menor y una prueba en papel.
Pon este diálogo en globos dentro de las viñetas, en orden de lectura:
"Let's build a task app."
"Do we need reminders now?"
"Start with add and complete."
"Let's try this first."
Usa examples/DESIGN.md para la paleta. Guarda examples/02-idea-conversation.png.
```

[Detalles de generación, diálogo y continuidad](examples/02-idea-conversation.md).

## Configuración y compatibilidad

### Invocar la skill

Invoca `$shapeup-illustrations` en tu agente o pide la skill por su nombre. Describe la idea, la audiencia, el texto exacto que debe aparecer y el destino deseado. El agente elige una composición, genera la imagen y la inspecciona. Por defecto, guarda las imágenes locales en `assets/<topic-slug>-shapeup/` dentro de tu proyecto, junto con un archivo Markdown complementario.

Una escena puede explicar una idea; las secuencias muestran cambios significativos. Las conversaciones de cuatro viñetas usan una cuadrícula de 2×2, pero hay otras composiciones y cantidades de viñetas disponibles. La skill crea escenas y diagramas dibujados, excluyendo capturas y composiciones basadas en capturas.

### Generación de imágenes

Usa un agente con generación de imágenes GPT nativa o Codex CLI instalado y autenticado con generación de imágenes GPT disponible. No necesitas una clave API nueva si cuentas con una opción autenticada. Si ninguna está disponible, el agente puede entregar un prompt, pero no generar la imagen.

### Colores y DESIGN.md

Para cada color, la prioridad es **petición explícita → `DESIGN.md` aplicable al proyecto → valores por defecto de la skill**. El agente revisa la raíz del proyecto y la ruta del directorio de salida; si hay valores en conflicto, prevalece el documento de diseño más cercano.

Por ejemplo:

```text
Usa el DESIGN.md de este proyecto para la paleta.
```

Para cambiar solo el acento:

```text
Respeta DESIGN.md, pero usa azul #2563EB para el límite de alcance.
```

Cambiar el acento conserva las demás decisiones de la paleta. El documento de diseño guía los colores y el fondo mientras la ilustración mantiene su estilo dibujado a mano. Sin indicaciones del proyecto ni una petición explícita, la skill usa negro sobre blanco con acentos funcionales discretos.

[examples/DESIGN.md](examples/DESIGN.md) solo aplica a estos ejemplos, no a los proyectos que instalan la skill. GPT puede aproximar un color hexadecimal sin reproducirlo exactamente. Consulta las [reglas de color y diseño](references/style-dna.md#custom-accents-and-designmd).

## Referencias y derechos

Los dibujos de Basecamp en `assets/examples/` son referencias de calibración. Sus autores conservan sus derechos. Consulta las [fuentes y su procedencia](references/sources.md). La skill crea escenas nuevas en lugar de copiar esas obras.

## Mantenimiento del repositorio

Si tienes acceso al repositorio privado, clónalo y haz los commits y pushes dentro de la copia:

```bash
git clone https://github.com/jerolan/shapeup-illustrations.git
cd shapeup-illustrations
```

En dotfiles, la copia está en `agents/skills/shapeup-illustrations`. Haz los commits y pushes de la skill desde ese directorio:

```bash
git -C agents/skills/shapeup-illustrations status
git -C agents/skills/shapeup-illustrations add README.md README.es.md
git -C agents/skills/shapeup-illustrations commit -m "Update illustration documentation"
git -C agents/skills/shapeup-illustrations push origin main
```

Prepara solo los archivos que cambiaste. Después de un commit de la skill, prepara la ruta del submódulo en dotfiles para registrar el nuevo commit. Confirma ese puntero por separado cuando corresponda. Una máquina nueva necesita acceso a GitHub para inicializar este submódulo privado.
