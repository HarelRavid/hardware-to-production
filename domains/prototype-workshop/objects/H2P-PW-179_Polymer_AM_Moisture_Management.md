---
id: H2P-PW-179
title: Polymer AM Moisture Management
object_type: Process
domain: Prototype Workshop
subdomain: Polymer Additive Manufacturing
lifecycle: [Prototype, Engineering Prototype, EVT, DVT]
status: Researching
---

# Polymer AM Moisture Management

## Definition
Control of feedstock and printed-part moisture condition when hygroscopic behavior can affect processing, dimensional stability or mechanical properties.

## Why it matters
Polymer families differ strongly in moisture sensitivity. Nylon is a major example: feedstock condition can influence processing, and the condition of the printed part can influence measured properties. Therefore “dry” versus “conditioned” state should be captured whenever relevant.

## Practical controls
- Sealed storage and desiccation
- Drying procedures appropriate to the exact material
- Humidity exposure tracking where relevant
- Recording feedstock lot and condition in build records
- Conditioning test coupons and parts consistently before comparison
- Avoiding cross-comparison of dry and conditioned property values

## PBF note
Commercial PA12 datasets often distinguish orientation and conditioning. Current EOS PA2200 data explicitly reports dry/conditioned columns, reinforcing the need to track condition as part of the evidence metadata.

## Relationships
| Type | Target Object | Strength | Confidence | Reason | Evidence |
|---|---|---|---|---|---|
| AFFECTS | H2P-PW-176 FDM / FFF Material Selection | Strong | High | Hygroscopic feedstocks require condition control | Material practice |
| AFFECTS | H2P-PW-178 Polymer PBF Material Selection | Strong | High | Powder/part condition affects interpretation of properties | EOS data |
| REQUIRES | H2P-PW-017 Prototype Build Record | Strong | High | Material condition should be recorded for reproducibility | Project governance |

## Open gaps
Add polymer-specific equilibrium moisture, drying and conditioning standards without turning this entry into a generic plastics handbook.