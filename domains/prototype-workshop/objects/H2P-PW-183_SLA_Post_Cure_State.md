---
id: H2P-PW-183
title: SLA Post-Cure State
object_type: Process State
domain: Prototype Workshop
subdomain: Polymer Additive Manufacturing
lifecycle: [Prototype, Engineering Prototype, EVT, DVT]
status: Researching
---

# SLA Post-Cure State

## Definition
The defined wash/cure condition of a photopolymer part after printing, treated as part of the material/process specification rather than optional cosmetic finishing.

## Why it matters
Mechanical and thermal properties can change substantially between green and post-cured states. Therefore material data, prototype build records and test reports must record cure conditions.

## Example evidence
Formlabs High Temp Resin data reports UTS 21 MPa in green condition, 58 MPa after a 60 °C cure and 49 MPa after an extended 80 °C + 160 °C cure schedule. HDT @0.45 MPa changes from 49 °C to 120 °C and then 238 °C across those states. Tough-resin data similarly specifies printer, layer thickness and cure schedule alongside properties.

## Minimum build-record fields
- Resin product and lot
- Printer / process version
- Layer setting
- Wash medium and time
- Cure equipment
- Cure temperature
- Cure duration
- Delay between print/cure/test if material is aging-sensitive

## Relationships
| Type | Target Object | Strength | Confidence | Reason | Evidence |
|---|---|---|---|---|---|
| APPLIES_TO | H2P-PW-022 SLA Printing | Mandatory | High | Cure completes material system | Manufacturer TDS |
| REQUIRED_BY | H2P-PW-177 SLA Resin Family Selection | Mandatory | High | Properties are cure-dependent | Manufacturer TDS |
| REQUIRES | H2P-PW-017 Prototype Build Record | Strong | High | Cure state must be traceable | Project governance |
| AFFECTS | H2P-PW-036 Additive Prototype Accuracy | Medium | Medium | Cure can affect final condition/dimensions | AM practice |

## Open gaps
Add independent dimensional-change and aging studies by resin class.