# RÛN — PROJECT STATE

## Objetivo
TP1 individual — Desarrollo de Videojuegos. Side-quest: PREHISTORIA.

El proyecto final debe estar en español.

## Concepto bloqueado
- Personaje: RÛN.
- Prehistoria alternativa con restos de tecnología desconocida reinterpretados como “piedras del cielo”.
- RÛN es rastreador/cazador de megafauna.
- Ojo IZQUIERDO implantado.
- Brazo IZQUIERDO protésico.
- Mano DERECHA orgánica y dominante.
- La tecnología debe sentirse reinterpretada desde una lógica prehistórica, no como sci-fi/cyberpunk.
- Sistema de rastreo del implante: información representada mediante lenguaje visual inspirado en pinturas rupestres.

## Jerarquía visual bloqueada
1. Foco principal: implante ocular + sistema de rastreo rupestre.
2. Foco secundario: brazo protésico integrado y discreto.
3. Foco terciario: tecnología contenida en las armas.

## Materiales
Dominantes:
- cuero / piel animal.

Secundario:
- hueso.

Acentos:
- sílex / obsidiana;
- tendones;
- resina;
- madera cuando sea funcional;
- material tecnológico oscuro tipo grafito/cerámica.

## Paleta
- carbón;
- tierra;
- marrones apagados;
- hueso / marfil;
- ocre rojizo;
- obsidiana / grafito.

Acento tecnológico:
- blanco azulado MUY tenue.

## Armas bloqueadas
### 1. Atlatl de Impulso
Basado en un atlatl prehistórico real. La tecnología amplifica mecánicamente el lanzamiento. No dispara energía ni rayos.

### 2. Hacha de Fractura
Basada en un hacha/herramienta de piedra. Núcleo tecnológico contenido que genera microvibración en el impacto. Funciona como arma y herramienta.

## Restricciones visuales
- No cyberpunk.
- No armaduras sci-fi genéricas.
- No neón.
- No HUD holográfico.
- No brazo robótico exagerado.
- No circuitos/cables/paneles visibles.
- No manos protésicas tipo garra.
- No gadgets extra.
- No tecnología distribuida simétricamente por todo el cuerpo.

## Investigación realizada
Reference pack ya investigado con:
- Cro-Magnon / Ötzi;
- ropa y construcción prehistórica;
- flintknapping / fractura concoidea;
- herramientas de hueso y asta;
- atlatls reales;
- hachas de piedra enmangadas;
- arte rupestre / signos geométricos;
- ocre y pigmentos;
- megafauna;
- contraste de materiales.

## Etapa 1 — SILUETA
ESTADO: APROBADA / CERRADA POR CLAUDE.

Pose elegida: A — Postura de Alerta.

Especificaciones:
- torso: 10–15° hacia adelante;
- cabeza: 10° hacia la derecha (lado del ojo orgánico);
- atlatl: ~45° diagonal;
- hombro izquierdo ligeramente más alto/pesado;
- figura esbelta, atlética, resistente;
- brazo izquierdo protésico del mismo largo que el orgánico pero algo más delgado;
- peso centrado;
- mantener lectura ágil, no power stance.

Corrección de Claude al cerrar Stage 1:
- La base de piernas de Pose A estaba algo ancha. En la vista frontal, estrechar un poco la postura para reforzar agilidad.

## Etapa 2 — VISTA FRONTAL
ESTADO: CERRADA POR CLAUDE — boceto de concepto real producido directamente por Claude.

Nota de continuidad: el block-in `assets/STAGE2_FRONT_VIEW.jpg` (JPEG progresivo, 240×252px) sigue bloqueado técnicamente para evaluación visual en el entorno de Claude Code (sin soporte de JPEG progresivo ni herramientas de conversión con permisos habilitados). En lugar de seguir bloqueado en esa evaluación, Claude produjo un boceto de concepto propio y avanzó la etapa, tal como fue indicado explícitamente por el usuario. Ese JPG queda como referencia histórica, no como bloqueante.

