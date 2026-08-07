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
Polymer families differ strongly in moisture sensitivity. Polyamides are a major example: feedstock condition can influence extrusion/process stability, and printed-part moisture condition can influence measured properties. Therefore "dry", "as printed" and "conditioned" states should not be silently mixed.

## Practical controls
- Store hygroscopic feedstock in sealed/dry conditions appropriate to the exact supplier specification.
- Use drying procedures specified for the exact material rather than a generic "nylon drying" recipe.
- Record material grade, lot, storage condition and drying/conditioning state in the build record when functional data will be compared.
- Condition test coupons and parts consistently before comparative mechanical or dimensional testing.
- Do not compare dry and conditioned material values as though they represent the same state.
- Where a supplier intentionally modifies a polyamide for reduced moisture uptake, treat that as a formulation-specific characteristic rather than a universal nylon property.

## Evidence examples
UltiMaker's current S-series Nylon is a PA6/66-based grade explicitly marketed as having reduced humidity absorption compared with other nylon filaments. This is useful evidence that moisture behavior is formulation-specific even inside the broad "nylon" family.

## PBF note
Commercial PA12 datasets may distinguish dry/conditioned values or provide explicit conditioning context. This reinforces the need to preserve condition metadata alongside property data.

## Relationships
| Type | Target Object | Strength | Confidence | Reason | Evidence |
|---|---|---|---|---|---|
| AFFECTS | H2P-PW-176 FDM / FFF Material Selection | Strong | High | Hygroscopic feedstocks require condition control | Material practice |
| AFFECTS | H2P-PW-178 Polymer PBF Material Selection | Strong | High | Powder/part condition affects interpretation of properties | Material datasets |
| REQUIRES | H2P-PW-017 Prototype Build Record | Strong | High | Material condition should be recorded for reproducibility | Project governance |
| AFFECTS | H2P-PW-036 Additive Prototype Accuracy | Medium | High | Moisture state can change dimensions and process consistency | Polymer behavior |

## Engineering rule
If moisture state is capable of changing the property being tested, moisture/conditioning state becomes part of the test configuration.

## Open gaps
Add polymer-specific equilibrium moisture, drying and conditioning standards for PA11/PA12/PA6-family materials without turning this entry into a generic plastics handbook.