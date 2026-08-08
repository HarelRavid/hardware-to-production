# 4.3 Tooling, Jigs & Fixtures

status: Researching
provenance: [GNR]

## Scope
Production tooling as a controlled manufacturing resource: locating, holding, guiding, assembling, processing, inspecting and mistake-proofing product throughout the routing.

## Object families
- jig
- fixture
- nest
- assembly fixture
- welding fixture
- machining fixture
- drill/template jig
- bonding/curing fixture
- test fixture
- inspection gauge/fixture
- lifting/handling fixture boundary
- soft jaws / inserts
- master/reference artifact

## Core design objects
- locating scheme
- datum interface
- constraint strategy
- clamping
- force/load path
- accessibility
- repeatability
- stiffness
- thermal behavior
- wear surfaces
- replaceable details
- adjustment
- poka-yoke
- sensors/interlocks boundary
- calibration/verification
- maintenance
- revision/effectivity

## Engineering principle
A fixture is part of the manufacturing process definition. If it establishes product location, force, geometry or acceptance, its condition and revision can directly affect product conformity.

## DFM questions
1. Which product datums should the fixture physically reference?
2. Is the part fully and repeatably constrained without overconstraint?
3. Can clamp forces deform the product or alter the process result?
4. Can the operator load the wrong variant or orientation?
5. Are critical surfaces protected from fixture damage/contamination?
6. What wears, how is wear detected, and what is replaceable?
7. Does the fixture permit required process and inspection access?
8. Is fixture variation included in the process capability model?

## Lifecycle
Requirement -> concept -> design -> analysis/review -> manufacture -> qualification -> release -> use -> periodic verification/maintenance -> repair/change -> requalification -> retirement.

## Decision objects
### D-PSE-TOOL-001 — Is dedicated tooling required?
### D-PSE-LOC-001 — Datum/location strategy
### D-PSE-CLAMP-001 — Clamping/force strategy
### D-PSE-POKA-001 — Required mistake-proofing
### D-PSE-QUAL-001 — Tool qualification and periodic verification strategy

## Traceability
Tool ID -> revision -> applicable product/routing revision -> qualification status -> calibration/verification -> maintenance -> repair/change history -> usage boundary where required.

## Cross-links
Tooling <-> routing
Tooling <-> GD&T/datums
Tooling <-> work instructions
Tooling <-> MSA
Tooling <-> ergonomics/safety
Tooling <-> automation
Tooling <-> PFMEA/control plan

No universal fixture accuracy ratio or verification interval is asserted.