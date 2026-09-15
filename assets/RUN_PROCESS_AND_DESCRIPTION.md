# RÛN — Documentación de proceso, texto descriptivo y paquete final

TP1 individual — Desarrollo de Videojuegos. Side-quest: PREHISTORIA.

## 1. Texto descriptivo del personaje

RÛN es una rastreadora/rastreador de megafauna en una prehistoria alternativa donde restos de tecnología desconocida —caídos del cielo mucho antes del presente narrativo— fueron encontrados, reinterpretados y reintegrados a la cultura material humana como si fueran piedra, hueso o resina: "piedras del cielo". RÛN perdió el ojo y el brazo izquierdos en una cacería o un accidente con esos restos, y la comunidad los reemplazó con un implante ocular y una prótesis de brazo construidos con la misma lógica que cualquier otra herramienta del grupo: envueltos en cuero y tendón, encastrados en hueso, nunca expuestos como mecanismo. El implante traduce lo que ve en un lenguaje visual heredado de la pintura rupestre, y es ese sistema —no la prótesis— el verdadero corazón de su ventaja como rastreadora.

Complexión esbelta y ágil, apta para el rastreo de larga distancia más que para el choque frontal. Viste capas de cuero y piel con acentos de hueso, ocre y obsidiana/sílex; lleva el atlatl de impulso cruzado en diagonal sobre la espalda y el hacha de fractura enganchada en la cadera del lado dominante (orgánico). El cabello, medio-largo e irregular, lleva un mechón atado que despeja el rostro sin domesticar del todo su aspecto de superviviente.

Visualmente, RÛN debe leerse primero como una cazadora/cazador prehistórico real, y solo en un segundo vistazo revelar que parte de su cuerpo y su equipo son tecnología reinterpretada. Ningún elemento debe evocar ciencia ficción, cyberpunk o fantasía genérica.

## 2. Metodología y roles

- **Claude (este entorno):** desarrollo visual — bocetos de concepto, consistencia entre vistas, evaluación de artefactos, decisiones de diseño finales cuando el archivo de estado no las resuelve por sí solo.
- **ChatGPT:** coordinación del flujo, mantenimiento del estado en GitHub/Issue #1, y — crítico para la continuidad — **merge de las Pull Requests de Claude a `main`** antes de disparar la etapa siguiente (ver nota de proceso en `RUN_PROJECT_STATE.md`).
- **Usuario:** no produce arte manualmente; define el encargo académico y valida el resultado final.

Todas las decisiones de esta sesión se tomaron de forma autónoma siguiendo `CLAUDE.md` y los bloqueos ya fijados en `RUN_PROJECT_STATE.md`, sin pedir aprobación intermedia.

## 3. Bitácora de decisiones por etapa

**Etapa 1 — Silueta.** Pose A (Alerta) aprobada; corrección de Claude: estrechar la base de piernas para reforzar agilidad.

**Etapa 2 — Vista frontal.** El artefacto original (`STAGE2_FRONT_VIEW.jpg`) no pudo evaluarse: es un JPEG progresivo de 240×252px que el visor de este entorno no decodifica, y el entorno no dispone de herramientas de conversión de imagen. En lugar de bloquear el proyecto en esa limitación, Claude produjo un boceto de concepto real y propio (`RUN_STAGE2_CONCEPT_SKETCH.svg`) construido directamente desde el concepto bloqueado, y lo fijó como entregable vigente de la etapa. Se definieron ahí las proporciones de referencia (≈8.3 cabezas) que rigen todas las vistas posteriores.

**Etapa 3 — Vistas lateral y posterior.** Derivadas geométricamente del mismo esqueleto de proporciones que la vista frontal (mismas coordenadas verticales, silueta de torso reflejada) para garantizar consistencia real entre vistas en vez de re-interpretar el diseño desde cero. Se fijó la regla de que la vista posterior invierte la lateralidad de la frontal (el lado protésico pasa de aparecer a la derecha de la imagen a la izquierda), por ser la consecuencia física correcta de girar al personaje 180°.

**Etapa 4 — Lámina de detalle.** Close-ups del implante ocular, la articulación protésica del codo y un muestrario de materiales, todos derivados de lo ya bloqueado — sin introducir diseño nuevo.

**Bloqueo de proceso identificado:** las ramas de ejecuciones anteriores (`claude/issue-1-20260915-0735`, `-0741`, `-0744`) no llegaron a mergearse a `main`, y este entorno no tiene permiso para hacer `git fetch` de ramas remotas fuera de la rama de trabajo actual en modo no interactivo. Por eso los artefactos de Etapas 2 y 3 se reconstruyeron íntegramente en la rama de esta ejecución en vez de asumir contenido no verificable. Corrección de proceso para que esto no se repita: **mergear cada PR de Claude a `main` antes de disparar la siguiente etapa.**

## 4. Paquete académico — estado de empaquetado

| Elemento requerido | Archivo | Estado |
|---|---|---|
| Concepto/proceso inicial | `RUN_PROJECT_STATE.md` | Completo |
| Boceto de personaje (frontal) | `assets/RUN_STAGE2_CONCEPT_SKETCH.svg` | Completo |
| Consistencia lateral | `assets/RUN_STAGE3_SIDE_VIEW.svg` | Completo |
| Consistencia posterior | `assets/RUN_STAGE3_BACK_VIEW.svg` | Completo |
| Close-up / lámina de detalle | `assets/RUN_STAGE4_DETAIL_SHEET.svg` | Completo |
| Concepto de armas (2) | `assets/RUN_WEAPONS_CONCEPT_SKETCH.svg` | Completo |
| Documentación de proceso | este archivo | Completo |
| Texto descriptivo | sección 1 de este archivo | Completo |
| Diagrama estructural interno (no cuenta como boceto/arte final) | `assets/RUN_CLAUDE_VISUAL_DRAFT.svg` | Referencia interna únicamente |

Pendiente fuera de este entorno: exportar los SVG a PNG/JPG de alta resolución si la entrega final lo exige en formato rasterizado (este entorno de Claude Code vía GitHub Actions no tiene acceso a un renderer raster ni a ejecución de scripts de conversión en modo no interactivo).
