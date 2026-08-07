---
id: H2P-PW-009
title: Workshop Capability Matrix
aliases: [Prototype Shop Capability Matrix, Internal Fabrication Capability Matrix]
object_type: Deliverable
domain: Prototype Workshop
subdomain: Strategy & Workshop Architecture
lifecycle: [POC, Prototype, Engineering Prototype, EVT, DVT, Pilot]
status: Researching
summary: A structured inventory of what an internal prototype workshop can actually make, assemble, measure and test, including materials, envelope, tolerance, throughput, safety, training and readiness limits.
tags: [workshop-capability, prototype-shop, equipment, make-buy, metrology, readiness]
created: 2026-08-07
last_reviewed: 2026-08-07
---

# Workshop Capability Matrix

## 1. Definition
The Workshop Capability Matrix is the authoritative map of internal prototype-shop capability. It converts a list of machines into engineering decision data: what can be fabricated, assembled, measured or tested; with which materials; at what practical envelope, accuracy, turnaround, readiness and constraints.

## 2. Purpose
- Make in-house capability visible to development teams.
- Support prototype make/buy decisions.
- Prevent misuse of equipment beyond demonstrated process capability.
- Identify bottlenecks, training gaps and CAPEX priorities.
- Match prototype questions to the fastest adequate fabrication route.

## 3. Problem Solved
A workshop equipment list does not answer whether the organization can reliably produce a specific prototype. Capability depends on machine, tooling, software, operator competence, materials, inspection, utilities, safety controls, queue and demonstrated results.

## 4. Lifecycle Position
Established as soon as an internal workshop exists and continuously maintained. Early development uses it to maximize iteration speed; EVT/DVT use it to distinguish development-grade capability from production-representative capability; Pilot may use the same matrix to identify which prototype resources remain useful for production support.

## 5. Typical Owner / Responsible Roles
Prototype Workshop Lead / Manufacturing Engineering, with input from machine owners, metrology, EHS and development engineering.

## 6. Inputs / Preconditions
- Equipment inventory.
- Tooling and workholding inventory.
- Materials/process compatibility.
- Demonstrated tolerances and quality limits.
- Operator/training status.
- Maintenance/calibration state.
- Utility/EHS constraints.
- Queue and typical turnaround data.

## 7. Outputs / Deliverables
A living matrix with fields such as:
- Capability/process.
- Machine/equipment.
- Materials.
- Work envelope.
- Typical and demonstrated tolerance.
- Surface/feature limitations.
- Minimum practical feature size.
- Setup requirements.
- Post-processing.
- Inspection capability.
- Trained users.
- Safety controls.
- Typical CAD-to-part lead time.
- Capacity/utilization.
- Readiness/status.
- Outsource fallback.

## 8. How It Works
The matrix should be capability-centric, not equipment-centric. For example, "FDM functional polymer prototype" is more useful to an engineer than simply listing a printer model. Each capability should point to the equipment, trained people and measurement route that make the capability real.

NASA Ames provides an institutional example of integrated machining, instrumentation, rapid prototyping, fabrication and engineering evaluation. MIT's CCTR Device Workshop similarly combines 3D printing, laser cutting, hand/bench tools, electronics and training specifically to support rapid device development and modifications. SLAC's APF combines precision machining, joining, vacuum processes, metrology and electrical testing as an integrated rapid-prototyping capability.

## 9. Decision Criteria
A capability should be marked "available" only when the full chain is usable: design data -> preparation/CAM -> machine/tooling -> competent operator -> safe process -> post-process -> measurement/test. Capability is not proven by equipment ownership alone.

## 10. Alternatives and Tradeoffs
- Simple equipment list: easy to maintain but poor for engineering decisions.
- Supplier database: complementary for external capability.
- Machine-by-machine SOP system: deeper operational detail but not sufficient as a capability-selection map.

## 11. Limitations / Failure Conditions
- Marketing specification used as demonstrated process capability.
- No distinction between theoretical and proven tolerance.
- Ignoring queue/setup/post-process time.
- No owner or review cadence.
- Missing metrology/test route.
- Capability remains listed despite broken equipment, expired calibration or no trained operator.

