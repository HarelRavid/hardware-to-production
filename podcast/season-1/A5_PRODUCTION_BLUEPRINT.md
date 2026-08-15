# A5 Production Blueprint — Serious Mechanical Prototype

status: PRODUCTION BLUEPRINT COMPLETE
season: Season 1 — Build the Right Thing

## Listener transformation
Before: “The mechanical prototype looks right and works, so the mechanical design is mostly done.”
After: “I can design a prototype to retire specific mechanical uncertainties in loads, interfaces, material behavior, tolerances, assembly and environment.”

## Narrative hook
The prototype closes, moves and survives the demo. On the first multi-unit build: holes do not align, the seal leaks, a hinge binds, fasteners loosen, and every unit needs hand fitting. The problem was not that the prototype was cheap; it was that it never tested the production-relevant failure mechanisms.

## Teaching flow
### Segment 1 — From shape to evidence
Separate visual/fit fidelity from engineering evidence.

### Segment 2 — Mechanical evidence dimensions
Teach the difference between evidence for:
- geometry/kinematics;
- loads/stiffness/strength;
- material behavior;
- surface/friction/wear;
- thermal expansion/distortion;
- sealing/environment;
- tolerance/interchangeability;
- joining/fastening;
- assembly/service access;
- manufacturing process.

### Segment 3 — Hand fitting is data
Manual filing, drilling, bending, shimming or selective assembly can be legitimate in DEV, but every rescue is a signal about uncertainty. Capture it instead of hiding it.

### Segment 4 — Interfaces and tolerance stacks
Show why one favorable stack can make a prototype work. Introduce the need to identify functional dimensions and CTQs before full production drawings exist.

### Segment 5 — Material/process substitution
Printed polymer, machined aluminum, sheet metal and molded polymer can reproduce geometry while changing stiffness, creep, sealing, surface, fatigue or thermal behavior. Ask what evidence transfers.

### Segment 6 — Serious next-build design
Choose the build based on the highest-consequence uncertainty. Do not make every feature production-intent at once.

### Segment 7 — Sentinel Node
Use enclosure, gasket, mounting boss and connector opening examples. Show how a printed prototype proves access/fit but not necessarily gasket compression distribution, molded warpage or long-term outdoor performance.

### Segment 8 — DEV→LVP→SVP horizon
DEV: expose mechanisms and interfaces quickly.
LVP: increase interchangeability, controlled materials/processes and assembly evidence.
SVP: link released tolerances/material/process/supplier and measurement capability.

## Listener tools
### Mechanical Prototype Evidence Map
`Claim → failure mechanism → representative dimensions → prototype route → nonrepresentative dimensions → observed rescue/rework → next evidence`.

### Mechanical Build Debrief
After every build record:
- what required touch labor beyond plan;
- what was shimmed/adjusted/selected;
- what fit only in one assembly order;
- what could not be measured;
- which feature drove rework.

## Misconceptions to challenge
- “Machined metal is always more serious than printed plastic.”
- “A tight prototype means tolerances are fine.”
- “Hand fitting is just craftsmanship, not engineering data.”
- “Production intent means final process everywhere.”
- “Material change is only a strength question.”

## Standards/source backlog
GPS/GD&T and material/process claims stay source-gated. No numerical tolerance rule enters the script without exact process/standard applicability.

## Closing handoff
A5 leaves the listener able to build mechanical evidence deliberately. A6 applies the same discipline to electronics and embedded hardware, where dev boards, bench supplies and debug access hide a different class of production debt.
