---
id: H2P-PW-184
title: Polymer AM Design Rules
object_type: Method
domain: Prototype Workshop
subdomain: Polymer Additive Manufacturing
lifecycle: [Prototype, Engineering Prototype, EVT]
status: Researching
---

# Polymer AM Design Rules

## Definition
A process-aware set of geometry rules used to design polymer AM prototypes that are printable, measurable and suitable for their intended learning objective.

## Rule families
- Minimum wall thickness
- Minimum feature / pin diameter
- Minimum hole size
- Unsupported spans / overhangs
- Clearance for moving or mating parts
- Escape holes / powder evacuation
- Bosses and fastening features
- Text / embossed or engraved detail
- Thin ribs and high-aspect-ratio features
- Large cross-sections and warpage
- Datum and inspection access
- Orientation-sensitive interfaces

## Core principle
Do not publish one universal number for “3D-print minimum wall thickness” or “AM tolerance.” Design limits are process-, material-, geometry-, orientation-, machine- and post-process dependent.

ISO/ASTM 52910 provides general AM design guidance; ISO/ASTM 52911-2 provides process-specific recommendations for polymer laser PBF. Material-extrusion requirements are further constrained by extrusion width, layer bonding, support strategy and thermal distortion.

## Process distinctions
### FDM/FFF
Rules are strongly coupled to nozzle/extrusion width, bead placement, layer height, orientation, bridging and support strategy.

### SLA/MSLA
Fine detail can be high, but support attachment, drainage, cure state, trapped resin and thin-feature brittleness must be considered.

### SLS/MJF
No attached supports are normally required; powder evacuation, thermal mass, packing/nesting, large cross-sections and feature resolution become dominant.

## Relationships
| Type | Target Object | Strength | Confidence | Reason | Evidence |
|---|---|---|---|---|---|
| DEPENDS_ON | H2P-PW-173 Prototype Manufacturing Process Selection | Strong | High | Design rules follow selected process | ISO 52910 |
| INTERACTS_WITH | H2P-PW-181 Additive Support Strategy | Strong | High | Supports affect allowable geometry | Process guidance |
| INTERACTS_WITH | H2P-PW-033 Additive Orientation Strategy | Strong | High | Orientation changes feature capability | AM literature |
| AFFECTS | H2P-PW-036 Additive Prototype Accuracy | Strong | High | Feature geometry affects achieved accuracy | NIST/AM literature |

## Open gaps
Create machine-class-specific appendices for quantitative ranges; never collapse those appendices into a universal rule table.