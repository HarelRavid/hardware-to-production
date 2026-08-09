# Section 2 — DFM / DFA / DFT Foundations — Domain Map

status: Researching
provenance: [GNR]

## Scope
Cross-process design principles that determine whether a product can be manufactured, assembled, tested, calibrated, serviced and scaled robustly before selecting or optimizing individual manufacturing processes.

## Canonical WBS
2.1 DFM principles and process-driven design
2.2 DFA and mistake prevention
2.3 DFT / calibration / traceability by design
2.4 Tolerances, GD&T and variation
2.5 Material selection for manufacturing
2.6 Reliability/service/repair considerations
2.7 Prototype-to-production representativeness
2.8 Cross-process design decision framework

## Existing foundation discovered
Substantial process-specific DFM knowledge already exists across Manufacturing Processes and Prototype Workshop, including tolerance/GD&T interaction, process sequence/datum migration, FDM design rules, CNC inspection/metrology and prototype fidelity/purpose objects. Section 2 therefore acts as the cross-process foundation and decision layer rather than duplicating every process-specific rule.

## Core design questions
- Can the required geometry/properties be produced by a capable process?
- Can the assembly be built correctly and mistake-resistant?
- Can critical requirements be measured/tested/calibrated?
- Does tolerance architecture reflect functional need and process capability?
- Is material selection compatible with manufacturing and lifecycle requirements?
- Can the product be serviced/repaired where required?
- Does prototype evidence transfer to the intended production route?
- What cross-process tradeoff gives the best whole-product outcome?

## Master decision object
### D-DFX-MASTER-001 — Is the design production-capable across manufacture, assembly, test, quality, service and scale?

Inputs:
- functional requirements/CTQs
- geometry/GD&T
- material
- candidate processes
- assembly architecture
- test/calibration strategy
- reliability/service needs
- volume/takt
- supplier/tooling capability
- prototype evidence
- cost/risk

Output:
- design risks
- process constraints
- required design changes
- assumptions/evidence
- unresolved decisions

## Integrity rule
DFM is not equivalent to making a part easy for one process if the resulting design makes assembly, test, reliability, supply chain or lifecycle performance worse.