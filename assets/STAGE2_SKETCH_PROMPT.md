# RÛN — Especificación de producción: boceto real de personaje (Stage 2)

## Estado
`assets/RUN_CLAUDE_VISUAL_DRAFT.svg` (rama `claude/issue-1-20260915-0735`) queda confirmado como diagrama estructural de apoyo (block-in), **no** como boceto de personaje ni como arte final de Stage 2.

## Bloqueo técnico confirmado
Este entorno (Claude Code ejecutado vía GitHub Actions) no tiene acceso a ningún modelo ni herramienta de generación de imágenes raster (no hay `ImageGen`/difusión, no hay renderer, no hay acceso a APIs de generación visual). Las únicas salidas visuales posibles aquí son código vectorial (SVG) o marcado, que no alcanza la línea de forma orgánica ("form language") pedida. Por eso no se produce aquí otro SVG haciéndolo pasar por boceto.

**Camino ejecutable siguiente:** este archivo es el prompt de producción, listo para pegar en un entorno de Claude con generación de imágenes (o cualquier otra herramienta de concept art raster). El resultado queda marcado como **pendiente de generación** hasta que se ejecute ahí.

## Prompt de generación (listo para usar)

```
Character concept sketch, front-view full body, monochrome graphite/ink concept-art
sketch style with loose construction lines and light rendering (NOT vector, NOT flat
icon shapes, NOT geometric primitives) — readable human anatomy, real cloth/leather
folds, real muscle and bone structure.

CHARACTER: RÛN, a lean and agile prehistoric hunter-tracker of megafauna. Alert
standing pose, torso tilted 10-15° forward, head turned ~10° to their own right
(the organic-eye side), weight centered, narrow/agile leg stance (not a wide power
stance). Slender, athletic, weathered build — not bulky.

ORIENTATION (mandatory, front view, character facing viewer):
- Character's LEFT eye is bionic/implanted → appears on the RIGHT side of the image.
- Character's LEFT arm is a prosthetic → appears on the RIGHT side of the image,
  same length as the organic arm, slightly slimmer.
- Character's RIGHT arm and hand are organic and dominant → appears on the LEFT
  side of the image.
- Left shoulder (prosthetic side) reads slightly higher/heavier than the right.

MATERIALS (dominant to accent, prehistoric only — no sci-fi surfacing):
- Dominant: tanned animal leather/hide clothing, wrapped and layered, sinew lacing.
- Secondary: carved bone/antler ornaments and joint reinforcements.
- Accents: knapped flint/obsidian shards (conchoidal fracture edges) as decorative
  and functional inserts, tendon cordage, hardened resin joints, structural wood
  only where functional, and a dark graphite/ceramic-like "unknown technology"
  material worked into the implant and prosthetic joints as if it were a natural
  material — not metal, not plastic, no visible circuitry or cables, no exposed
  mechanisms, no panel lines.
- Palette: charcoal, earth, muted browns, bone/ivory, reddish ochre, obsidian/graphite,
  with an extremely faint pale blue-white glow ONLY at the implant socket and the
  prosthetic's joint seams — barely visible, not neon, not a HUD.

VISUAL HIERARCHY (in this priority order):
1. The implanted left eye and its faint cave-painting-inspired tracking marks
   around the socket (geometric rock-art motifs, not digital HUD glyphs).
2. The integrated prosthetic left arm — discreet, following the natural arm
   silhouette, not an oversized robotic limb.
3. Contained technology hinted at inside the weapons (subtle, not glowing circuitry).

WEAPONS (visible on the body, not necessarily in hand):
- Atlatl (spear-thrower) slung diagonally across the back at ~45°, based on a real
  atlatl form, mechanically amplified — no energy beams, no glowing barrels.
- "Fracture axe": a hafted stone/flint axe at the hip/lower back, a real knapped
  stone axe silhouette with a contained technological core hinted at subtly in the
  haft binding, not an obvious gadget.

HARD EXCLUSIONS: no cyberpunk armor, no sci-fi plating, no neon, no holographic HUD,
no exaggerated robotic arm, no visible wires/cables/circuit panels, no claw-type
prosthetic hand, no extra gadgets, no symmetric tech distributed across the whole body.

RENDER NOTES: this is a Stage 2 concept sketch — anatomy, proportions, silhouette,
material hierarchy and orientation must be clearly readable; fine hair, weapon
micro-detail and implant glyph detail are not required yet.
```

## Negative prompt / restricciones
```
vector art, flat icon, geometric primitives, 3D render, cyberpunk armor, sci-fi
plating, neon glow, holographic UI, exposed circuitry, cables, metal exoskeleton,
claw hand, symmetrical body technology, glowing weapon barrels, modern clothing
```

## Criterios de evaluación al recibir el resultado
Los mismos de Stage 2 en `RUN_PROJECT_STATE.md`: proporciones frontales, orientación izquierda/derecha, asimetría de hombros, masa de torso/ropa, jerarquía de materiales, proporción del brazo protésico, ubicación del implante, postura y legibilidad general — evaluados ahora sobre anatomía y forma real, no sobre un diagrama.

## Próxima acción
Ejecutar este prompt en un entorno de Claude (u otra herramienta) con capacidad real de generación de imágenes raster, subir el resultado a `assets/` (por ejemplo `assets/STAGE2_SKETCH_V1.png`) y volver a activar la revisión de Claude sobre ese artefacto.
