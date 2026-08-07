---
id: H2P-PW-189
title: FDM ASA
object_type: Material
parent_process: H2P-PW-021
status: Researching
lifecycle: [Prototype, Engineering Prototype]
tags: [FDM, ASA, polymer-am, outdoor-prototype]
---
# FDM ASA

## Definition
Acrylonitrile-styrene-acrylate feedstock used in material extrusion, typically considered when outdoor exposure and UV/weathering resistance matter.

## Engineering use
ASA is often a better prototype choice than ABS when the prototype must experience sunlight or outdoor weathering while retaining similar engineering-thermoplastic behavior.

## Decision criteria
Consider ASA for exterior housings, brackets, fixtures and field prototypes exposed to UV/weather. Use ABS when outdoor durability is not required and the existing process is already qualified for ABS. Verify exact vendor formulation and print conditions before using quantitative mechanical or thermal values.

## Evidence notes
UltiMaker lists its Method-series ASA at about 49 MPa tensile strength, 96 °C heat deflection and 2.3 GPa flexural modulus under its specified conditions. Values are formulation- and process-specific.

## Relationships
| Type | Target | Strength | Reason |
|---|---|---|---|
| MATERIAL_FOR | H2P-PW-021 | Strong | Engineering FDM feedstock. |
| ALTERNATIVE_TO | H2P-PW-188 | Strong | Often considered instead of ABS for outdoor use. |
| REQUIRES_CHECK_OF | H2P-PW-180 | Strong | UV/weathering and environmental compatibility must be validated. |
| AFFECTED_BY | H2P-PW-033 | Strong | Orientation changes printed-part response. |

## Podcast use
Prototype Shop — material choice for field and outdoor prototypes.
