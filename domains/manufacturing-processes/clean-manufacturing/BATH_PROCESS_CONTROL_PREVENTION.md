# 3.13.6 Bath/Process Control & Contamination Prevention

status: Researching
provenance: [GNR]

## Process-control objects
- chemistry concentration
- pH
- conductivity boundary
- temperature
- contamination loading
- bath age
- filtration
- oil separation/skimming boundary
- rinse-water quality
- flow/agitation
- ultrasonic condition
- change-out criteria
- replenishment
- equipment cleanliness
- calibration

## Prevention hierarchy
1. eliminate contamination source where possible
2. isolate dirty and clean operations
3. prevent cross-contamination
4. control tooling/containers/handling
5. clean only what cannot reasonably be prevented
6. verify the critical clean state
7. preserve it until use

## Contamination-source objects
- machining fluids
- lubricants
- cutting debris
- abrasive media
- dirty fixtures
- gloves/hands
- compressed air/gas
- water quality
- packaging
- transport containers
- maintenance activity
- adjacent processes

## Decision objects
### D-CLEAN-CTRL-001 — Which cleaning-process parameters are CTQs/CPPs?
### D-CLEAN-BATH-001 — Bath/rinse replacement or replenishment strategy
### D-CLEAN-PREV-001 — Prevent contamination or remove it downstream?

## Production principle
A stable cleaning process requires control of the cleaning medium itself. Repeating the same recipe with a progressively contaminated bath is not necessarily the same process state.

## Cross-links
Bath control <-> SPC
Chemistry <-> EHS/waste treatment
Filtration <-> particle control
Water quality <-> residue/corrosion
Prevention <-> line layout/material flow

Quantitative bath limits remain chemistry/process-specific evidence objects.