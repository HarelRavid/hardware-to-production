# Section 5 — Pilot, Validation & Ramp — Domain Map

status: Researching
provenance: [GNR]

## Scope
Transition from a designed production system to demonstrated, repeatable production capability at intended or progressively representative scale.

## 5.1 Pilot-build planning
## 5.2 Production validation build
## 5.3 Yield / FPY / RTY
## 5.4 Rework and scrap
## 5.5 Learning curve
## 5.6 Capacity and bottlenecks
## 5.7 Takt and line balance
## 5.8 Supplier readiness
## 5.9 Engineering changes during ramp
## 5.10 Ramp exit criteria

## Core state model
Prototype-capable -> pilot-capable -> production-validation capable -> controlled ramp -> stable serial production.

These states are evidence states, not calendar phases.

## Core objects
- build
- unit/lot
- production-intent design
- production-intent material
- production-intent tooling
- production-intent process
- production-intent supplier
- operator qualification
- routing/WI
- inspection/test system
- defect
- yield
- rework
- cycle time
- capacity
- bottleneck
- change/deviation
- exit criterion

## Engineering principle
A successful build is not automatically evidence of a capable production system. The build conditions must be representative, controlled and traceable enough to support the conclusion being claimed.

## Master decision object
### D-RAMP-MASTER-001 — Is the product and production system ready to advance to the next ramp state?
Inputs: design maturity, configuration control, process/tooling readiness, supplier readiness, operator competence, MSA/test readiness, yield, defect Pareto, rework, cycle time, capacity, reliability evidence, open changes/deviations and risk.

Output: advance / conditional advance / hold + evidence + actions + owners + assumptions/open questions.

## Cross-links
Ramp <-> NPI readiness
Ramp <-> Production System Engineering
Ramp <-> Quality/Reliability
Ramp <-> Supply Chain
Ramp <-> Automation
Ramp <-> Manufacturing Data Hub

## Integrity rule
Volume produced is not itself evidence of production maturity.