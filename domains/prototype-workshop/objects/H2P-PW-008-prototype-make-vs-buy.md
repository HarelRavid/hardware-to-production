---
id: H2P-PW-008
title: Prototype Make vs Buy
aliases: [Prototype In-house vs Outsource Decision]
object_type: Method
domain: Prototype Workshop
subdomain: Capability & Investment Decisions
lifecycle: [POC, Prototype, Engineering Prototype, EVT, DVT]
status: Researching
summary: A structured decision method for choosing whether a prototype part, assembly or process should be executed internally or sourced externally, considering learning speed, capability, strategic knowledge, cost, uncertainty and supply risk.
tags: [make-buy, outsourcing, prototype-sourcing, capability, lead-time, workshop-strategy]
created: 2026-08-07
last_reviewed: 2026-08-07
---

# Prototype Make vs Buy

## 1. Definition
Prototype Make vs Buy is the sourcing decision applied to development work: determine whether a prototype activity should be performed using internal workshop capability or purchased from an external supplier/service bureau.

The decision is not identical to production make/buy. In prototyping, the value of fast feedback, tacit learning, design confidentiality, iteration flexibility and engineering access may outweigh nominal piece-price differences.

## 2. Purpose
- Put rapid, high-learning activities close to the design team when justified.
- Use external specialists where capability, process fidelity, certification or equipment economics favor outsourcing.
- Avoid buying capital equipment merely because a single prototype is expensive externally.
- Preserve strategically important know-how and reduce dependency where appropriate.

## 3. Problem Solved
Prototype teams often default either to "do everything in-house" or "send everything out." Both can be inefficient. The correct decision depends on the engineering learning objective, required process fidelity, utilization, supplier lead time, internal skills and strategic importance.

## 4. Lifecycle Position
The decision begins at POC and changes as product maturity increases. Early prototypes favor speed and learning; EVT/DVT increasingly favor representative materials/processes and supplier/process realism. A process may therefore be made internally early and bought later, or vice versa.

## 5. Typical Owner / Responsible Roles
Development Engineering, Prototype/Workshop Lead, NPI/Manufacturing Engineering, Supply Chain/Purchasing, Finance for significant CAPEX.

## 6. Inputs / Preconditions
- Prototype objective and fidelity requirement.
- Internal capability matrix.
- Supplier capabilities and lead times.
- Expected iteration count and annual utilization.
- Equipment/tooling/maintenance/training cost.
- IP, quality, safety and strategic capability considerations.

## 7. Outputs / Deliverables
- Make/buy decision and rationale.
- Selected supplier or internal process.
- Identified capability gap.
- CAPEX candidate if repeated demand justifies investment.
- Risk controls for outsourced or internal work.

## 8. How It Works
Evaluate at least six dimensions:
1. Learning latency: how quickly can engineers change, build and retest?
2. Capability: can the internal process achieve the required geometry, material, tolerance and test fidelity?
3. Strategic knowledge: does doing the work internally create or protect know-how that matters?
4. Economics: total cost across expected iterations, not one-piece price alone.
5. Risk: supplier dependency, queue, quality variation, IP, logistics and schedule uncertainty.
6. Production relevance: does the prototype need a production-representative process that the internal shop cannot reproduce?

Academic make/buy literature repeatedly identifies strategy/core competency, capability, transaction cost and uncertainty/risk as central determinants. Those principles transfer well to prototype sourcing, with added emphasis on iteration speed and learning.

## 9. Decision Criteria
Favor internal execution when:
- iteration frequency is high;
- engineer-to-machine feedback needs to be immediate;
- geometry/design changes are frequent;
- the capability is reusable across many programs;
- internal learning itself is strategically valuable;
- external queue/logistics dominate cycle time.

Favor outsourcing when:
- specialized/high-cost equipment would have low utilization;
- production-representative processes are required;
- special certifications, expertise or environmental controls are required;
- supplier capability materially exceeds internal capability;
- external economics remain superior after total lead-time/risk costs are included.

## 10. Alternatives and Tradeoffs
A hybrid model is often strongest: retain fast general-purpose capabilities in-house and use external specialists for capital-intensive, regulated or low-frequency processes.

