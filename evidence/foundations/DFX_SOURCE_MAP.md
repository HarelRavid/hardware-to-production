# DFM / DFA / DFT Foundations — Evidence Source Map

status: IN PROGRESS — DFM/GD&T/DFA/DFT BACKBONE CAPTURED
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
- tolerancing/measurement/manufacturing integration
- process selection and digital manufacturing information

Key sources:
- NIST conceptual process-planning research: manufacturability and process planning belong in early design rather than only after release.
- Szykman & Kim, NIST / Journal of Mechanical Design, "Combining Interactive Exploration and Optimization for Assembly Design" (1998): assembly design is treated as a design-space problem with explicit constraints, design rationale and multiple alternatives.

Applicability: strong cross-industry engineering research; specific optimization methods are examples, not universal required workflows.

### ASME Y14.5 / ISO GPS standards family
Use for:
- GD&T and geometric specification architecture
- datum/reference concepts
- communication of design intent across design, manufacturing and inspection
- specification versus verification boundaries
Applicability: exact standard/version and jurisdiction/customer requirements must be tracked; no copyrighted clause reproduction.

### DFA academic / industrial research
Captured source families:
- CIRP / Procedia CIRP assembly-design literature
- Journal of Manufacturing Systems robotic-assembly research
- industrial ergonomics/assembly-quality research

Key evidence captured:
- DFA methods explicitly evaluate assembly sequence, handling/insertion or operating time rather than treating assembly as an afterthought.
- Carter (Journal of Manufacturing Systems, 1990) used laboratory/industrial task-time data in a robotic-DFA method and showed assembly-time estimates could materially change when realistic gripper-change effects were included.
- Kanai et al. / CIRP work uses DFA and predetermined-time standards to compare feasible assembly sequences by operating time.
- A 2017 industrial electronics NPI study developed a human-factors design-for-assembly scorecard during early design of tasks, fixtures and tooling and linked assembly complexity/human factors to quality outcomes.

Applicability boundary: Boothroyd-Dewhurst style metrics are methodology-specific; podcast conclusions should focus on transferable principles such as sequence, handling, orientation, access, force, verification and human-error opportunity.

### IEEE 1149.1 / boundary-scan DFT
Primary standards-family evidence captured from IEEE working-group / standards pages.

IEEE 1149.1 purpose/scope supports:
- including test logic during IC design;
- testing interconnections after ICs are assembled onto a PCB/substrate;
- observing, modifying or loading internal data during test/programming/configuration/debug;
- overcoming loss of physical probe access in dense assemblies through standardized embedded test access.

Applicability: electronics/PCB-specific DFT mechanism, not a universal DFT architecture for mechanical or process systems.

### Keysight commercial DFT guidance
Use for:
- board-level boundary-scan implementation
- test-access constraints in dense PCBAs
- chain architecture and signal integrity
- coverage analysis from schematic/netlist/BSDL data
- practical evidence that DFT choices affect production-test coverage and debugging

Applicability: experienced test-equipment/vendor guidance, subordinate to standards and product-specific validation.

### AIAG / automotive Core Tools
Use for:
- product/process risk linkage
- APQP/Control Plan/FMEA/MSA/SPC/PPAP relationships
- design/process development connection
Applicability: automotive-specific requirements; broader engineering logic must be separated from contractual requirements.

### Materials/process-selection literature and databases
Target use:
- material/process compatibility
- manufacturing route consequences
- whole-chain tradeoffs
Status: source capture still open.

## Claim register

### C-DFX-001 — Manufacturability should be evaluated during design, not only after design release
status: STRONG
Evidence basis: NIST early-design/conceptual process-planning work + APQP logic.
Podcast use: Episode 6.

### C-DFX-002 — DFM optimization of one part/process can worsen whole-product assembly/test/lifecycle performance
status: GNR SYNTHESIS
Need: systems/cost evidence and case studies.
Podcast use: Episodes 6, 11, 19.

### C-DFX-003 — DFA is broader than part-count reduction
status: STRONG DIRECTION
Evidence basis: assembly-design research explicitly models assembly sequence, geometric feasibility, handling/operating time, human factors and tooling/task design. These dimensions go beyond simply minimizing part count.
Podcast use: Episode 7.

### C-DFX-004 — Assembly sequence and accessibility can be engineering design variables, not merely shop-floor planning details
status: STRONG
Evidence basis: CIRP/NIST assembly-design research evaluates feasible sequences and their time/constraint consequences during design.
Podcast use: Episode 7.

