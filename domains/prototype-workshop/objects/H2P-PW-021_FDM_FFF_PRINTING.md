# H2P-PW-021 — FDM / FFF Printing

```yaml
id: H2P-PW-021
title: FDM / FFF Printing
aliases: [Fused Filament Fabrication, Fused Deposition Modeling, Material Extrusion]
object_type: Manufacturing Process
domain: Prototype Workshop
subdomain: Additive Manufacturing — Polymer
lifecycle: [POC, Prototype, Engineering Prototype, EVT]
status: Researching
summary: Material-extrusion additive manufacturing process in which thermoplastic feedstock is deposited layer by layer; highly accessible and fast for iteration, but process-induced anisotropy, thermal history, dimensional variation and surface finish must be treated explicitly.
tags: [FDM, FFF, material-extrusion, polymer-AM, rapid-prototyping]
created: 2026-08-07
last_reviewed: 2026-08-07
```

## 1. Definition
FDM/FFF is the polymer material-extrusion AM process in which thermoplastic feedstock is softened and selectively deposited through a nozzle to create a part layer by layer.

## 2. Purpose
Fast, low-barrier fabrication of concept models, fit-check parts, fixtures, housings and selected functional prototypes without hard tooling.

## 3. Problem Solved
It compresses CAD-to-part lead time and makes repeated physical iteration economical when geometry or design intent is still changing.

## 4. Lifecycle Position
Strongest in POC through EVT. It can support later stages for fixtures, tooling aids and some end-use parts, but it should not automatically be treated as representative of molded or machined production parts.

## 5. Typical Owner / Responsible Roles
Mechanical engineer, prototype engineer, workshop technician, additive manufacturing engineer.

## 6. Inputs / Preconditions
3D CAD; intended prototype purpose; material choice; build orientation; slicing strategy; machine/material compatibility; acceptance criteria.

## 7. Outputs / Deliverables
Printed part; print file/build file; process settings; inspection result; build record; lessons learned.

## 8. How It Works
Filament or other thermoplastic feedstock is driven into a heated extrusion zone and deposited along programmed paths. Thermal bonding between adjacent roads and layers creates the final body. The deposited structure and thermal history make the resulting properties process-specific rather than equivalent to the bulk polymer.

## 9. Decision Criteria
Use when iteration speed, low setup cost and geometric flexibility dominate. Escalate to another process when production-material fidelity, isotropic structural behavior, very fine surface/detail, tight interfaces, thermal performance or production-process representativeness dominate.

## 10. Alternatives and Tradeoffs
SLA/MSLA for finer detail and smooth surfaces; SLS/MJF for support-free powder-bed polymer parts and batch nesting; CNC for production-grade stock material and precise interfaces.

## 11. Limitations / Failure Conditions
Layer-direction sensitivity; poor or variable interlayer bonding; warpage and shrinkage; nozzle/toolpath limitations; visible layer texture; support scars; moisture-sensitive feedstocks; machine- and parameter-specific behavior.

## 12. Common Mistakes
Treating datasheet polymer properties as printed-part properties; ignoring orientation; using cosmetic success as evidence of structural adequacy; assuming nominal CAD dimensions equal finished dimensions; using FDM as proof that an injection-molded geometry is production-ready.

## 13. Standards and Regulations
- ISO/ASTM 52900 — AM terminology and process categories.
- ISO/ASTM 52903-1:2020 — feedstock requirements for material-extrusion plastic AM.
- ISO/ASTM 52903-2:2020 — process-equipment / part-integrity framework for material-extrusion plastic AM.
- ISO/ASTM DIS 52961 — under-development EHS standard for polymer material extrusion; draft status must be preserved when cited.

## 14. Academic Evidence
Published work consistently shows that orientation, infill/toolpath and interlayer bonding affect mechanical response. Thermal gradients and cooling also drive residual stress, shrinkage and warpage.

## 15. Books and Professional Handbooks
To be expanded during source-depth pass.

## 16. Industry Guidance / White Papers
Reserved for machine/material-specific operating windows; vendor values will never be generalized across the entire process family.

## 17. Courses, Lectures and Training Material
MIT rapid-prototyping and design/manufacturing courses provide useful process-selection context.

## 18. Case Studies
To be expanded.

## 19. Relationships
| Type | Target Object | Strength | Confidence | Reason | Evidence |
|---|---|---|---|---|---|
| SPECIALIZES | H2P-PW-173 Prototype Manufacturing Process Selection | Strong | High | FDM is one candidate process inside the common selection framework. | Knowledge architecture |
| REQUIRES | H2P-PW-033 Additive Orientation Strategy | Mandatory | High | Orientation changes geometry, supports, surface and mechanical behavior. | Academic literature |
| AFFECTS | H2P-PW-036 Additive Prototype Accuracy | Strong | High | Thermal and path effects influence dimensional outcome. | NIST AM accuracy work |
| AFFECTS | H2P-PW-037 Additive Prototype Surface Finish | Strong | High | Layered deposition creates process-specific surface texture. | NIST metrology context |
| ALTERNATIVE_TO | H2P-PW-022 SLA Printing | Medium | High | Both serve polymer rapid prototyping but optimize different needs. | Process comparison |
| ALTERNATIVE_TO | H2P-PW-024 SLS Polymer Printing | Medium | High | Both serve polymer prototypes with different support/material/batch behavior. | Process comparison |
| ALTERNATIVE_TO | H2P-PW-049 CNC Milling | Medium | High | CNC may dominate where stock-material fidelity and precision matter. | NIST/MIT process-selection logic |

## 20. Open Questions / Evidence Gaps
Build machine-independent numeric envelopes for accuracy, minimum feature size and mechanical anisotropy without over-generalizing across materials and machines.

## 21. Podcast Mapping
- Relevant section: Prototype Shop
- Candidate episode(s): Polymer 3D Printing; Choosing a Prototype Process
- Listener tags: #FDM #FFF #MaterialExtrusion #PrototypeShop
- Prerequisite objects: H2P-PW-001, H2P-PW-002, H2P-PW-173

## 22. Future Toolkit Mapping
Reserved.

## 23. Future Learning Path Mapping
Reserved.

## 24. Revision Notes
Initial research-backed object created 2026-08-07.