## 11. Limitations / Failure Conditions
- Comparing external unit price only against internal material cost.
- Ignoring operator training, maintenance, utilities, extraction, inspection and floor space.
- Buying equipment without expected utilization or capability ownership.
- Outsourcing work where engineering learning depends on observing the process.
- Keeping a process in-house after prototype requirements exceed workshop capability.

## 12. Common Mistakes
- "We used it three times, so we need to buy the machine."
- "Supplier price is cheaper" while ignoring a two-week iteration delay.
- Treating prototype suppliers as production-qualified suppliers.
- Confusing possession of a machine with process capability.

## 13. Standards and Regulations
No universal make/buy standard. Process-specific safety, quality and regulatory obligations remain applicable regardless of sourcing model.

## 14. Academic Evidence
- Parmigiani-style make/buy theory is represented here through modern review literature.
- "Should we make or buy? An update and review" (2018) concludes that sourcing decisions should combine resource-based, strategic-management and transaction-cost perspectives; strategy, capabilities and uncertainty are recurring determinants.
- "New dimensions of outsourcing" (2000) combines transaction-cost economics with core-competency theory.
- Mantel et al. (2006), Journal of Operations Management: strategic vulnerability and core competency influence make/buy evaluation.

## 15. Books and Professional Handbooks
Gap to fill: sourcing strategy, operations strategy and product-development literature specifically addressing prototype/internal workshop capability.

## 16. Industry Guidance / White Papers
- NIST equipment pre-purchase guidance highlights lifecycle questions around financing, installation, safety, maintenance and disposal rather than purchase price alone.
- NIST MEP supplier scouting illustrates access to external manufacturing capability as a deliberate supply-chain capability.

## 17. Courses, Lectures and Training Material
To be expanded during the workshop economics research wave.

## 18. Case Studies
Institutional models at NASA Ames and SLAC demonstrate a conscious choice to maintain broad in-house fabrication and test capabilities where rapid interaction with researchers and engineers creates value.

## 19. Relationships
| Type | Target Object | Strength | Confidence | Reason | Evidence |
|---|---|---|---|---|---|
| INFORMED_BY | H2P-PW-001 Prototype Strategy | Strong | High | Prototype purpose/fidelity determine required sourcing capability. | Camburn 2017; synthesis |
| REQUIRES | H2P-PW-009 Workshop Capability Matrix | Strong | High | A make decision requires knowing actual internal capability. | Project model |
| COMPARES | H2P-PW-168 Outsourcing Lead Time | Strong | High | Supplier lead time directly affects development latency. | Project model |
| CONSIDERS | H2P-PW-169 Outsourcing Quality Risk | Strong | High | Quality uncertainty is part of sourcing risk. | Make/buy literature |
| CONSIDERS | H2P-PW-170 Internal Capability Readiness | Strong | High | Equipment ownership is insufficient without competent process capability. | Engineering synthesis |
| INFORMS | H2P-PW-165 Equipment Purchase Decision | Strong | High | Repeated make/buy outcomes can justify investment. | NIST pre-purchase guidance |
| INFORMS | H2P-PW-166 Workshop CAPEX Prioritization | Medium | High | Capability gaps and repeated outsourcing identify investment candidates. | Project synthesis |
| AFFECTS | H2P-PW-163 Design Iteration Cycle Time | Strong | High | Sourcing choice can add or remove queue and logistics time. | NIST AM; engineering synthesis |

## 20. Open Questions / Evidence Gaps
- Develop a prototype-specific total-cost model including value of learning delay.
- Identify threshold frameworks for equipment utilization/CAPEX decisions.
- Collect hardware-startup case studies comparing in-house shop strategies.

## 21. Podcast Mapping
- Relevant section: The Prototype Shop
- Candidate episode(s): What Should You Make In-house?; When to Stop Making It Yourself; Building a Prototype Shop by ROI
- Listener tags: #MakeVsBuy #PrototypeSourcing #WorkshopROI
- Prerequisite objects: H2P-PW-001, H2P-PW-009

## 22. Future Toolkit Mapping
Reserved.

## 23. Future Learning Path Mapping
Reserved.

## 24. Revision Notes
v0.1 — Prototype-specific synthesis of make/buy literature plus NIST equipment/supplier guidance.