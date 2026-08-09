# 2.1–2.3 DFM, DFA & DFT Core

status: Researching
provenance: [GNR]

## DFM — process-driven design
Design features should be evaluated against candidate production processes, tooling, access, material behavior, capability, inspection, volume and cost per good part.

### DFM objects
- feature
- functional requirement
- candidate process
- process constraint
- tooling/access constraint
- manufacturability risk
- capability expectation
- secondary operation
- inspection requirement
- cost/volume sensitivity

### Principle
A nominally manufacturable feature is not necessarily production-capable if it depends on unstable process tails, excessive inspection, manual adjustment or unrealistic supplier capability.

## DFA — assembly and mistake prevention
### Objects
- part count
- handling/orientation
- insertion/mating
- fastening/joining
- datum/alignment
- accessibility
- sequence
- force/torque
- connector/interface
- mistake-proofing
- verification
- rework/disassembly boundary

### Questions
- Can a component be installed backwards, swapped or omitted?
- Can interfaces self-locate or require skilled alignment?
- Are fasteners/tools accessible and standardized where sensible?
- Does assembly force damage or preload components?
- Can the assembly state be verified before it becomes hidden?

### Principle
Operator training is weaker than eliminating an error opportunity through design or engineered mistake prevention where practical.

## DFT — test/calibration/traceability by design
### Objects
- test point/interface
- diagnostic access
- isolation boundary
- stimulus/response
- calibration access
- serial/identity carrier
- software/configuration identity
- sensor/reference interface
- fault localization
- test fixture interface

### Questions
- Can every critical requirement be verified at the right level?
- Can failures be localized without destructive disassembly?
- Does calibration require inaccessible adjustments?
- Is unit identity preserved through assembly/test/service?
- Can production test reach the relevant state safely and repeatably?

### Principle
Testability designed late often creates expensive fixtures, long EOL cycles and poor diagnostic resolution.

## Decision objects
### D-DFX-DFM-001 — Design feature versus candidate production processes
### D-DFX-DFA-001 — Assembly simplification/mistake-prevention opportunity
### D-DFX-DFT-001 — Required test/calibration/diagnostic access

## Cross-links
DFM <-> Manufacturing Process Atlas
DFA <-> tooling/standard work/ergonomics
DFT <-> production test/MSA/EOL
DFX <-> PFMEA/reliability
DFX <-> cost/supply chain