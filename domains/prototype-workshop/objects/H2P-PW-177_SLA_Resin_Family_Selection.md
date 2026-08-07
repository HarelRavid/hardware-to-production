---
id: H2P-PW-177
title: SLA Resin Family Selection
object_type: Method
domain: Prototype Workshop
subdomain: Polymer Additive Manufacturing
lifecycle: [POC, Prototype, Engineering Prototype, EVT]
status: Researching
---

# SLA Resin Family Selection

## Definition
A method for choosing photopolymer resin families according to required stiffness, toughness, flexibility, thermal performance, surface/detail needs and post-cure behavior.

## Key principle
The label “SLA resin” is not a useful engineering material specification. Resin families span brittle high-detail materials, tough/ductile formulations, flexible/elastomeric grades, heat-resistant formulations, filled rigid materials and application-specific biocompatible grades.

## Selection dimensions
- Dimensional/detail fidelity
- Surface appearance
- Tensile modulus / strength
- Elongation and impact behavior
- HDT and thermal cycling
- Creep and long-term stability
- UV / environmental aging
- Chemical compatibility
- Required post-cure protocol
- Biocompatibility / compliance needs

## Evidence examples
Formlabs High Temp Resin demonstrates why post-cure state is part of the material definition: published HDT @0.45 MPa rises from 49 °C in green condition to 120 °C after one cure schedule and 238 °C after an extended high-temperature cure schedule. Tough 1000 is positioned around HDPE-like stiffness with published elongation at break of 180%, while Tough 1500 targets PP-like compliance and toughness.

These examples are system-specific and must not be treated as universal SLA properties.

## Relationships
| Type | Target Object | Strength | Confidence | Reason | Evidence |
|---|---|---|---|---|---|
| APPLIES_TO | H2P-PW-022 SLA Printing | Mandatory | High | Resin family defines functional capability | Manufacturer TDS |
| DEPENDS_ON | H2P-PW-003 Prototype Purpose Classification | Strong | High | Appearance and functional prototypes need different materials | Project method |
| REQUIRES | H2P-PW-183 SLA Post-Cure State | Mandatory | High | Final properties depend on cure state | Formlabs TDS |
| ALTERNATIVE_TO | H2P-PW-176 FDM / FFF Material Selection | Medium | High | Both solve polymer prototype material selection via different processes | Process-selection model |

## Open gaps
Add independent aging, creep and chemical-resistance evidence; separate manufacturer marketing equivalence claims from directly measured standardized test data.