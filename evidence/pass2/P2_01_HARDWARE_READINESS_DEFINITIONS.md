# Pass 2.01 — Hardware Evolution & Manufacturing Readiness Definitions

status: ACTIVE — DEPTH PASS
created_on: 2026-08-11
maps_to: Opening Arc A1–A8; Episodes 1–5, 26–31; Hardware Evolution Ladder
canonical_owners: A0 Early Hardware Development; A1 Product Readiness/NPI; A5 Pilot/Ramp/Capacity

## Purpose
Turn the podcast's Hardware Evolution Ladder from a useful editorial sequence into an evidence-scoped readiness framework. The goal is not to pretend DEV/LVP/SVP or the Ladder are industry-standard lifecycle names. The goal is to show what evidence changes as hardware moves from concept and proof-of-concept toward production-intent, low-rate production, ramp and serial production.

## Primary-source depth backbone

### NASA Technology Readiness Levels (TRL)
NASA defines TRL as a maturity measurement for a particular technology. Key hardware distinctions useful to our framework include:
- TRL 3: analytical/experimental proof of critical function or characteristic;
- TRL 4: component/breadboard validation in laboratory environment;
- TRL 5: component/breadboard validation in relevant environment;
- TRL 6: system/subsystem model or prototype demonstration in relevant environment;
- TRL 7: system prototype demonstration in operational environment;
- TRL 8: actual system completed and qualified through test/demonstration;
- TRL 9: actual system proven through successful operations.

Applicability boundary: TRL describes technology maturity. It does not by itself establish manufacturing readiness, supplier readiness, production rate capability, quality-system maturity or commercial economics.

### NASA Production Readiness Review (PRR)
NASA PRR asks whether developers are ready to efficiently produce/build/integrate/test the required number of systems and whether production plans support operational needs.

Representative entrance themes include:
- significant production-engineering problems from development resolved;
- design documentation adequate for production;
- production plans/preparation adequate to begin fabrication;
- production-enabling products/resources available and allocated;
- production risks and mitigations identified;
- schedule reflects production activities.

Applicability boundary: NASA PRR is an aerospace/program review model. We use it as strong evidence for categories of production-readiness evidence, not as a universal mandatory gate for startups.

### DoD Manufacturing Readiness Levels (MRL)
The DoD MRL framework explicitly separates manufacturing maturity from technology maturity and progresses toward pilot-line, low-rate and full-rate production readiness.

High-level depth anchors from the current MRL definitions include:
- MRL 8: pilot-line capability demonstrated; manufacturing and quality processes/procedures proven in pilot-line environment, controlled and ready for low-rate production; supply chain established/stable; materials available for planned low-rate schedule;
- MRL 9: low-rate production demonstrated and capability in place for full-rate production; major design features stable/proven; processes established/controlled at an appropriate quality level; learning/cost evidence developing for full-rate production;
- MRL 10: full-rate production demonstrated; engineering/design changes relatively few; materials, manufacturing processes, procedures, inspection and test equipment in production and controlled; production meets engineering/performance/quality/reliability requirements.

Applicability boundary: MRL definitions are defense-acquisition constructs and include program-specific language. We use their separation of manufacturing maturity dimensions and evidence progression, not their acquisition milestones as generic startup requirements.

## Core synthesis — readiness is multidimensional
A product can have high technology maturity and still have low manufacturing readiness.

For the podcast, readiness should be discussed through at least these dimensions:
1. functional/technology evidence;
2. integrated-system evidence;
3. design/configuration stability;
4. production-process maturity;
5. measurement/quality-control maturity;
6. supplier/material maturity;
7. tooling/equipment/test readiness;
8. documentation/work-instruction readiness;
9. rate/capacity/yield evidence;
10. service/support/lifecycle readiness where relevant.

This is a synthesis aligned with NASA TRL/PRR and DoD MRL concepts; it is not claimed as a quoted standard taxonomy.

## Hardware Evolution Ladder — evidence interpretation
Canonical editorial ladder:
`Idea → Requirements → Architecture → POC → Integrated Prototype → Engineering Prototype → Production-Intent Hardware → LVP → Production Validation → Ramp → SVP`

### Idea → Requirements
Primary exit evidence:
- problem/use case articulated;
- critical functional/environmental/safety assumptions explicit;
- first measurable success criteria defined;
- major unknowns identified.

Do not imply: a complete production specification is required before exploration.

### Requirements → Architecture
Primary exit evidence:
- system boundaries/interfaces defined enough to assign ownership;
- key technology/process risks identified;
- architecture supports intended verification approach;
- obvious future manufacturing/test/service constraints are not ignored.

### Architecture → POC
Primary exit evidence:
- critical technical principle demonstrated analytically/experimentally;
- test result is linked to the specific hypothesis being reduced;
- limitations of the POC are explicit.

Strong analogy: NASA TRL 3, but not a one-to-one equivalence.

### POC → Integrated Prototype
Primary exit evidence:
- critical subsystems coexist and interfaces work sufficiently to expose integration risk;
- major scaling/environment assumptions begin to be tested;
- configuration identity is retained enough to know what was actually tested.

### Integrated Prototype → Engineering Prototype
Primary exit evidence:
- prototype is sufficiently representative for the engineering questions being asked;
- critical requirements have verification methods;
- environmental/load/boundary testing is increasingly realistic;
- prototype shortcuts and their expiration conditions are explicit.

