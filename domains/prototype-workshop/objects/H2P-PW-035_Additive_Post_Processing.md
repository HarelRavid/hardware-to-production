---
id: H2P-PW-035
title: Additive Post-processing
object_type: Process
domain: Prototype Workshop
subdomain: Polymer Additive Manufacturing
lifecycle: [Prototype, Engineering Prototype, EVT, DVT]
status: Researching
---

# Additive Post-processing

## Definition
All operations applied after polymer AM build completion that alter cleanliness, support state, cure, surface, dimensional condition, color, sealing, machinability or functional performance.

## Process-specific operations
### FDM/FFF
- Support removal
- Soluble-support dissolution
- Deburring / trimming
- Sanding / machining
- Vapor smoothing where material-appropriate
- Heat-set inserts / secondary assembly

### SLA/MSLA
- Washing
- Drying
- Support removal
- UV/thermal post-cure
- Sanding / coating / polishing

### SLS/MJF
- Depowdering
- Media blasting
- Tumbling / smoothing
- Dyeing
- Sealing / infiltration where applicable
- Secondary machining

## Core principle
Post-processing is part of the manufacturing route, not an afterthought. Accuracy, surface finish, material properties, labor, lead time and cost should be reported with the post-process state.

Current SLA engineering-material guidance explicitly treats washing and post-curing as required workflow steps. SLS workflows require depowdering and commonly media blasting; powder refresh rate is also a material/process-economic parameter.

## Relationships
| Type | Target Object | Strength | Confidence | Reason | Evidence |
|---|---|---|---|---|---|
| AFFECTS | H2P-PW-037 Additive Prototype Surface Finish | Mandatory | High | Surface state is post-process dependent | Manufacturer guidance |
| AFFECTS | H2P-PW-036 Additive Prototype Accuracy | Strong | High | Secondary operations can alter dimensions | AM practice |
| INCLUDES | H2P-PW-183 SLA Post-Cure State | Strong | High | SLA cure is a critical post-process | TDS |
| CONTRIBUTES_TO | H2P-PW-019 Prototype Cost Tracking | Strong | High | Labor/equipment/material contribute to true cost | Project method |
| CONTRIBUTES_TO | H2P-PW-020 Prototype Lead-time Tracking | Strong | High | Post-processing extends CAD-to-test time | Project method |

## Open gaps
Add process-time benchmarks and automated post-processing options after primary-source validation.