### C-DFX-005 — Human factors in assembly can affect quality and should be considered before workstation/tooling freeze
status: MODERATE/STRONG INDUSTRIAL SUPPORT
Evidence basis: industrial electronics NPI research used early human-factors/DFA methods to identify assembly-quality risks during design/ramp.
Podcast use: Episodes 7 and 25.

### C-DFX-006 — Testability should be designed before production-test/EOL architecture is locked
status: STRONG FOR ELECTRONICS / broader-system generalization requires care
Evidence basis: IEEE 1149.1 explicitly embeds test-access structures into IC architecture to make assembled-board testing feasible when physical probe access is constrained. Keysight implementation guidance shows coverage depends on design choices made in the board architecture/layout.
Podcast use: Episode 8.

### C-DFX-007 — DFT is fundamentally about controllability/observability/access to the failure mechanisms or nodes being tested
status: STRONG FOR ELECTRONICS
Evidence basis: IEEE 1149.1 and boundary-scan practice provide a concrete standardized implementation of this principle.
Podcast use: Episode 8.

### C-DFX-008 — Dense/high-complexity electronics can lose physical test access, making embedded/architectural DFT more valuable
status: STRONG
Evidence basis: IEEE 1149.1 working-group need statement and Keysight DFT guidance cite increasing density/limited physical access as drivers for boundary scan.
Podcast use: Episode 8.

### C-DFX-009 — Tighter tolerances are not automatically better
status: STRONG ENGINEERING DIRECTION
Evidence basis: GD&T exists to communicate functional design intent and interchangeability; tolerance must be related to function rather than minimized indiscriminately. Quantitative cost/capability evidence remains Pass 2.
Podcast use: Episode 9.

### C-DFX-010 — Tolerance architecture should connect function, process capability and measurement capability
status: STRONG SYNTHESIS
Evidence direction: ASME/ISO GPS + later MSA/capability campaign.
Podcast use: Episode 9.

### C-DFX-011 — Material selection cannot be separated from manufacturing route and supply maturity
status: MODERATE/STRONG DIRECTION
Need: material/process-selection literature.
Podcast use: Episodes 6, 10, 11.

### C-DFX-012 — Prototype evidence transfers only across dimensions for which the prototype is representative
status: STRONG CONCEPTUAL SUPPORT from A0; non-aerospace depth still open.
Podcast use: Episodes 6, 9, 10.

## Editorial conclusions now supportable
1. DFM belongs in design, not as a release-afterthought.
2. DFA should be taught through sequence, handling, orientation, access, force, verification and human-error opportunity — not only part count.
3. DFT is best understood as designing access/controllability/observability before physical/product architecture removes that access.
4. GD&T/tolerancing should communicate functional intent across design, manufacturing and inspection rather than becoming a competition to specify the smallest numbers.
5. DEV/LVP/SVP implementations should scale the rigor, not change the underlying engineering logic.

## DEV / LVP / SVP lens
### DEV
Optimize learning speed while recording which DFX constraints are intentionally deferred. Prototype conveniences must be labeled when they remove production assembly/test constraints.

### LVP
Design must support repeatable manual/semi-automated assembly, practical access, mistake-resistant orientation, economical inspection/test, controlled substitutions and sensible tolerances.

### SVP
Design/process architecture must support capability, rate, scalable suppliers/tooling, high-throughput test where justified, controlled variation, service strategy and robust failure diagnosis.

## Breadth gaps to close
1. material/process-selection source backbone;
2. serviceability/repairability evidence;
3. non-aerospace prototype representativeness cases;
4. cross-process lifecycle-cost decision evidence;
5. stronger general-system DFT examples outside electronics;
6. top myths/mistakes/case studies for Episodes 6–10.

## Pass-2 candidates
- tolerance-cost quantitative examples;
- DFA case studies with measured assembly-time/error reduction;
- board/system DFT examples and test-coverage tradeoffs;
- material/process substitution failures;
- prototype-route mismatch case studies;
- standards/version applicability mapping;
- compare physical test-point access, boundary scan, functional test and software diagnostics by defect class.

## Readiness
Source map: IN PROGRESS
Critical claims identified: YES
Primary-source backbone: GOOD for DFM/GD&T/DFT; MODERATE for DFA
Applicability conflicts visible: YES
Podcast Ready: NO