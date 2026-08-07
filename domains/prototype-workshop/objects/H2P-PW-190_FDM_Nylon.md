---
id: H2P-PW-190
title: FDM Nylon Family
object_type: Material Family
parent_process: H2P-PW-021
status: Researching
lifecycle: [Prototype, Engineering Prototype]
tags: [FDM, Nylon, PA, polymer-am, functional-prototype]
---
# FDM Nylon Family

## Definition
Polyamide feedstocks used in material extrusion. `Nylon` is a family label, not a single engineering material; PA6, PA66, PA11, PA12 and filled variants can differ substantially.

## Engineering use
Nylon-family materials are useful for tough, wear-resistant, low-friction or fatigue-tolerant prototype parts where brittle/stiff materials are unsuitable.

## Decision criteria
Specify the exact polyamide and formulation. Evaluate moisture conditioning, dimensional stability, wear, temperature, chemical exposure and print-system requirements before selection.

## Key limitations
- Hygroscopic behavior can alter processing and final properties.
- Drying/storage discipline is often more critical than with PLA/PETG.
- Generic `nylon` datasheets are insufficient for design decisions.
- Printed-part properties remain orientation/process dependent.

## Evidence notes
UltiMaker lists its Method-series Nylon at about 66 MPa tensile strength, 91 °C heat deflection and 1.7 GPa flexural modulus under its own process conditions. These data characterize that material/system, not the whole nylon family.

## Relationships
| Type | Target | Strength | Reason |
|---|---|---|---|
| MATERIAL_FOR | H2P-PW-021 | Strong | Polyamide is an engineering FDM feedstock family. |
| REQUIRES | H2P-PW-179 | Mandatory | Moisture management strongly affects feedstock/process quality. |
| SELECTED_BY | H2P-PW-176 | Strong | Exact family/formulation must be selected by application. |
| RELATED_TO | H2P-PW-178 | Strong | PA11/PA12 also appear in polymer PBF and must not be conflated across processes. |

## Podcast use
Prototype Shop — why `nylon` is not a sufficient material specification.
