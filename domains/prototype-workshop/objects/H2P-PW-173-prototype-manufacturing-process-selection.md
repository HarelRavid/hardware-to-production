---
id: H2P-PW-173
title: Prototype Manufacturing Process Selection
aliases: [Prototype Process Selection, Rapid Prototyping Process Selection]
object_type: Method
domain: Prototype Workshop
subdomain: Capability & Technology Selection
lifecycle: [POC, Prototype, Engineering Prototype, EVT, DVT]
status: Researching
summary: Structured selection of a prototype manufacturing process based on purpose, fidelity, material, geometry, loading, accuracy, lead time, cost, quantity, in-house capability, and production representativeness.
tags: [PrototypeStrategy, ProcessSelection, RapidPrototyping, MakeBuy, Manufacturing]
created: 2026-08-07
last_reviewed: 2026-08-07
---

# Prototype Manufacturing Process Selection

## 1. Definition
Prototype manufacturing process selection is the structured choice of the fabrication route used to build a prototype or prototype batch. It is not equivalent to choosing the fastest available machine. The selected route should be the lowest-cost and lowest-latency route that can answer the intended engineering question with sufficient fidelity.

## 2. Purpose
To avoid overbuilding or underbuilding prototypes, reduce learning latency, prevent misleading test results, and make deliberate tradeoffs between speed, cost, accuracy, material behavior and production representativeness.

## 3. Problem Solved
Prototype teams often choose processes by convenience: "print it because the printer is available" or "machine it because that is what the supplier does." This can create false confidence, unnecessary cost, long lead times or test data that does not represent the intended product.

## 4. Lifecycle Position
- Concept/POC: prioritize speed and learning; low fidelity may be appropriate.
- Prototype: optimize for geometry, fit, ergonomics and architecture learning.
- Engineering Prototype / EVT: increase functional and material fidelity.
- DVT: process and material representativeness become more important.
- PVT onward: this object hands off to production process selection and DFM rather than prototype-only process selection.

## 5. Typical Owner / Responsible Roles
Mechanical Engineer, Hardware Engineer, Prototype Engineer, NPI Engineer, Manufacturing Engineer, Workshop Manager.

## 6. Inputs / Preconditions
- Prototype purpose classification.
- Required fidelity.
- CAD / geometry maturity.
- Target material or required material properties.
- Functional loads and environmental conditions.
- Critical dimensions and surface requirements.
- Required quantity.
- Deadline / learning latency target.
- Internal capability matrix.
- Supplier capability and lead time.

## 7. Outputs / Deliverables
- Selected process.
- Selected material.
- In-house vs outsource route.
- Expected fidelity and known deviations from production intent.
- Cost and lead-time estimate.
- Inspection/test requirements.
- Explicit statement of what the prototype can and cannot prove.

## 8. Decision Framework
A prototype process should be compared using one common criterion set:

1. Purpose — what question must the prototype answer?
2. Fidelity — geometric, visual, functional, material, interface and process fidelity.
3. Material behavior — does the selected material reproduce the needed stiffness, thermal behavior, friction, sealing, electrical or environmental behavior?
4. Geometry — size, wall thickness, cavities, undercuts, unsupported features, reach/access and feature density.
5. Functional loading — static, dynamic, thermal, pressure, fatigue, sealing or wear loads.
6. Accuracy and repeatability — dimensions, datum relationships and repeatability across multiple builds.
7. Surface condition — roughness, appearance, friction, sealing and post-processing needs.
8. Lead time — CAD-to-part and total feedback latency.
9. Cost — direct part cost plus setup, tooling, post-processing, inspection and engineering labor.
10. Quantity — one-off, small batch, bridge batch or pilot quantity.
11. Production representativeness — whether the process, material, assembly interfaces and resulting variation are representative of the intended production process.
12. Capability availability — internal equipment, skills, safety, metrology and supplier availability.

## 9. Process-Family Heuristics
### Polymer additive manufacturing
Strong when geometry is complex, tooling must be avoided, quantities are low and rapid iteration is valuable. NIST notes that additive manufacturing can bypass tooling lead time and improve economics for low-volume production.

### CNC machining
Strong when material properties, dimensional fidelity, machined surfaces or functional metallic/polymer prototypes are important. NIST has documented high-speed CNC machining as a viable rapid-prototyping route for functional metallic prototypes with competitive process times.

### Sheet-metal fabrication
Strong when the production product will itself be sheet metal and bend geometry, fastener locations, stackups and assembly access must be evaluated. It may provide better production representativeness than a printed surrogate enclosure.

### Laser / waterjet cutting
Strong for rapid 2D profiles, plates, brackets, gaskets, fixtures and early sheet-based concepts, especially when secondary bending or joining is simple.

### Production-intent / soft tooling
Strong when the question is no longer only geometry or function but production-process behavior, molded features, material response or part-to-part variation.

## 10. Alternatives and Tradeoffs
The correct selection may be a hybrid build: for example, CNC critical interfaces plus printed noncritical geometry; laser-cut plates plus printed spacers; or production-intent molded parts only for the subassembly where process fidelity matters.

