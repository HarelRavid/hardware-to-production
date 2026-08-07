---
id: H2P-PW-002
title: Prototype Fidelity
aliases: [Prototype Resolution, Prototype Representativeness]
object_type: Concept
domain: Prototype Workshop
subdomain: Strategy & Workshop Architecture
lifecycle: [Concept, POC, Prototype, Engineering Prototype, EVT, DVT]
status: Researching
summary: The degree to which a prototype represents selected attributes of the intended product; fidelity must be defined relative to the question being tested rather than as a single low-to-high score.
tags: [prototype-fidelity, focused-prototype, comprehensive-prototype, representativeness]
created: 2026-08-07
last_reviewed: 2026-08-07
---

# Prototype Fidelity

## 1. Definition
Prototype Fidelity is the degree of representativeness of a prototype with respect to the attributes relevant to a specific test or learning objective. Fidelity is multidimensional: geometry, appearance, material, mechanics, interfaces, controls, user interaction, manufacturing process and environment may each have different fidelity levels.

## 2. Purpose
To deliberately choose which aspects of the final product must be represented accurately and which can be simplified, substituted or omitted.

## 3. Problem Solved
Treating fidelity as "how close is this to the final product?" encourages expensive comprehensive builds. A prototype can be extremely high fidelity in one attribute and intentionally crude in another.

## 4. Lifecycle Position
Fidelity generally increases as design maturity increases, but it should not rise monotonically for every attribute. Focused low-cost rigs remain valuable even during EVT/DVT when the question is localized.

## 5. Typical Owner / Responsible Roles
Design engineering, systems engineering, test engineering, prototype engineering.

## 6. Inputs / Preconditions
Prototype purpose, test question, requirements, risk, available manufacturing methods.

## 7. Outputs / Deliverables
A stated fidelity profile identifying which characteristics must be representative for the evidence to be valid.

## 8. How It Works
Useful dimensions include:
- Scale.
- System level: component, subsystem, integrated system.
- Requirements/functional fidelity.
- Geometric fidelity.
- Material fidelity.
- Interface fidelity.
- Manufacturing-process fidelity.
- Environmental fidelity.
- Media: physical, analytical/virtual, hybrid.

Camburn et al. explicitly model scale, system level, requirements fidelity and media as independent prototype-strategy dimensions. Product-development literature also commonly distinguishes focused vs comprehensive and physical vs analytical prototypes.

## 9. Decision Criteria
Set the minimum fidelity required for the intended decision. Production-process fidelity becomes critical when testing behavior that depends on production material, surface state, tolerance, residual stress, joining or assembly variation.

## 10. Alternatives and Tradeoffs
Higher fidelity can increase evidence relevance but usually adds cost, lead time and design commitment. Lower/focused fidelity can dramatically accelerate learning but may not expose integration effects.

## 11. Limitations / Failure Conditions
Evidence is invalid when the missing fidelity dimension materially influences the tested behavior and this is not recognized.

## 12. Common Mistakes
- Calling a prototype simply "low fidelity" or "high fidelity" without stating the dimension.
- Testing structural performance on a geometry-accurate but mechanically nonrepresentative material.
- Using a 3D-printed part as evidence for injection-molded production behavior without identifying process differences.
- Equating cosmetic fidelity with design maturity.

## 13. Standards and Regulations
Method-specific standards apply; there is no universal prototype-fidelity standard.

## 14. Academic Evidence
Camburn et al. (2017), Design Science, DOI 10.1017/dsj.2017.10, provides the primary framework currently adopted by this Knowledge OS.

## 15. Books and Professional Handbooks
Gap: validate terminology against current edition of Ulrich/Eppinger/Yang and additional product-design texts.

## 16. Industry Guidance / White Papers
NIST additive-manufacturing guidance supports rapid iteration but reinforces the need to recognize the differing economics and properties of manufacturing methods.

## 17. Courses, Lectures and Training Material
MIT OCW 16.810 combines analytical analysis, CAD, CAM, physical manufacturing and structural testing, providing a practical example of mixed prototype media/fidelity.

## 18. Case Studies
To be developed during technology-specific research.

## 19. Relationships
| Type | Target Object | Strength | Confidence | Reason | Evidence |
|---|---|---|---|---|---|
| USED_BY | H2P-PW-001 Prototype Strategy | Strong | High | Fidelity is a core strategic variable. | Camburn 2017 |
| DETERMINED_BY | H2P-PW-003 Prototype Purpose Classification | Strong | High | Required fidelity depends on what the build must demonstrate. | Camburn 2017 |
| INFORMS | H2P-PW-006 Prototype Build Planning | Strong | High | Fidelity drives material/process/test choices. | Engineering synthesis |
| INFORMS | H2P-PW-008 Prototype Make vs Buy | Strong | High | Required fidelity can force specialized external or production-representative processes. | Project synthesis |
| CONSTRAINS | H2P-PW-021 FDM / FFF Printing | Medium | High | FDM is suitable only where its achievable fidelity supports the question. | NIST AM + synthesis |
| CONSTRAINS | H2P-PW-049 CNC Milling | Medium | High | CNC may be selected when material/geometric fidelity requirements exceed simpler methods. | Engineering synthesis |

## 20. Open Questions / Evidence Gaps
Develop a controlled fidelity taxonomy specific to hardware industrialization and map each manufacturing technology to fidelity dimensions.

## 21. Podcast Mapping
- Relevant section: The Prototype Shop
- Candidate episode(s): Stop Building the Final Product Too Early; Choosing the Right Prototype
- Listener tags: #PrototypeFidelity #PrototypeStrategy
- Prerequisite objects: H2P-PW-003

## 22. Future Toolkit Mapping
Reserved.

## 23. Future Learning Path Mapping
Reserved.

## 24. Revision Notes
v0.1 — Initial fidelity model anchored in Camburn et al.