## 12. Common Mistakes
- Buying machines before defining missing capabilities.
- Overly specific matrix tied to one machine model rather than transferable process capability.
- No indication of material/process safety restrictions.
- No outsource fallback for overload or out-of-envelope work.

## 13. Standards and Regulations
Process-specific standards and EHS requirements apply. Additive manufacturing vocabulary should use current ISO/ASTM terminology where applicable; ISO/ASTM 52900:2021 is the current foundational AM vocabulary standard.

## 14. Academic Evidence
The prototyping literature supports selecting prototype embodiment based on scale, system level, fidelity and media; the capability matrix is an operational mechanism for mapping those needs to available fabrication methods.

## 15. Books and Professional Handbooks
Gap to fill: facilities planning, manufacturing-process selection, prototyping and metrology references for standardized capability descriptors.

## 16. Industry Guidance / White Papers
- NASA Ames Applied Manufacturing and Engineering Test Division.
- NIST MEP Additive Manufacturing/3D Printing.
- NIST pre-purchase equipment guide for lifecycle/equipment decision factors.

## 17. Courses, Lectures and Training Material
- MIT makerspace resources and MIT CCTR Device Workshop.
- MIT OCW 16.810, which integrates CAD/CAE/CAM, machining and testing.

## 18. Case Studies
- NASA Ames: broad integrated fabrication/testing capability supporting researchers and engineers from concept through finished hardware.
- MIT CCTR: prototype-focused device workshop for rapid builds, repairs and modifications with equipment-specific training.
- SLAC APF: integrated precision manufacturing/metrology facility supporting concept-to-proof-of-design cycles.

## 19. Relationships
| Type | Target Object | Strength | Confidence | Reason | Evidence |
|---|---|---|---|---|---|
| ENABLES | H2P-PW-001 Prototype Strategy | Medium | High | Strategy can select only from known internal/external capabilities. | Camburn + synthesis |
| ENABLES | H2P-PW-004 Rapid Iteration Loop | Strong | High | Local capability removes procurement/queue latency for many iterations. | NASA Ames; MIT CCTR |
| REQUIRED_BY | H2P-PW-008 Prototype Make vs Buy | Strong | High | Sourcing decisions require a realistic baseline of internal capability. | Project synthesis |
| INFORMS | H2P-PW-165 Equipment Purchase Decision | Strong | High | Matrix gaps expose where equipment may add capability. | NIST pre-purchase guidance |
| INFORMS | H2P-PW-166 Workshop CAPEX Prioritization | Strong | High | Missing/high-demand capabilities become investment candidates. | Project synthesis |
| MEASURED_BY | H2P-PW-170 Internal Capability Readiness | Strong | High | Readiness indicates whether a nominal capability is truly executable. | Project model |
| CONSTRAINED_BY | H2P-PW-150 Workshop Capacity | Medium | High | Capability may exist but be unavailable due to capacity. | Project model |
| CONSTRAINED_BY | H2P-PW-139 Workshop Training Matrix | Strong | High | Capability depends on trained users. | MIT CCTR training model |
| CONSTRAINED_BY | H2P-PW-141 Calibration Program | Medium | High | Measurement-dependent capability requires valid calibration. | Engineering synthesis |

## 20. Open Questions / Evidence Gaps
- Define standard fields by process family (AM, machining, electronics, test).
- Define maturity grades: Installed, Commissioned, Demonstrated, Controlled, Production-support capable.
- Determine best method for representing confidence intervals around real workshop tolerances.

## 21. Podcast Mapping
- Relevant section: The Prototype Shop
- Candidate episode(s): How to Build a Prototype Workshop; Which Machines Do You Actually Need?; Prototype Shop at $10k/$50k/$100k/$500k
- Listener tags: #WorkshopCapability #PrototypeShop #MakeVsBuy #WorkshopROI
- Prerequisite objects: none

## 22. Future Toolkit Mapping
Reserved.

## 23. Future Learning Path Mapping
Reserved.

## 24. Revision Notes
v0.1 — Initial architecture based on NASA Ames, MIT CCTR, SLAC APF and NIST manufacturing guidance.