## 11. Limitations / Failure Conditions
- A visually accurate prototype may be mechanically misleading.
- A material-equivalent CNC prototype may not reproduce molded anisotropy, knit lines, draft, shrinkage or process variation.
- Additive prototypes can introduce process-specific anisotropy and surface behavior.
- Production-intent tooling can be too slow and expensive for questions that could be answered by lower fidelity.

## 12. Common Mistakes
- Selecting the process before defining the prototype purpose.
- Treating "high fidelity" as a single variable.
- Using production-intent processes too early.
- Testing strength or sealing on nonrepresentative materials without stating the limitation.
- Ignoring inspection and metrology when choosing the process.
- Ignoring workshop/supplier queue time and focusing only on machine cycle time.

## 13. Standards and Regulations
- ISO/ASTM 52900:2021 — AM terminology.
- ISO/ASTM 52910:2018 — general AM design requirements, guidelines and recommendations.
- ISO/ASTM 52911 series — process-specific AM design guidance for powder-bed-fusion processes.

## 14. Academic Evidence
Manufacturing-process-selection literature treats process choice as a multi-constraint problem driven by material, geometry, capability, quality and economics rather than by a single factor. Prototype-strategy literature similarly emphasizes choosing technique and fidelity according to the question being answered.

## 15. Books and Professional Handbooks
Candidate anchors for later deep review: Ashby-style process selection methods; Bralla DFM handbook; Boothroyd/Dewhurst/Knight; Groover manufacturing-process texts.

## 16. Industry / Government Guidance
- NIST MEP: Additive Manufacturing/3D Printing.
- NIST: The Application of High-Speed CNC Machining to Prototype Production.
- Manufacturing.gov: Rapid Prototyping and Additive Manufacturing definitions.
- MIT 2.008 Design and Manufacturing II integrates process, cost, quality and flexibility and exposes students to sheet metal, machining, molding and AM.

## 17. Relationships
| Type | Target Object | Strength | Confidence | Reason | Evidence |
|---|---|---|---|---|---|
| REQUIRES | H2P-PW-003 Prototype Purpose Classification | Mandatory | High | Process choice must follow the engineering question. | Camburn et al. |
| REQUIRES | H2P-PW-002 Prototype Fidelity | Mandatory | Required fidelity constrains viable process families. | Camburn et al. |
| USES | H2P-PW-009 Workshop Capability Matrix | Strong | Available capability affects feasible in-house routes. | Project synthesis; NASA/MIT facility models |
| INFORMS | H2P-PW-007 In-house vs Outsource Decision | Strong | Process availability and requirements feed sourcing. | Project synthesis |
| INFORMS | H2P-PW-008 Prototype Make vs Buy | Strong | Cost, lead time and capability are common inputs. | Make/buy literature |
| SELECTS_FROM | H2P-PW-021 FDM / FFF Printing | Medium | One candidate process family. | NIST/Manufacturing.gov |
| SELECTS_FROM | H2P-PW-022 SLA Printing | Medium | One candidate process family. | AM literature |
| SELECTS_FROM | H2P-PW-024 SLS Polymer Printing | Medium | One candidate process family. | ISO/ASTM 52911-2 |
| SELECTS_FROM | H2P-PW-025 MJF Printing | Medium | One candidate process family. | AM literature |
| SELECTS_FROM | H2P-PW-049 CNC Milling | Medium | Functional precision prototype route. | NIST CNC paper |
| SELECTS_FROM | H2P-PW-050 CNC Turning | Medium | Rotational functional prototype route. | Manufacturing-process literature |
| SELECTS_FROM | H2P-PW-068 CO2 Laser Cutting | Medium | Rapid 2D route for suitable materials. | MIT manufacturing curriculum |
| SELECTS_FROM | H2P-PW-069 Fiber Laser Cutting | Medium | Rapid sheet-metal cutting route. | Manufacturing-process literature |
| SELECTS_FROM | H2P-PW-070 Waterjet Cutting | Medium | Rapid 2D cutting without a laser heat-affected zone. | Manufacturing-process literature |
| SELECTS_FROM | H2P-PW-072 Sheet Metal Bending | Medium | Production-representative route for sheet products. | MIT 2.008 |
| PRECEDES | H2P-PW-006 Prototype Build Planning | Strong | Selected process becomes a build-plan constraint. | Project synthesis |

## 18. Open Questions / Evidence Gaps
- Quantitative selection thresholds for accuracy, batch size and lead time across process families vary strongly by equipment and supplier.
- A later object should formalize Production Representativeness as a separate dimension.
- Process-specific environmental and safety constraints need to be linked from workshop governance objects.

## 19. Podcast Mapping
Relevant section: The Prototype Shop.
Candidate episode: Choosing How to Build the Prototype.
Listener tags: #ProcessSelection #PrototypeFidelity #RapidPrototyping #CNC #3DPrinting #SheetMetal

## 20. Revision Notes
v0.1 — Created as the central technology-selection node for Prototype Workshop research wave 02.
