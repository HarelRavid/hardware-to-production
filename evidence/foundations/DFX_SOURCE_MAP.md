# DFM / DFA / DFT Foundations — Evidence Source Map

status: IN PROGRESS
campaign: A2
maps_to: MASTER_WBS Section 2; PODCAST_MAP Episodes 6–10
provenance: primary-source-first

## Purpose
Build the evidence backbone for cross-process design decisions that determine whether hardware can be manufactured, assembled, tested, tolerated, serviced and transitioned from prototype to production economically and robustly.

## Initial authoritative source families

### AIAG / automotive Core Tools
Use for:
- product/process risk linkage
- APQP/Control Plan/FMEA/MSA/SPC/PPAP relationships
- design/process development connection
Applicability: automotive-specific requirements; broader engineering logic must be separated from contractual requirements.

### NIST manufacturing/design research
Use for:
- conceptual process planning
- manufacturability during early design
- tolerancing/measurement/manufacturing integration
- process selection and digital manufacturing information

### ASME Y14.5 / ISO GPS standards family
Use for:
- GD&T and geometric specification architecture
- datum/reference concepts
- specification versus verification boundaries
Applicability: exact standard/version and jurisdiction/customer requirements must be tracked; no copyrighted clause reproduction.

### IEC/IEEE/vendor DFT and electronics production guidance
Target use:
- test access
- boundary scan / board test architecture where applicable
- programming/calibration access
- electronics production-test design
Status: source capture open.

### Boothroyd-Dewhurst / academic DFA literature
Target use:
- assembly simplification
- part count/handling/insertion methodology
- evidence and limitations of DFA metrics
Status: source capture open; distinguish proprietary methodology from general principles.

### Materials/process-selection literature and databases
Target use:
- material/process compatibility
- manufacturing route consequences
- whole-chain tradeoffs
Status: source capture open.

## Initial claim register

### C-DFX-001 — Manufacturability should be evaluated during design, not only after design release
status: STRONG DIRECTION
Evidence basis: NIST early-design/conceptual process-planning work + APQP logic.

### C-DFX-002 — DFM optimization of one part/process can worsen whole-product assembly/test/lifecycle performance
status: GNR SYNTHESIS
Need: systems/cost evidence and case studies.

### C-DFX-003 — DFA includes mistake prevention, handling/orientation, access and verification, not only reducing part count
status: MODERATE DIRECTION
Need: authoritative/academic breadth.

### C-DFX-004 — Testability should be designed before production-test/EOL architecture is locked
status: GNR / HIGH PRIORITY
Need: electronics/system DFT sources and production examples.

### C-DFX-005 — Tighter tolerances are not automatically better
status: STRONG ENGINEERING DIRECTION
Need: tolerance-cost/capability evidence and standards boundary.

### C-DFX-006 — Tolerance architecture should connect function, process capability and measurement capability
status: STRONG SYNTHESIS
Need: ASME/ISO + MSA/capability corroboration.

### C-DFX-007 — Material selection cannot be separated from manufacturing route and supply maturity
status: MODERATE/STRONG DIRECTION
Need: material/process-selection literature.

### C-DFX-008 — Prototype evidence transfers only across dimensions for which the prototype is representative
status: STRONG CONCEPTUAL SUPPORT from A0; non-aerospace depth open.

## DEV / LVP / SVP lens
### DEV
Optimize learning speed while recording which DFX constraints are intentionally deferred.

### LVP
Design must support repeatable manual/semi-automated assembly, practical inspection/test, controlled substitutions and economically sensible tolerances.

### SVP
Design/process architecture must support capability, rate, scalable suppliers/tooling, automated or high-throughput test where justified, controlled variation and lifecycle/service strategy.

## Breadth gaps to close
1. authoritative DFA source family and empirical evidence;
2. DFT/test-access standards and industrial guidance;
3. tolerance/GD&T + cost/capability evidence;
4. material/process selection sources;
5. serviceability/repairability evidence;
6. non-aerospace prototype representativeness case studies;
7. cross-process lifecycle-cost decision evidence;
8. top myths/mistakes/case studies for Episodes 6–10.

## Pass-2 candidates
- tolerance-cost quantitative examples;
- DFA case studies with measured assembly-time/error reduction;
- board/system DFT examples and test-coverage tradeoffs;
- material/process substitution failures;
- prototype-route mismatch case studies;
- standards/version applicability mapping.

## Readiness
Source map: STARTED
Critical claims identified: YES
Primary-source backbone: PARTIAL
Applicability conflicts visible: YES
Podcast Ready: NO