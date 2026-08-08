# 4. Production System Engineering — Domain Map

status: Researching
provenance: [GNR]

## 4.1 Scope
Define how a released product definition becomes an executable, controlled and scalable manufacturing system.

## 4.2 Core modules
- EBOM -> MBOM transformation
- Manufacturing BOM structures and alternates
- Process flow / routing
- Operation sequencing
- Work centers and resources
- Tooling, jigs and fixtures
- Work instructions / standard work
- Training and operator qualification
- PFMEA / control plans / quality gates
- Production test and calibration
- Measurement-system capability
- Material handling and internal logistics
- Line layout and ergonomics

## 4.3 Core production-system objects
- product revision
- EBOM
- MBOM
- phantom/kit/subassembly boundary
- operation
- routing
- work center
- resource
- tooling/fixture
- process parameter set
- work instruction
- inspection/test step
- operator qualification
- material issue/consumption
- WIP state
- rework route
- scrap disposition
- traceability point
- quality gate

## 4.4 Engineering principle
A released design BOM is not yet a manufacturing system. Production requires an explicit model of how material, operations, resources, people, tooling, quality controls and data transform the product from incoming material to a released finished unit.

## 4.5 Master decision object
### D-PSE-MASTER-001 — Is the product definition executable in production?
Inputs: product revision, BOM maturity, assembly/process sequence, resource capability, tooling, work instructions, inspection/test, operator requirements, material logistics, traceability, quality controls, takt/capacity and change-control state.

Output: readiness gaps + required production-system objects + assumptions/open questions.

## 4.6 Cross-links
Production System <-> Manufacturing Processes
Production System <-> NPI
Production System <-> Quality
Production System <-> Supply Chain
Production System <-> Automation
Production System <-> Manufacturing Data Hub

## Integrity rule
Do not treat BOM release, work-instruction release or routing release as proof of manufacturing readiness unless the complete production system has been validated together.