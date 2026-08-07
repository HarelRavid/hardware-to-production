# H2P-PW-024 — SLS Polymer Printing

```yaml
id: H2P-PW-024
title: SLS Polymer Printing
aliases: [Selective Laser Sintering, Laser-based Powder Bed Fusion of Polymers, LB-PBF/P]
object_type: Manufacturing Process
domain: Prototype Workshop
subdomain: Additive Manufacturing — Polymer
lifecycle: [Prototype, Engineering Prototype, EVT, DVT, Low-volume Production]
status: Researching
summary: Laser-based powder bed fusion of polymers; valuable for support-free complex geometries and nested batch builds, with process-specific design rules, powder behavior, thermal history, shrinkage and surface texture.
tags: [SLS, polymer-PBF, powder-bed-fusion, PA12, rapid-prototyping]
created: 2026-08-07
last_reviewed: 2026-08-07
```

## 1. Definition
SLS polymer printing is laser-based powder bed fusion of polymer feedstock. A laser selectively fuses regions of a thermoplastic powder layer while the surrounding unfused powder supports the geometry.

## 2. Purpose
Create complex, functional polymer prototypes and small batches without dedicated support structures or hard tooling.

## 3. Problem Solved
Enables geometries, assemblies, channels and densely nested batches that are difficult to produce efficiently with support-dependent AM processes.

## 4. Lifecycle Position
Most useful from functional prototype through DVT and bridge/low-volume production when powder-bed material and process are acceptable. Production representativeness must still be assessed against the intended mass-production route.

## 5. Typical Owner / Responsible Roles
Prototype engineer, additive manufacturing engineer, external AM supplier, manufacturing engineer.

## 6. Inputs / Preconditions
CAD model; material/powder system; packing/nesting strategy; thermal/process recipe; design rules; depowdering and finishing plan; dimensional acceptance criteria.

## 7. Outputs / Deliverables
Fused polymer part; build record; powder/batch traceability where relevant; depowdered/finished part; inspection result.

## 8. How It Works
Powder is spread into a bed, thermally conditioned and selectively fused by laser energy. The powder cake supports surrounding geometry during the build. Cooling and depowdering are integral parts of the workflow and can affect dimensional stability and cycle time.

## 9. Decision Criteria
Prefer for complex unsupported geometries, nested batches, durable polymer prototypes and moving/interlocking features where support removal would be problematic. Evaluate carefully for very smooth cosmetic surfaces, tight sealing, precision bores and features near process limits.

## 10. Alternatives and Tradeoffs
MJF offers a related powder-bed route using agents and thermal energy rather than laser tracing; SLA may outperform on very fine visual detail; CNC may outperform on precision stock-material interfaces; FDM may be more economical for immediate one-off in-house iteration.

## 11. Limitations / Failure Conditions
Powder aging/reuse effects; thermal distortion/shrinkage; rough/granular as-built surface; depowdering of enclosed cavities; minimum feature limitations; long cooling cycles; dimensional compensation; process-dependent porosity and density.

## 12. Common Mistakes
Calling SLS 'support free' and then ignoring trapped powder; assuming arbitrary minimum wall/clearance values across all systems; treating PA12 data as universal SLS data; ignoring cooling and powder-refresh strategy; using an SLS prototype as proof of injection-molding behavior.

## 13. Standards and Regulations
- ISO/ASTM 52900 — terminology and process classification.
- ISO/ASTM 52910 — general AM design requirements/guidance.
- ISO/ASTM 52911-2:2019 — detailed design recommendations for laser-based PBF of polymers; confirmed current in 2026.

## 14. Academic / Government Evidence
NIST identifies polymer AM measurement gaps in FDM, SLA and SLS, emphasizing dimensional, process and material characterization. NIST part-qualification work also cautions that AM geometry, surfaces and internal structures challenge conventional dimensional metrology.

## 15–18. Additional Sources / Case Studies
To be expanded during SLS-specific depth pass.

## 19. Relationships
| Type | Target Object | Strength | Confidence | Reason | Evidence |
|---|---|---|---|---|---|
| SPECIALIZES | H2P-PW-173 Prototype Manufacturing Process Selection | Strong | High | SLS is a selectable process inside the common decision framework. | Knowledge architecture |
| DEFINED_BY | ISO/ASTM 52911-2:2019 | Strong | High | Standard gives process-specific PBF/P design guidance. | ISO |
| REQUIRES | H2P-PW-031 SLS/MJF Design Rules | Mandatory | High | Powder-bed geometry has dedicated process rules. | ISO/ASTM 52911-2 |
| REQUIRES | H2P-PW-033 Additive Orientation Strategy | Strong | High | Orientation/nesting influence thermal behavior, feature outcome and packing. | Process literature |
| REQUIRES | H2P-PW-035 Additive Post-processing | Strong | High | Cooling, depowdering and finishing are part of delivered-part quality. | Process principle |
| AFFECTS | H2P-PW-036 Additive Prototype Accuracy | Strong | High | Shrinkage, thermal history and feature geometry affect dimensions. | NIST metrology work |
| AFFECTS | H2P-PW-037 Additive Prototype Surface Finish | Strong | High | Powder-bed surfaces are process-specific. | NIST metrology context |
| ALTERNATIVE_TO | H2P-PW-025 MJF Printing | Strong | High | Both are polymer powder-bed routes with different fusion mechanisms. | Process comparison |
| ALTERNATIVE_TO | H2P-PW-021 FDM / FFF Printing | Medium | High | Both can serve functional polymer prototyping with different batch/support economics. | Process comparison |

## 20. Open Questions / Evidence Gaps
Quantify machine-independent envelopes for shrinkage, density, surface, powder reuse and feature limits by material family; separate raw-process capability from supplier finishing effects.

## 21. Podcast Mapping
- Relevant section: Prototype Shop
- Candidate episode(s): Polymer 3D Printing; Powder-Bed Prototyping
- Listener tags: #SLS #PBF #PA12 #PrototypeShop
- Prerequisite objects: H2P-PW-002, H2P-PW-173

## 22–23. Future Mapping
Reserved.

## 24. Revision Notes
Initial research-backed object created 2026-08-07.
