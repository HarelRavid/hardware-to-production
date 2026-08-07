---
id: H2P-PW-001
title: Prototype Strategy
aliases: [Strategic Prototyping]
object_type: Method
domain: Prototype Workshop
subdomain: Strategy & Workshop Architecture
lifecycle: [Concept, POC, Prototype, Engineering Prototype, EVT, DVT]
status: Researching
summary: A deliberate plan for what to prototype, why, at what fidelity and system level, using which medium, and how many iterations or parallel concepts to build in order to reduce uncertainty efficiently.
tags: [prototype-strategy, rapid-prototyping, iteration, fidelity, risk-reduction]
created: 2026-08-07
last_reviewed: 2026-08-07
---

# Prototype Strategy

## 1. Definition
Prototype Strategy is the planned selection and sequencing of prototype activities used to answer specific engineering, user, manufacturing, or business questions with the minimum appropriate expenditure of time, cost, and design commitment.

A prototype should therefore be treated as an experiment with an explicit learning objective, not merely as a more complete version of the product.

## 2. Purpose
- Reduce uncertainty before expensive design commitments are made.
- Expose technical, interface, usability, manufacturability, and integration risks.
- Accelerate learning through deliberate build-test-learn cycles.
- Prevent overbuilding high-fidelity prototypes when a focused prototype can answer the question faster.
- Determine when physical fabrication, analytical simulation, subsystem rigs, or comprehensive builds are appropriate.

## 3. Problem Solved
Hardware teams frequently spend significant time and money producing prototypes that are too complete, too expensive, too slow, or incapable of answering the actual design question. Strategic prototyping aligns the prototype embodiment with the uncertainty being reduced.

## 4. Lifecycle Position
Prototype strategy starts during Concept/POC and remains important through EVT and DVT. Its character changes over time:
- Concept/POC: explore principles and feasibility.
- Prototype: compare architectures and interfaces.
- Engineering Prototype: increase functional and dimensional fidelity.
- EVT: verify design requirements and major risks.
- DVT: increasingly representative builds for qualification, reliability, usability and compliance.

PVT/Pilot prototyping shifts toward manufacturing-process and tooling validation and is covered primarily by NPI objects.

## 5. Typical Owner / Responsible Roles
Hardware/Mechanical/Electrical Engineering, Systems Engineering, Product Development, Prototype Engineering; NPI and Manufacturing Engineering increasingly participate as maturity increases.

## 6. Inputs / Preconditions
- Design questions or uncertainties.
- Requirements and constraints appropriate to the maturity level.
- Risk register or known unknowns.
- Available workshop/supplier capabilities.
- Time and budget constraints.

## 7. Outputs / Deliverables
- Prototype objective and hypothesis.
- Selected fidelity, scale, system level and medium.
- Build/test plan.
- Pass/fail or learning criteria.
- Captured evidence and decisions.
- Updated design risks and next prototype action.

## 8. How It Works
A useful strategic sequence is:
1. State the question to be answered.
2. Identify the minimum representation needed to answer it.
3. Decide physical vs analytical, focused vs comprehensive, scale, fidelity and system level.
4. Choose one or more fabrication/testing routes.
5. Decide serial iteration vs parallel concepts.
6. Define evidence to collect before building.
7. Build and test.
8. Record learning and determine whether another prototype is justified.

Camburn et al. describe prototyping strategy as a planned combination of techniques used to achieve objectives, with individual builds characterized by scale, system level, requirements fidelity and media. Their review also identifies iteration and parallel testing as cross-cutting strategic techniques.

## 9. Decision Criteria
Prototype strategy should be driven by uncertainty and learning value rather than by a desire for visual completeness. Increase fidelity only when the question requires it. Use focused prototypes for isolated mechanisms, interfaces, dimensions or functions; use comprehensive prototypes when system-level interaction is itself the uncertainty.

## 10. Alternatives and Tradeoffs
- Analytical model/simulation: fast and inexpensive for modeled behavior, but limited by model assumptions.
- Physical focused prototype: efficient for specific questions but may hide integration effects.
- Comprehensive prototype: strong integration evidence but expensive and slow.
- Parallel prototypes: explore more of the design space but consume additional resources.
- Sequential iteration: concentrates resources but risks local optimization.

