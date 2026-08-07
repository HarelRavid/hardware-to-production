---
id: H2P-PW-186
title: FDM PLA
object_type: Material
parent_process: H2P-PW-021
status: Researching
lifecycle: [POC, Prototype, Engineering Prototype]
tags: [FDM, PLA, polymer-am, rapid-prototyping]
---
# FDM PLA

## Definition
Polylactic acid (PLA) feedstock used in material-extrusion additive manufacturing. This object covers PLA as a prototype material, not generic bulk PLA properties.

## Engineering use
PLA is useful when fast, predictable printing, dimensional iteration and stiffness are more important than elevated-temperature performance, impact toughness or long-term environmental durability.

## Decision criteria
Prefer PLA for visual/form/fit models, quick geometry checks, fixtures with modest thermal/mechanical demand and early design iteration. Escalate to PETG, ABS/ASA, nylon, reinforced polymers, SLA engineering resin, PBF or CNC when the prototype must represent demanding heat, impact, wear, outdoor or production-material behavior.

## Key limitations
- Printed-part properties depend on process settings, geometry and orientation.
- Heat resistance is relatively limited compared with common engineering thermoplastics.
- High apparent tensile stiffness/strength does not imply high impact toughness.
- Standard PLA should not be used as a proxy for injection-molded production material unless the learning objective makes that substitution acceptable.

## Relationships
| Type | Target | Strength | Reason |
|---|---|---|---|
| MATERIAL_FOR | H2P-PW-021 | Strong | PLA is a common FDM/FFF feedstock. |
| SELECTED_BY | H2P-PW-176 | Strong | FDM material selection determines when PLA is appropriate. |
| LIMITED_BY | H2P-PW-174 | Strong | PLA prototypes may have low production representativeness for non-PLA production parts. |
| AFFECTED_BY | H2P-PW-033 | Strong | Orientation changes printed-part behavior. |

## Evidence notes
UltiMaker's Tough PLA data show HDT around 58 °C and orientation-dependent tensile yield values, illustrating why printed-part data must retain test orientation and formulation context.

## Podcast use
Prototype Shop — FDM materials and material-selection tradeoffs.
