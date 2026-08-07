---
id: H2P-PW-187
title: FDM PETG
object_type: Material
parent_process: H2P-PW-021
status: Researching
lifecycle: [Prototype, Engineering Prototype]
tags: [FDM, PETG, polymer-am, functional-prototype]
---
# FDM PETG

## Definition
PETG feedstock used in material-extrusion AM for functional prototypes requiring a balance of printability, toughness and resistance to external influences.

## Engineering use
Useful when PLA is too brittle or thermally limited but the project does not require the higher temperature capability, UV performance or process complexity of other engineering polymers.

## Evidence-backed observations
UltiMaker reports HDT about 76 °C for its PETG formulation and strong orientation dependence: tensile stress at break was about 38.5 MPa in XY, 44.0 MPa in YZ and 19.0 MPa in Z under its stated test conditions. These values are formulation/process-specific but strongly support retaining orientation in any engineering property record.

## Decision criteria
Consider PETG for functional housings, manufacturing aids, containers and laboratory prototypes where toughness, moderate temperature capability and chemical/moisture resistance are useful. Do not assume generic chemical compatibility; verify the exact chemical, concentration, temperature, exposure duration and printed-part condition.

## Relationships
| Type | Target | Strength | Reason |
|---|---|---|---|
| MATERIAL_FOR | H2P-PW-021 | Strong | Common FDM feedstock. |
| SELECTED_BY | H2P-PW-176 | Strong | FDM material selection controls use. |
| AFFECTED_BY | H2P-PW-033 | Mandatory | Printed strength is orientation dependent. |
| REQUIRES_CHECK_OF | H2P-PW-180 | Strong | Environmental compatibility cannot be inferred from polymer name alone. |

## Podcast use
Prototype Shop — choosing functional FDM materials.
