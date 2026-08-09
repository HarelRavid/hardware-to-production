# 2.4–2.6 Tolerances, Materials, Reliability & Service by Design

status: Researching
provenance: [GNR]

## Tolerance / GD&T / variation architecture
Functional requirement -> datum/reference strategy -> tolerance allocation -> process capability -> measurement capability -> assembly stack -> functional verification.

### Variation objects
- nominal
- tolerance/specification
- datum/reference
- geometric control
- process distribution
- measurement variation
- assembly stack
- thermal/environmental variation
- wear/life variation

### Principle
Tighter tolerance is not automatically better design. Tolerance should protect function while remaining compatible with process and measurement capability and whole-assembly variation.

## Material selection for manufacturing
Material selection must consider both product performance and the manufacturing route.

### Dimensions
- mechanical/thermal/electrical/chemical requirements
- stock/product form availability
- machinability/formability/castability/moldability/joinability
- heat-treatment response
- coating/surface compatibility
- dimensional stability
- contamination/cleanliness
- supplier maturity
- inspection/certification
- scrap/recycling
- cost/lead time

### Principle
A material can be functionally excellent and industrially poor if it requires immature supply, unstable processing, excessive inspection or incompatible joining/finishing.

## Reliability / service / repair by design
### Objects
- mission profile
- failure mechanism
- wear item
- access
- replaceable unit
- connector/fastener
- inspection point
- calibration/service interface
- repair process
- service tool
- field traceability

### Questions
- Which parts are expected to wear or fail during useful life?
- Can they be inspected/replaced without damaging unrelated components?
- Does service disturb safety-critical alignment/calibration/sealing?
- Is repair economically and technically justified versus replacement?
- Can repaired configuration and replaced serial components be traced?

## Decision objects
### D-DFX-TOL-001 — Functional tolerance allocation and process capability tradeoff
### D-DFX-MAT-001 — Material/process/supply-chain selection
### D-DFX-SVC-001 — Serviceability/repairability architecture

## Integrity rules
- Do not use drawing tolerance as a substitute for functional reasoning.
- Do not select material independently of the intended manufacturing chain.
- Do not claim serviceability merely because a product can physically be disassembled.