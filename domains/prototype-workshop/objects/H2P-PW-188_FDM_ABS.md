---
id: H2P-PW-188
title: FDM ABS
object_type: Material
parent_process: H2P-PW-021
status: Researching
lifecycle: [Prototype, Engineering Prototype]
tags: [FDM, ABS, polymer-am, functional-prototype]
---
# FDM ABS

## Definition
Acrylonitrile-butadiene-styrene feedstock used in material extrusion for functional prototypes, housings and parts requiring more heat and impact capability than common PLA formulations.

## Engineering use
ABS is commonly selected when a prototype must better represent tough thermoplastic behavior, allow sanding/machining/finishing, or operate at temperatures where PLA is inadequate.

## Decision criteria
Use when toughness, post-processing and moderate thermal performance matter and an enclosed/controlled printing process is available. Consider ASA when outdoor UV/weathering performance is important, PETG when simpler printing and chemical/moisture resistance dominate, or PC/PC blends when higher temperature/impact capability is needed.

## Limitations
- Warpage and thermal shrinkage make large parts more process-sensitive.
- Printed ABS is not equivalent to injection-molded ABS; layer interfaces and process history remain important.
- Ventilation/EHS must be managed according to machine, material SDS and local requirements.

## Evidence notes
UltiMaker reports tensile strength around 43 MPa and HDT around 84 °C for its Method-series ABS under its specified conditions. These values are not universal ABS properties.

## Relationships
| Type | Target | Strength | Reason |
|---|---|---|---|
| MATERIAL_FOR | H2P-PW-021 | Strong | Common engineering FDM feedstock. |
| SELECTED_BY | H2P-PW-176 | Strong | Part of FDM material-selection decision. |
| COMPARED_WITH | H2P-PW-189 | Strong | ASA is a common alternative where UV/weathering matters. |
| AFFECTED_BY | H2P-PW-033 | Strong | Orientation affects printed behavior. |
| AFFECTED_BY | H2P-PW-034 | Strong | Shrinkage/warpage require dimensional compensation. |

## Podcast use
Prototype Shop — engineering FDM materials and when PLA stops being sufficient.
