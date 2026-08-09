# DFM / DFA / DFT Foundations — Evidence Source Map

status: BREADTH COMPLETE
campaign: A2
maps_to: MASTER_WBS Section 2; PODCAST_MAP Episodes 6–10
provenance: primary-source-first

## Purpose
Build the evidence backbone for cross-process design decisions that determine whether hardware can be manufactured, assembled, tested, tolerated, serviced and transitioned from prototype to production economically and robustly.

## Authoritative source families captured

### NIST manufacturing/design research
Use for:
- conceptual process planning
- manufacturability during early design
- assembly-design exploration/optimization
- process/material selection
- manufacturing cost/time estimation during design

Key sources:
- Conceptual Process Planning — A Definition and Functional Decomposition
- Incorporating Process Planning into Conceptual Design
- Manufacturing Process and Material Selection During Conceptual Design
- A Decision Support System for Material and Manufacturing Process Selection
- A Web-Based Process/Material Advisory System
- A System for Generating Process and Material Selection Advice During Embodiment Design

Core evidence:
- manufacturability and manufacturing cost should be assessed during early design;
- material and process selection are coupled multi-attribute decisions;
- selected processes constrain detailed design;
- alternatives should balance functional requirements with manufacturing economics rather than optimize material or process in isolation.

### ASME Y14.5 / ISO GPS standards family
Use for:
- GD&T and geometric specification architecture
- datum/reference concepts
- communication of design intent across design, manufacturing and inspection
- specification versus verification boundaries
Applicability: exact edition and customer/jurisdiction requirements must be tracked; no copyrighted clause reproduction.

### DFA academic / industrial research
Captured source families:
- NIST / Journal of Mechanical Design assembly-design work
- CIRP assembly-sequence and operating-time literature
- industrial electronics NPI human-factors/DFA research

Core evidence:
- assembly sequence, access, handling, orientation and operating time can be evaluated as design variables;
- human factors and tooling/task design can influence assembly quality;
- DFA is broader than simple part-count reduction.

### IEEE 1149.1 / boundary-scan DFT
Primary standards-family evidence supports:
- embedding test access during IC architecture;
- testing assembled-board interconnections;
- observability/control/programming/debug through standardized test access;
- recovering testability as physical probe access decreases.

Applicability: electronics-specific implementation of a broader testability principle.

### Keysight commercial DFT guidance
Use for:
- board-level DFT implementation
- test-access constraints in dense PCBAs
- coverage analysis
- relationship between design choices and production-test coverage/debugging

### Material / process / lifecycle evidence
NIST sources now provide a strong source family showing material and process choice should be considered together during conceptual/embodiment design.

Additional lifecycle source family:
- NIST circular-product/circular-economy manufacturing models and literature

Use for:
- downstream lifecycle stages feeding back into design decisions;
- repair, reuse, remanufacturing and recovery as lifecycle considerations;
- material information as a product-lifecycle decision input.

Boundary: circular-economy research does not by itself prove that every product should be field-repairable; it supports the broader claim that service/recovery consequences can be legitimate design inputs.

### Prototype representativeness
NASA systems-engineering material remains the strongest primary source captured in Breadth Pass for explicit prototype/test-article pedigree and fidelity.

Core evidence:
- prototype/engineering/qualification/final units have different pedigree and inference boundaries;
- prototype fidelity should be sufficient for the conclusion being drawn;
- experience from prototypes can feed manufacturing, integration and maintainability improvements.

Breadth boundary:
- non-aerospace empirical prototype-route mismatch case studies remain a Pass-2 target rather than being overstated here.

## Claim register

### C-DFX-001 — Manufacturability should be evaluated during design, not only after design release
status: STRONG
Evidence basis: NIST conceptual-process-planning / DFM work.

### C-DFX-002 — DFM optimization of one part/process can worsen whole-product assembly/test/lifecycle performance
status: STRONG SYNTHESIS / case-study depth open
Evidence basis: NIST process/material multi-attribute decision work + DFA/DFT/lifecycle sources.
Boundary: requires case-specific tradeoff evidence; no universal numerical weighting is asserted.

### C-DFX-003 — DFA is broader than part-count reduction
status: STRONG DIRECTION
Evidence basis: assembly-design research on sequence, handling, feasibility, time, tooling and human factors.

