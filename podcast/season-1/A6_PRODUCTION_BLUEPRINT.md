# A6 Production Blueprint — Serious Electronics & Embedded Prototype

status: PRODUCTION BLUEPRINT COMPLETE
season: Season 1 — Build the Right Thing

## Listener transformation
Before: “The circuit and firmware work on the bench.”
After: “I can distinguish bench success from controlled hardware evidence and build a traceable electronics prototype that exposes power, timing, component, programming, calibration and production-test risk.”

## Narrative hook
The demo is flawless on a dev board. The custom PCB resets under motor load, the chosen regulator is unavailable, firmware behaves differently between units, programming needs an engineer’s laptop and calibration constants live in an untracked folder. The electronics worked — the product configuration did not yet exist.

## Teaching flow
### Segment 1 — Bench success hides infrastructure
Show what dev boards/lab supplies/debuggers provide invisibly: clean power, known clocks, protection, easy reset, programming, logging and generous access.

### Segment 2 — Electronics maturity dimensions
Separate evidence for:
- architecture/function;
- power integrity/margins;
- timing/noise/signal integrity;
- thermal behavior;
- component/package/source;
- PCB/assembly;
- firmware/configuration;
- programming/update;
- calibration;
- production test;
- EMC/safety/environment where applicable.

### Segment 3 — Controlled build identity
Introduce the minimal identity:
`Unit ID → PCB/HW rev → BOM rev → firmware/build → configuration/calibration → programming method → test procedure/result → deviations/rework`.

### Segment 4 — Component maturity
Move from “electrically works” to lifecycle/availability, package/assembly compatibility, substitutes/alternates and impact assessment. Do not overclaim qualification.

### Segment 5 — Design for programming/test early
Explain why test points, boot/programming modes, fixtures, accessible states and calibration architecture are product-design decisions.

### Segment 6 — Engineering workarounds are visible debt
Bodge wires, manual reset, debug cable, firmware flags, bench-only supply and technician calibration are acceptable if owned and given expiration triggers.

### Segment 7 — Sentinel Node
Trace the evolution from dev board + USB + breakout sensor to a controlled custom PCB candidate. Identify what becomes newly testable and what new risks appear.

### Segment 8 — DEV→LVP→SVP horizon
DEV: maximize visibility and learning.
LVP: controlled BOM/FW/configuration + repeatable programming/test.
SVP: released configurations, supplier/process controls, traceability, rate-compatible test and compliance evidence.

## Listener tools
### Electronics Prototype Debt Scan
Flag:
`dev-board dependency / bodges / untracked FW / manual flashing / unknown margin / no test access / undefined identity / silent rework / unqualified substitution`.

### Controlled Build Identity
Create a one-page or spreadsheet record for every serious build.

## Misconceptions to challenge
- “Custom PCB means production intent.”
- “Component datasheet compliance proves system compliance.”
- “Firmware is separate from hardware configuration.”
- “Production test can be designed after the board is frozen.”
- “A final PASS means rework history no longer matters.”

## Standards/source backlog
IPC/JEDEC/J-STD references stay applicability- and edition-gated. No class/acceptance threshold enters script until verified.

## Closing handoff
A5 and A6 have now produced serious mechanical/electronics evidence. A7 asks the question that turns those builds into engineering proof: **what exactly are we trying to verify, under which conditions, and what decision will the result support?**
