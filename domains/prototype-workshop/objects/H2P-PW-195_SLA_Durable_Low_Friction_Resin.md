---
id: H2P-PW-195
title: SLA Durable / Low-Friction Resin Family
object_type: Material Family
parent_process: H2P-PW-022
status: Researching
lifecycle: [Prototype, Engineering Prototype]
tags: [SLA, durable-resin, low-friction, engineering-resin, polymer-am]
---
# SLA Durable / Low-Friction Resin Family

## Definition
Photopolymer formulations optimized for pliability, impact tolerance and lower-friction behavior rather than maximum stiffness or temperature capability.

## Engineering use
Useful for squeezable parts, low-friction assemblies, compliant prototypes, gears/ball-joint concepts and impact-tolerant jigs where standard rigid resin would give misleading results.

## Evidence-backed example
Formlabs Durable Resin V2 reports approximately 28 MPa UTS, 1.0 GPa tensile modulus, 55% elongation at break and HDT 41 °C at 0.45 MPa under its stated conditions. The vendor positions it as PE-like in strength/stiffness with low-friction behavior.

## Decision criteria
Use when compliance and friction behavior matter more than heat resistance or high stiffness. Compare against Tough-family resin when fatigue, ductility and higher environmental stability dominate.

## Relationships
| Type | Target | Strength | Reason |
|---|---|---|---|
| MATERIAL_FOR | H2P-PW-022 | Strong | SLA engineering photopolymer family. |
| SELECTED_BY | H2P-PW-177 | Strong | Resin-family selection controls suitability. |
| REQUIRES | H2P-PW-183 | Mandatory | Post-cure state affects final behavior. |
| ALTERNATIVE_TO | H2P-PW-193 | Strong | Tough-family resins cover a different stiffness/ductility/fatigue trade space. |
| LIMITED_BY | H2P-PW-174 | Strong | Similarity to PE/POM-like behavior is application-specific, not production-process equivalence. |

## Podcast use
Prototype Shop — choosing low-friction and compliant SLA materials.
