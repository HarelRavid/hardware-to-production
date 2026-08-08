# 4.2 Process Flow & Routing

status: Researching
provenance: [GNR]

## 4.2.1 Core objects
- process flow
- routing
- operation
- step
- work center
- resource
- queue
- move
- setup
- run
- inspection
- test
- hold
- rework
- outsource step
- subcontract operation
- release gate

## 4.2.2 Operation model
Operation ID -> input state/material -> required resource -> tooling/fixture -> instruction/specification -> process parameters -> operator qualification -> expected output state -> inspection/test -> records -> next allowed operation.

## 4.2.3 Routing attributes
- sequence
- predecessor/successor
- alternate route
- rework route
- setup time
- cycle time
- transfer/queue time
- batch size
- work center
- skill requirement
- tooling
- process recipe/program revision
- inspection gate
- traceability event
- outsource supplier
- effectivity

## 4.2.4 Engineering principle
A routing is not merely a list of work centers. It is the controlled definition of allowed state transitions for the product through manufacturing.

## 4.2.5 DFM/NPI questions
1. Is the operation sequence technically necessary or inherited from prototype practice?
2. Which operations can be combined or parallelized?
3. Where should inspection occur to catch failure before additional value is added?
4. Does an outsourced operation break genealogy or configuration control?
5. Are rework paths pre-defined or invented after failure?
6. Which operations change datum, cleanliness, material condition or product configuration?
7. Is transport/queue time itself a process variable for cure, cleanliness, oxidation or shelf-life-sensitive states?

## 4.2.6 Decision objects
### D-ROUTE-001 — Select manufacturing sequence
### D-ROUTE-002 — Place inspection/test gate
### D-ROUTE-003 — Internal vs subcontract operation
### D-ROUTE-004 — Standard route vs alternate route
### D-ROUTE-005 — Define controlled rework route

## 4.2.7 Cross-links
Routing <-> MBOM
Routing <-> PFMEA
Routing <-> Control Plan
Routing <-> Work Instructions
Routing <-> Capacity/Takt
Routing <-> Traceability
Routing <-> ERP/MES

## Integrity rule
A process performed successfully during development is not automatically a valid production routing step until its inputs, outputs, controls, resources and records are defined.