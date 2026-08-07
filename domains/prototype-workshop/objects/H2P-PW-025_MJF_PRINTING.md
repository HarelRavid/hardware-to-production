# H2P-PW-025 — MJF Printing

```yaml
id: H2P-PW-025
title: MJF Printing
aliases: [Multi Jet Fusion]
object_type: Manufacturing Process
domain: Prototype Workshop
subdomain: Additive Manufacturing — Polymer
lifecycle: [Prototype, Engineering Prototype, EVT, DVT, Low-volume Production]
status: Researching
summary: Polymer powder-bed AM process using selectively jetted agents and thermal energy; strong candidate for functional nylon-family prototypes and densely packed batches, but material/system specificity and post-processing must be preserved in all comparisons.
tags: [MJF, powder-bed, polymer-AM, PA12, rapid-prototyping]
created: 2026-08-07
last_reviewed: 2026-08-07
```

## 1. Definition
MJF is a polymer powder-bed additive process in which agents are selectively jetted onto powder and thermal energy is used to fuse the desired regions.

## 2. Purpose
Produce functional polymer prototypes and small batches with complex geometry, dense nesting and no conventional support structures.

## 3. Problem Solved
Offers a batch-oriented polymer AM route suited to functional parts where FDM support/orientation constraints or SLA resin behavior are undesirable.

## 4. Lifecycle Position
Useful from functional prototyping through DVT and bridge/low-volume production. It can sometimes produce end-use parts, but its representativeness depends on whether MJF is itself the intended production process.

## 5. Typical Owner / Responsible Roles
Prototype engineer, additive manufacturing engineer, manufacturing engineer, qualified external supplier.

## 6. Inputs / Preconditions
CAD; purpose; material family; nesting strategy; supplier/machine capability; dimensional criteria; depowdering/finishing plan; build record.

## 7. Outputs / Deliverables
Printed and depowdered parts; finish condition; process/build traceability; inspection results.

## 8. How It Works
Powder layers are deposited. Fusing/detailing agents define thermal response and boundaries, followed by thermal exposure that fuses selected regions. The surrounding powder supports the parts during the build.

## 9. Decision Criteria
Strong candidate for durable polymer parts, complex unsupported geometry and batches. Compare against SLS on material portfolio, supplier capability, density, dimensional behavior, surface condition, cost, cooling and finishing rather than assuming one is universally superior.

## 10. Alternatives and Tradeoffs
SLS is the closest alternative; SLA is preferred for some high-detail/surface applications; FDM can dominate rapid one-off in-house loops; CNC can dominate precision and stock-material fidelity.

## 11. Limitations / Failure Conditions
Machine/vendor ecosystem dependency; powder and thermal-process variability; granular as-built surface; depowdering constraints; dimensional compensation; enclosed powder; limited direct equivalence to molded thermoplastics.

## 12. Common Mistakes
Treating MJF as simply 'better SLS'; comparing finished supplier samples without separating post-processing; generalizing PA12 behavior to all MJF materials; assuming support-free equals unrestricted geometry; treating batch economics as identical to one-off prototype economics.

## 13. Standards and Regulations
ISO/ASTM 52900 provides the high-level AM process vocabulary. MJF-specific design and qualification guidance is less directly codified than laser PBF/P, so evidence must distinguish general powder-bed principles from vendor/process-specific recommendations.

## 14. Academic Evidence
Published studies show MJF PA12 can support demanding functional geometries, but conclusions remain material-, geometry- and application-specific. Comparative claims versus SLS must therefore be evidence-scoped.

## 15–18. Additional Sources / Case Studies
To be expanded during MJF-specific depth pass.

## 19. Relationships
| Type | Target Object | Strength | Confidence | Reason | Evidence |
|---|---|---|---|---|---|
| SPECIALIZES | H2P-PW-173 Prototype Manufacturing Process Selection | Strong | High | MJF is one option in the common technology-selection framework. | Knowledge architecture |
| REQUIRES | H2P-PW-031 SLS/MJF Design Rules | Strong | High | Powder-bed design constraints apply, with process-specific differences. | Process literature |
| REQUIRES | H2P-PW-033 Additive Orientation Strategy | Strong | High | Build placement affects thermal and feature outcomes. | Process principle |
| REQUIRES | H2P-PW-035 Additive Post-processing | Strong | High | Depowdering and finishing affect delivered part. | Process principle |
| AFFECTS | H2P-PW-036 Additive Prototype Accuracy | Strong | High | Thermal/process compensation influences dimensions. | AM metrology logic |
| AFFECTS | H2P-PW-037 Additive Prototype Surface Finish | Strong | High | Raw MJF surfaces are process-specific and often finished. | Process literature |
| ALTERNATIVE_TO | H2P-PW-024 SLS Polymer Printing | Strong | High | Both are polymer powder-bed approaches with different fusion mechanisms. | Process comparison |
| ALTERNATIVE_TO | H2P-PW-021 FDM / FFF Printing | Medium | High | Both serve functional prototypes but differ strongly in batch behavior and support logic. | Process comparison |

## 20. Open Questions / Evidence Gaps
Need stronger independent SLS-vs-MJF data on dimensional capability, density, isotropy, permeability, feature limits and lifecycle cost, separated by material and finishing condition.

## 21. Podcast Mapping
- Relevant section: Prototype Shop
- Candidate episode(s): Polymer 3D Printing; Powder-Bed Prototyping
- Listener tags: #MJF #PowderBed #PA12 #PrototypeShop
- Prerequisite objects: H2P-PW-002, H2P-PW-173

## 22–23. Future Mapping
Reserved.

## 24. Revision Notes
Initial research-backed object created 2026-08-07.