Orientación obligatoria en vista frontal:
- RÛN mira al espectador.
- Su lado IZQUIERDO aparece a la DERECHA de la imagen.
- Ojo implantado izquierdo = derecha de la imagen.
- Brazo protésico izquierdo = derecha de la imagen.
- Brazo orgánico derecho = izquierda de la imagen.

El block-in de Stage 2 debe evaluarse SOLO por:
- proporciones frontales;
- orientación izquierda/derecha;
- asimetría de hombros;
- masa de torso/ropa;
- jerarquía de materiales;
- proporción del brazo protésico;
- ubicación del implante;
- postura y legibilidad general.

No evaluar todavía:
- render;
- textura;
- pelo fino;
- detalles de armas;
- símbolos finos del implante.

### Artefactos de Stage 2
- Boceto de concepto (autoría Claude, deliverable vigente): `assets/RUN_STAGE2_CONCEPT_SKETCH.svg`
- Lámina de armas (autoría Claude): `assets/RUN_WEAPONS_CONCEPT_SKETCH.svg`
- Diagrama estructural previo (solo apoyo interno, no es boceto/arte): `assets/RUN_CLAUDE_VISUAL_DRAFT.svg` (rama `claude/issue-1-20260915-0735`, no mergeada a `main`)
- Block-in legado sin evaluar (bloqueado técnicamente, ver nota arriba): `assets/STAGE2_FRONT_VIEW.jpg`

Proporciones bloqueadas del boceto de concepto (referencia para consistencia en Etapa 3):
- Altura total ≈ 8.3 alturas de cabeza (figura esbelta/ágil).
- Ancho de hombros ≈ 2.4 alturas de cabeza; hombro del lado protésico (izquierdo del personaje) ligeramente más alto y pesado.
- Cintura/cadera estrechadas respecto al block-in original (corrección de Etapa 1 aplicada).
- Brazo protésico: mismo largo que el orgánico, silueta ligeramente más delgada.
- Postura: peso centrado, piernas en estance angosto para lectura ágil.

## Etapa 3 — VISTA LATERAL Y POSTERIOR (blueprint bloqueado)
ESTADO: BLUEPRINT DEFINIDO POR CLAUDE, BOCETOS PENDIENTES DE PRODUCCIÓN.

Reglas de consistencia obligatorias (derivadas del boceto frontal):
- Mantener las proporciones bloqueadas arriba (misma altura total, mismo largo de brazos/piernas).
- Vista lateral: mostrar el atlatl en toda su diagonal real a lo largo de la espalda (~45°, saliendo desde la cadera derecha del personaje hasta sobre el hombro izquierdo), y el hacha de fractura visible en la cadera/zona lumbar, enfundada.
- Vista lateral debe elegirse desde el lado del ojo orgánico (perfil derecho del personaje) para lectura clara de rasgos, dejando el lado protésico sugerido en el contorno de espalda.
- Vista posterior: el cabello (medio-largo, irregular, parcialmente atado) cae sobre la espalda y debe leerse compatible con el mechón atado ya definido en el boceto frontal.
- Vista posterior debe mostrar con claridad el anclaje del atlatl y el hacha en la espalda/cadera sin bloquear la silueta general.
- No introducir nuevos materiales o colores fuera de la paleta y jerarquía ya bloqueadas.

## Flujo de trabajo compartido
- Claude: lee `RUN_PROJECT_STATE.md`, produce bocetos de concepto propios cuando se le pide un artefacto visual real, evalúa artefactos cuando el formato lo permite, y define blueprints de consistencia entre vistas.
- ChatGPT: coordina el estado del repo, releva tareas y produce material adicional cuando corresponda.
- Usuario: no dibuja ni produce manualmente; usa ambos asistentes para desarrollar el proceso.

## Próxima acción
Producir los bocetos de concepto de VISTA LATERAL y VISTA POSTERIOR siguiendo el blueprint de Etapa 3, manteniendo la consistencia de proporciones, materiales y ubicación de armas ya bloqueada.