### C-DFX-004 — Assembly sequence and accessibility can be engineering design variables
status: STRONG

### C-DFX-005 — Human factors in assembly can affect quality and should be considered before tooling/workstation freeze
status: MODERATE/STRONG INDUSTRIAL SUPPORT

### C-DFX-006 — Testability should be designed before production-test/EOL architecture is locked
status: STRONG FOR ELECTRONICS / broader generalization bounded

### C-DFX-007 — DFT is fundamentally about controllability, observability and access to what must be verified/diagnosed
status: STRONG FOR ELECTRONICS; general systems translation is synthesis

### C-DFX-008 — Dense/high-complexity electronics can lose physical test access, increasing value of architectural DFT
status: STRONG

### C-DFX-009 — Tighter tolerances are not automatically better
status: STRONG ENGINEERING DIRECTION
Boundary: quantitative tolerance-cost relationships are Pass-2 work.

### C-DFX-010 — Tolerance architecture should connect function, process capability and measurement capability
status: STRONG SYNTHESIS

### C-DFX-011 — Material selection cannot be separated from manufacturing route
status: STRONG
Evidence basis: NIST material/process selection research treats them as coupled decisions during early design.

### C-DFX-012 — Material/process selection is a multi-attribute decision, not a single-property optimization
status: STRONG
Evidence basis: NIST decision-support/process-selection work.

### C-DFX-013 — Service/repair/recovery consequences can legitimately feed back into product design
status: MODERATE/STRONG LIFECYCLE SUPPORT
Evidence basis: NIST circular-product/circular-economy activity models explicitly use downstream lifecycle data to inform design and include repair/remanufacturing/reuse flows.
Boundary: product-specific repairability requirement still depends on business, safety, regulatory and lifecycle context.

### C-DFX-014 — Prototype evidence transfers only across dimensions for which the prototype is sufficiently representative
status: STRONG CONCEPTUAL SUPPORT
Evidence basis: explicit test-article/product-form distinctions and prototype-fidelity logic in NASA systems engineering.
Boundary: non-aerospace case-study evidence remains Pass 2.

### C-DFX-015 — Process/material decisions made early constrain later detailed design and manufacturing economics
status: STRONG
Evidence basis: NIST conceptual/embodiment design and advisory-system research.

## Editorial conclusions supportable for Episodes 6–10
1. DFM belongs inside product design, not after release.
2. Material and process selection should be treated together.
3. DFA should be taught through sequence, handling, orientation, access, force, verification and human-error opportunity — not only part count.
4. DFT is designing the access/observability/controllability needed for verification and diagnosis before product architecture removes that access.
5. GD&T/tolerancing communicates functional intent across design, manufacturing and inspection; smaller numbers are not automatically better engineering.
6. Service/repair/lifecycle consequences are valid design inputs when relevant to the product strategy.
7. Prototype conclusions must be bounded by prototype fidelity and pedigree.
8. DEV/LVP/SVP should scale implementation rigor while preserving the same engineering questions.

## DEV / LVP / SVP lens
### DEV
Optimize learning speed while explicitly recording deferred DFX constraints and prototype-fidelity limits.

### LVP
Design for repeatable manual/semi-automated assembly, practical inspection/test access, controlled substitutions, economically sensible tolerances and feasible service/rework where intended.

### SVP
Design/process architecture must support capability, rate, scalable tooling/suppliers, production test, controlled variation, lifecycle strategy and robust diagnostics.

## Pass-2 depth targets
- tolerance-cost quantitative examples;
- measured DFA assembly-time/error-reduction case studies;
- board/system DFT coverage and defect-class tradeoffs;
- product-specific serviceability/repair economics;
- non-aerospace prototype-route mismatch case studies;
- quantitative lifecycle economics and cost-per-good-part examples;
- standards/version applicability mapping;
- case studies showing material/process choice forcing later redesign or manufacturing constraints.

## Readiness
Source map: BREADTH COMPLETE
Critical claims identified: YES
Primary-source backbone: YES
Weak/GNR claims visibly bounded: YES
Applicability conflicts visible: YES
Podcast Ready: NO