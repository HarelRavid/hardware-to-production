# A3 Production Blueprint — System Architecture & Interfaces

status: PRODUCTION BLUEPRINT COMPLETE
season: Season 1 — Build the Right Thing

## Listener transformation
Before: “Each subsystem owner can optimize their part and integration will follow.”
After: “I can identify the interfaces that carry risk, define an explicit contract for them and assign ownership before integration failure teaches us the hard way.”

## Narrative hook
Mechanical says the connector location is fine. Electronics says the pinout is fine. Firmware says the protocol works. Thermal says temperatures are acceptable. Yet the assembled product resets when the cable bends and cannot be serviced without removing the heatsink. Every subsystem met its local objective; the interface system failed.

## Teaching flow
### Segment 1 — Why interfaces fail more than boxes
Introduce system boundary thinking: functions are delivered across physical, electrical, thermal, fluidic, software and human interfaces.

### Segment 2 — Architecture before detailed design
Teach a lightweight decomposition:
`Product function → subsystem → interface → owner → dependency → failure consequence`.
The point is not a perfect systems model but shared assumptions.

### Segment 3 — Interface families
Use tangible examples:
- mechanical: position, datum, load, fastening, sealing;
- electrical: voltage/current, pinout, grounding, noise;
- data/software: protocol, timing, states, error handling;
- thermal: heat generation, path, allowable temperature;
- fluidic/pneumatic: pressure, flow, media compatibility;
- user/service: access, orientation, replaceability, tools;
- manufacturing/test: fixture access, test points, calibration interfaces.

### Segment 4 — Interface Contract Sheet
Each important interface records:
`Purpose → owners → definition → limits/tolerance → operating states → abnormal states → verification → change authority`.

### Segment 5 — Temporary interfaces are allowed
A DEV jumper or oversized connector is fine when its temporary nature and evidence boundary are explicit. It becomes dangerous when enclosure, supplier, compliance, tooling or verification starts depending on it.

### Segment 6 — Interaction claims
Introduce the season’s first explicit interaction lesson: component evidence does not automatically prove the system interaction. A connector rating + cable rating + enclosure rating do not by themselves prove the assembled interface under load/environment.

### Segment 7 — Sentinel Node example
Map sensor-to-PCB, PCB-to-enclosure, connector-to-seal, firmware-to-calibration and enclosure-to-service interfaces. Show one local change propagating through several owners.

### Segment 8 — DEV→LVP→SVP horizon
DEV: provisional contracts are acceptable.
LVP: interfaces that drive supplier/build/test decisions become released and verified.
SVP: change/effectivity and cross-supplier interface evidence must stay controlled.

## Listener tool
### Interface Contract Sheet
Fields:
`Interface ID → function → side A owner → side B owner → physical/electrical/data/thermal definition → limits → tolerances → states → failure modes → test → change trigger`.

### Integration Risk Review
Pick the five interfaces whose failure would require the most redesign, supplier rework, tooling change or field action.

## Misconceptions to challenge
- “The CAD assembly is the interface definition.”
- “If both components meet spec, the interface is proven.”
- “Interfaces are only connectors.”
- “Systems engineering is too heavy for startups.”
- “Ownership shared by two teams means it is covered.”

## Evidence/source backlog
Authoritative systems-engineering interface guidance; product-specific interface standards only when selected. Keep the Interface Contract Sheet as internal synthesis.

## Closing handoff
A3 establishes what must connect. A4 asks how to build prototypes that test those connections rapidly **without letting temporary prototype technology masquerade as production evidence**.