Analogous to progression toward TRL 5/6 concepts where relevant; do not label generically as a TRL without formal assessment.

### Engineering Prototype → Production-Intent Hardware
Primary exit evidence:
- intended materials/components/processes/suppliers are increasingly representative;
- CTQs and inspection/test strategy exist;
- drawings/BOM/configuration are controlled enough to reproduce the build;
- DFM/DFA/DFT issues are addressed or consciously risk-accepted;
- changes in production route are recognized as potential evidence-invalidating changes.

### Production-Intent → LVP
Primary exit evidence:
- production documentation supports repeatable builds;
- tooling/fixtures/test equipment are usable and controlled;
- process risks/controls and measurement adequacy are understood;
- supplier/material availability supports the planned quantity;
- operators can build without continuous designer intervention, except where explicitly accepted for the maturity stage;
- traceability and nonconformance/change processes are sufficient for learning from the build.

NASA PRR and DoD MRL concepts strongly support this category of evidence, but exact startup thresholds are context-specific.

### LVP → Production Validation
Primary exit evidence:
- representative production route produces repeated units;
- yield/rework/defect data are captured;
- major failure/recovery modes are understood;
- process controls and reaction plans function in practice;
- production changes are configuration-controlled;
- capacity assumptions are tested rather than inferred from one ideal cycle.

### Production Validation → Ramp
Primary exit evidence:
- production rate is demonstrated for a meaningful duration/product mix;
- bottlenecks, downtime, WIP, staffing and maintenance assumptions are understood;
- supplier and material flow can support planned ramp;
- quality/yield performance is not dependent on exceptional engineering intervention;
- open risks have owners/mitigations.

### Ramp → SVP
Primary exit evidence:
- sustained rate/capacity meets business need under defined assumptions;
- process and measurement systems are sufficiently stable/capable for CTQs;
- supplier/process/change controls operate as a system;
- cost model is increasingly based on actual production behavior;
- engineering changes are controlled and their production evidence impact is assessed;
- service/field feedback is connected where applicable.

## Critical claim register

### P2-C-RDY-001 — Technology maturity and manufacturing readiness are different dimensions
status: STRONG
Evidence: NASA TRL versus DoD MRL/PRR.
Podcast use: foundational.

### P2-C-RDY-002 — A working prototype is not evidence of readiness to repeatedly produce the required quantity
status: STRONG
Evidence: NASA PRR purpose/entrance themes + MRL progression.

### P2-C-RDY-003 — Production readiness requires evidence across design, process, resources, quality, supply and rate; no single build result is sufficient
status: STRONG SYNTHESIS
Evidence: NASA PRR + DoD MRL.

### P2-C-RDY-004 — The podcast Hardware Evolution Ladder is an editorial decision framework, not an industry-standard lifecycle
status: GOVERNANCE RULE

### P2-C-RDY-005 — Exit evidence should be tied to the uncertainty being retired at that stage rather than a universal document checklist
status: STRONG ENGINEERING SYNTHESIS
Needs additional case/examples before Podcast Ready.

## Myths to reject
- “TRL 6 means we are ready for production.”
- “The prototype works, so the design is production ready.”
- “A successful pilot means full-rate capacity is proven.”
- “Production readiness is just DFM.”
- “Every startup must use NASA/DoD gates literally.”

## Applicability Statements

### AS-P2-TRL-001
Source family: NASA TRL.
Applies when: describing maturity of a technology/system relative to demonstrated environments and integration.
Does not imply: manufacturing readiness, cost readiness, supplier maturity or rate capability.
Decision linkage: maturity evidence interpretation in A0/A1.

### AS-P2-PRR-001
Source family: NASA PRR.
Applies when: identifying evidence categories for readiness to repeatedly build/integrate/test required quantities.
Does not imply: a startup must perform a NASA-format formal review.
Decision linkage: production-intent/LVP/production-validation gates.

### AS-P2-MRL-001
Source family: DoD MRL.
Applies when: reasoning about progression from manufacturing development through pilot/low-rate/full-rate production and the maturity dimensions needed.
Does not imply: DoD acquisition milestone language or numerical MRL assignment applies universally.
Decision linkage: LVP/ramp/SVP readiness matrix.

## Worked-example target for next step
Build one fictional hardware product through the complete Ladder and show, at each transition:
- what changed physically;
- what evidence was generated;
- what evidence did NOT transfer;
- what production debt remained;
- what would block the next stage.

This becomes the reusable narrative spine for Opening Arc + Episode 60.

## Remaining depth work
1. Extract NASA systems-engineering review definitions/criteria for requirements/design/verification gates where useful.
2. Extract current DoD MRL thread/sub-thread structure at useful depth without importing acquisition bureaucracy into the podcast.
3. Reconcile readiness terminology with NPI/PVT conventions already captured in A1/A5.
4. Build the worked hardware example.
5. Map readiness evidence to DEV/LVP/SVP listener-facing checklist.
6. Promote only evidence-backed portions to Podcast Ready.

## Readiness
Primary-source depth backbone: CAPTURED
Applicability boundaries: CAPTURED
Canonical synthesis: CAPTURED
Worked example: NEXT
Podcast Ready: NOT YET