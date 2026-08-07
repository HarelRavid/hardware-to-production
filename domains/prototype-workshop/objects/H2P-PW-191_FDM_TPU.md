---
id: H2P-PW-191
title: FDM TPU Family
object_type: Material Family
parent_process: H2P-PW-021
status: Researching
lifecycle: [Prototype, Engineering Prototype]
tags: [FDM, TPU, elastomer, polymer-am]
---
# FDM TPU Family

## Definition
Thermoplastic polyurethane feedstocks used in material extrusion for flexible, compliant and energy-absorbing prototype parts.

## Engineering use
Useful for seals/gaskets used for geometric or assembly learning, bumpers, grips, flexible covers, compliant elements and soft-contact fixtures.

## Decision criteria
Select by exact hardness grade, elongation/fatigue requirement, friction, chemical/environmental exposure and printer feed-system capability. A generic `TPU` label is insufficient because Shore hardness and formulation strongly affect behavior.

## Limitations
- Flexible feedstock can reduce print speed and dimensional consistency.
- Printed TPU should not automatically be treated as equivalent to molded elastomer performance.
- Sealing prototypes require explicit validation of surface, porosity, compression set and media compatibility.

## Relationships
| Type | Target | Strength | Reason |
|---|---|---|---|
| MATERIAL_FOR | H2P-PW-021 | Strong | Flexible FDM feedstock family. |
| SELECTED_BY | H2P-PW-176 | Strong | Hardness/application determine suitability. |
| REQUIRES_CHECK_OF | H2P-PW-180 | Strong | Chemical/environmental compatibility is application-specific. |
| LIMITED_BY | H2P-PW-174 | Strong | Printed flexible prototype may poorly represent molded elastomer process behavior. |

## Podcast use
Prototype Shop — flexible and compliant prototypes.