## 11. Limitations / Failure Conditions
- Building before defining the question.
- Confusing appearance fidelity with functional fidelity.
- Treating a prototype as production evidence when materials/processes differ materially.
- Changing multiple variables without a test plan.
- Failing to capture prototype configuration and test conditions.

## 12. Common Mistakes
- "Make it as close to final as possible" too early.
- One prototype intended to answer every question.
- No hypothesis or acceptance criteria.
- Prototype becomes an undocumented one-off hero build.
- Prototype manufacturing method silently creates behavior different from production intent.

## 13. Standards and Regulations
There is no universal normative standard prescribing a product-development prototype strategy. Technology-specific standards become relevant to the methods used. For additive manufacturing terminology, ISO/ASTM 52900:2021 is a foundational vocabulary standard.

## 14. Academic Evidence
- Camburn, B. et al. (2017), "Design prototyping methods: state of the art in strategies, techniques, and guidelines," Design Science 3, e13, DOI 10.1017/dsj.2017.10. Open access.
- Camburn, B. et al. (2017), "Design prototyping of systems," ICED17. Proposes system-prototyping phases including partitioning, search and implementation.

## 15. Books and Professional Handbooks
Research gap: extract and cross-check prototype classifications and planning guidance from Product Design and Development (Ulrich, Eppinger & Yang) and other canonical product-development texts.

## 16. Industry Guidance / White Papers
- NIST MEP: Product Design and Development.
- NIST MEP: Additive Manufacturing/3D Printing.
- NASA Ames Applied Manufacturing and Engineering Test Division.

## 17. Courses, Lectures and Training Material
MIT OCW 16.810 Engineering Design and Rapid Prototyping: integrates requirements, CAD/CAE/CAM, fabrication, testing, iteration and optimization.

## 18. Case Studies
To be expanded. NASA Ames and SLAC provide institutional examples where engineering and fabrication capabilities are colocated to support development from concepts to finished hardware.

## 19. Relationships
| Type | Target Object | Strength | Confidence | Reason | Evidence |
|---|---|---|---|---|---|
| USES | H2P-PW-002 Prototype Fidelity | Strong | High | Fidelity is a primary strategic choice in prototype embodiment. | Camburn 2017 |
| USES | H2P-PW-003 Prototype Purpose Classification | Strong | High | Strategy begins with why the prototype is being built. | Camburn 2017 |
| ENABLES | H2P-PW-004 Rapid Iteration Loop | Strong | High | Planned prototype sequencing creates deliberate iteration. | Camburn 2017; MIT 16.810 |
| REQUIRES | H2P-PW-006 Prototype Build Planning | Strong | High | Strategy must become an executable build/test plan. | MIT 16.810 |
| INFORMS | H2P-PW-008 Prototype Make vs Buy | Medium | High | Required fidelity, speed and process determine internal/external sourcing options. | Project synthesis |
| REQUIRES | H2P-PW-009 Workshop Capability Matrix | Medium | High | Internal prototype choices depend on available capability. | NASA Ames; MIT makerspaces |
| PRODUCES | H2P-PW-162 Prototype Learning Capture | Strong | High | The intended output of prototyping is evidence and learning. | Camburn 2017 |

## 20. Open Questions / Evidence Gaps
- Quantitative frameworks for selecting prototype fidelity vs expected information gain.
- Strong empirical evidence comparing parallel vs sequential prototyping for hardware programs.
- Industry-specific deviations in regulated products.

## 21. Podcast Mapping
- Relevant section: The Prototype Shop
- Candidate episode(s): Why Prototype?; Building a Prototype Strategy; Shortening the Design-Build-Test Loop
- Listener tags: #PrototypeStrategy #RapidIteration #PrototypeFidelity
- Prerequisite objects: none

## 22. Future Toolkit Mapping
Reserved.

## 23. Future Learning Path Mapping
Reserved.

## 24. Revision Notes
v0.1 — First evidence-backed object created from Camburn, MIT, NIST and NASA anchor sources.