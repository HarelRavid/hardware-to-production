# A4 Production Blueprint — Choosing Prototype Technologies Without Trapping the Product

status: PRODUCTION BLUEPRINT COMPLETE
season: Season 1 — Build the Right Thing

## Listener transformation
Before: “The prototype worked, so this approach is validated.”
After: “I can say exactly which claims the prototype supports, which dimensions are nonrepresentative and when the shortcut expires.”

## Narrative hook
A startup has a beautiful 3D-printed enclosure and a dev-board prototype that survives every demo. The team commits to tooling and custom electronics. Then molding changes stiffness and sealing, the final power architecture behaves differently, and production programming becomes painfully slow. The prototype was useful — the conclusions were too broad.

## Teaching flow
### Segment 1 — Prototype as a question, not a miniature product
Every prototype should exist to answer a defined question. Appearance, cost and generation number are secondary.

### Segment 2 — Prototype technology families
Discuss what can be learned from:
- dev boards/breadboards;
- 3D printing;
- CNC;
- soft/bridge tooling;
- temporary harnesses/connectors;
- manual assembly;
- lab fixtures/instruments;
- COTS components;
- outsourced prototype fabrication.

### Segment 3 — Representativeness is multidimensional
Assess, claim by claim:
`geometry → material → process → surface → interfaces → electronics/power → firmware/configuration → supplier → assembly → measurement/test → environment → rate/variation`.

### Segment 4 — REPRESENT 8
`Question → Claim → Dimensions → Differences → Failure modes → Expiration → Next evidence → Record`.
Use it to decide whether a prototype is representative enough for a specific decision.

### Segment 5 — Shortcut Expiration
Every important shortcut gets an expiration condition. Examples:
- printed enclosure expires for sealing/creep/UV claims;
- dev board expires for final power/EMC/production-test claims;
- hand assembly expires for rate/operator-variation claims;
- bridge supplier expires when supplier process attributes drive the product claim.

### Segment 6 — Bridge processes can be legitimate production
Clarify that LVP does not always require mass-production processes. A CNC or additive bridge route can remain deliberate if its economics and evidence envelope support the intended volume.

### Segment 7 — Sentinel Node
Compare printed enclosure, CNC enclosure and molded enclosure; dev board vs custom PCB; lab calibration vs production station. For every change, explicitly state what evidence transfers and what does not.

### Segment 8 — DEV→LVP→SVP horizon
DEV: fastest credible learning.
LVP: controlled bridge routes + explicit expiration.
SVP: evidence representative for released process/supplier/rate claims.

## Listener tools
### Prototype Evidence Transfer Matrix
Rows = claims; columns = current prototype vs next configuration. Mark `TRANSFERS / PARTIAL / DOES NOT TRANSFER / UNKNOWN` with reason.

### Shortcut Expiration Card
`Shortcut → why accepted now → hidden dimension → risk → expiration trigger → replacement/verification action → owner`.

## Misconceptions to challenge
- “Production-like is always better.”
- “Cheap prototype evidence is weak evidence.”
- “A high-fidelity prototype proves more about everything.”
- “Bridge manufacturing is a failure to industrialize.”
- “Once a prototype passed, retesting after process/material change is waste.”

## Evidence/source backlog
Prototype representativeness remains primarily internal synthesis supported by verification principles. Any process-specific transfer claim needs process/material evidence.

## Closing handoff
A4 teaches how to choose prototype technology. A5 and A6 now ask what a **serious mechanical** and **serious electronics/embedded** prototype must actually prove before the team moves toward controlled production.
