---
id: H2P-PW-003
title: Prototype Purpose Classification
aliases: [Why-to-Prototype Classification]
object_type: Method
domain: Prototype Workshop
subdomain: Strategy & Workshop Architecture
lifecycle: [Concept, POC, Prototype, Engineering Prototype, EVT, DVT]
status: Researching
summary: A method for classifying the question a prototype must answer before deciding its fidelity, construction method or test plan.
tags: [prototype-purpose, learning-objective, exploration, communication, verification]
created: 2026-08-07
last_reviewed: 2026-08-07
---

# Prototype Purpose Classification

## 1. Definition
Prototype Purpose Classification identifies why a prototype is being created before determining how it should be created. It separates learning objectives such as exploration, comparison, verification, integration, communication, usability and manufacturability so the build can be deliberately tailored to the decision it must support.

## 2. Purpose
- Prevent purposeless or overbuilt prototypes.
- Match prototype form to the uncertainty being reduced.
- Make test evidence and expected decisions explicit.
- Allow multiple focused prototypes to replace one expensive comprehensive build when appropriate.

## 3. Problem Solved
Teams often start from a fabrication technology ("let's print it") or maturity label ("build an MVP") rather than from the question. This creates prototypes that look useful but produce ambiguous evidence.

## 4. Lifecycle Position
Applicable throughout development. Typical emphasis shifts from concept exploration and communication early, toward function, integration, requirement verification, reliability and manufacturability later.

## 5. Typical Owner / Responsible Roles
Design/System Engineering, Prototype Engineering, Test Engineering, Product/Industrial Design, Manufacturing/NPI as manufacturing questions become prominent.

## 6. Inputs / Preconditions
Requirements, risks, unknowns, user questions, interface assumptions, manufacturing concerns.

## 7. Outputs / Deliverables
- Primary prototype purpose.
- Secondary purposes, if any.
- Question/hypothesis.
- Evidence required to close the question.
- Decision enabled by the result.

## 8. How It Works
A practical initial classification for Hardware to Production is:
1. Explore — learn whether a principle, architecture, mechanism or interaction is promising.
2. Compare — discriminate between competing concepts or implementations.
3. Understand — expose behavior, interfaces or failure mechanisms.
4. Communicate — make an idea understandable to users, stakeholders or manufacturing partners.
5. Verify — test whether a defined requirement or engineering target is met.
6. Integrate — reveal interactions between components/subsystems.
7. Validate use — test whether the solution works in the intended user/context problem.
8. Evaluate manufacturability — learn about assembly, tooling, process access, tolerance or manufacturing constraints.
9. De-risk — attack a high-consequence technical, schedule, supply or compliance uncertainty.

A single prototype can have multiple purposes, but one should normally be designated primary because competing objectives can demand contradictory fidelity and test choices.

## 9. Decision Criteria
The prototype purpose must be expressed as a question that can be closed by evidence. If the team cannot state what decision will change based on the build, the prototype objective is not mature enough.

## 10. Alternatives and Tradeoffs
A comprehensive prototype may answer multiple questions but can obscure causal learning and cost more. Focused prototypes isolate uncertainties more efficiently but may miss system-level effects.

## 11. Limitations / Failure Conditions
Purpose classification is ineffective if teams use generic labels without measurable evidence or if the purpose changes after the build without updating the test plan.

## 12. Common Mistakes
- Prototype built mainly because a machine is available.
- "Show progress" treated as the only objective.
- Using one build simultaneously for appearance approval, structural proof and manufacturing validation despite incompatible representations.
- No explicit decision tied to the result.

## 13. Standards and Regulations
No single normative standard defines prototype-purpose classes. Requirement verification and validation concepts become governed by sector/system-engineering standards where applicable.

## 14. Academic Evidence
Camburn et al. (2017) distinguishes "why to prototype" outcomes from "how to prototype" techniques and frames prototyping strategy as mapping techniques to intended outcomes.

## 15. Books and Professional Handbooks
Gap: compare purpose taxonomies from product-development, industrial-design and systems-engineering literature.

## 16. Industry Guidance / White Papers
NIST product-development guidance connects prototypes to testing customer problems, material selection and durability. NASA Ames explicitly uses fabrication/test support to turn concepts into prototypes and finished hardware while improving manufacturability.

## 17. Courses, Lectures and Training Material
MIT 16.810 demonstrates a requirement-driven prototype cycle with physical testing and redesign.

## 18. Case Studies
To be expanded with examples of focused test rigs, looks-like prototypes, works-like prototypes, integration prototypes and manufacturing-intent builds.

## 19. Relationships
| Type | Target Object | Strength | Confidence | Reason | Evidence |
|---|---|---|---|---|---|
| INFORMS | H2P-PW-001 Prototype Strategy | Strong | High | Why-to-prototype determines how-to-prototype. | Camburn 2017 |
| DETERMINES | H2P-PW-002 Prototype Fidelity | Strong | High | Purpose defines which attributes require fidelity. | Camburn 2017 |
| INFORMS | H2P-PW-006 Prototype Build Planning | Strong | High | Build/test planning must follow the intended learning objective. | MIT 16.810 |
| INFORMS | H2P-PW-008 Prototype Make vs Buy | Medium | High | Purpose may require immediate iteration or specialist production-representative capability. | Synthesis |
| PRODUCES | H2P-PW-162 Prototype Learning Capture | Strong | High | Classification defines the learning that must be captured. | Project model |

## 20. Open Questions / Evidence Gaps
- Harmonize this practical taxonomy against additional canonical prototype-purpose frameworks.
- Define examples and anti-examples for each purpose.
- Determine whether manufacturability deserves multiple sub-purposes (assembly, process, inspection, service).

## 21. Podcast Mapping
- Relevant section: The Prototype Shop
- Candidate episode(s): Why Are You Building This Prototype?; Choosing What to Learn Before Choosing How to Build
- Listener tags: #PrototypePurpose #PrototypeStrategy #EngineeringExperiment
- Prerequisite objects: none

## 22. Future Toolkit Mapping
Reserved.

## 23. Future Learning Path Mapping
Reserved.

## 24. Revision Notes
v0.1 — Initial purpose taxonomy anchored in Camburn et al. and refined for hardware industrialization.