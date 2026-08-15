# A3 Research Pack — System Architecture & Interfaces: Preventing Cross-Discipline Integration Failure

status: RESEARCH PACK OPEN
season: Season 1 — Build the Right Thing
primary_audience: Audience A — founders / early hardware development teams
secondary_audience: systems, mechanical, electronics, embedded, test, NPI
lifecycle: DEV-FIRST / CROSS-STAGE
entry_point: STANDALONE FOUNDATION FOR TEAMS FACING INTEGRATION RISK
technical_depth: foundation-practitioner

## 1. Episode promise
Teach a small hardware team to define interfaces early enough that mechanical, electrical, firmware, thermal, fluidic and user-facing decisions do not evolve as incompatible local solutions.

Canonical listener question:
> Which interfaces can break our product even when every subsystem works on its own?

## 2. Navigation card
**You are here:** Requirements/team ownership → system architecture/interfaces → prototype choices.

**Best for:** teams integrating multiple disciplines or suppliers.

**You should already know:** rough product functions and subsystem candidates. A1/A2 helpful, not mandatory.

**You will leave with:** Interface Contract Sheet + Integration Risk Review.

**Prototype shortcut:** interfaces can remain provisional while architecture is still learning.

**Shortcut expires when:** another subsystem, supplier, verification activity, tooling, enclosure, compliance or field service decision depends on the interface.

**Next:** A4 prototype technology selection → A5/A6 serious prototypes → A7 verification.

## 3. Audience contract
### DEV takeaway
Write down interface assumptions before different disciplines silently optimize around different versions of the product.

### Prototype shortcut
Temporary connectors, jumper wires, oversize envelopes and provisional protocols are acceptable when their temporary nature is explicit.

### Shortcut expiration
An interface must become controlled when dependent teams/suppliers/tests need a stable contract.

### LVP change
Interfaces need released drawings/specifications, tolerances, pinouts/protocols, service/access requirements and controlled verification.

### SVP evidence
Interface compatibility must remain controlled across supplier lots, configuration changes, manufacturing variation and field/service conditions.

### Manufacturing-debt prevention
Do not let interface definition live only in CAD screenshots, Slack messages or one engineer’s memory.

### Listener action
Pick the three interfaces most likely to create late integration failure and build an Interface Contract Sheet for each.

## 4. Interface categories
Typical interface classes:
- mechanical: envelope, datums, mounting, loads, tolerance stack;
- electrical: voltage/current, grounding, connector/pinout, isolation;
- data/communications: protocol, timing, states, update/error behavior;
- thermal: heat generation, paths, allowable temperatures, contact/interface materials;
- fluidic/pneumatic: pressure, flow, connection, cleanliness, leakage;
- optical/RF/sensing: alignment, field of view, shielding, interference;
- software/firmware/hardware state: boot/update/configuration dependencies;
- user/service: access, replacement, calibration, maintenance;
- manufacturing/test: fixture access, programming, test points, assembly datum;
- regulatory/safety boundary: isolation, guarding, creepage/clearance or other product-specific constraints where applicable.

## 5. Claim register — draft
| ID | Claim | Class | Priority | Status | Note |
|---|---|---|---|---|---|
| A3-C01 | Subsystems that work individually can still fail as a system because of incompatible interface assumptions. | V5/V6 | P0 | OPEN | General systems-engineering support needed. |
| A3-C02 | Interface definitions should state more than physical connection; behavior, tolerances, limits, states and ownership may matter to the claim. | V2/V6 | P0 | OPEN | Avoid universal formalism. |
| A3-C03 | Interface ownership should be explicit because responsibility commonly spans more than one discipline. | V6 + A2 | P0 | BACKBONE-SUPPORTED | Ownership synthesis. |
| A3-C04 | Interface verification should be planned against the failure modes/conditions that matter, not only nominal fit/function. | V2/V6 | P0 | OPEN | Link A7. |
| A3-C05 | Production-intent manufacturing/test interfaces can constrain product architecture and should enter before tooling/test lock-in. | V6 + P2.01/P2.03 | P1 | BACKBONE-SUPPORTED | DFT/DFX link. |
| A3-C06 | Changing one side of an interface can invalidate evidence on the other side when the affected claim depends on the interaction. | V6 + INTERACTION CLAIM/P2.02 | P0 | BACKBONE-SUPPORTED | Global change/evidence rule. |
| A3-C07 | A connector, API, mounting pattern or protocol name does not by itself fully define an interface contract. | V6 | P1 | SYNTHESIS | Practical guardrail. |
| A3-C08 | Interface definition maturity should increase DEV→LVP→SVP rather than being either fully formal or absent. | V6 | P1 | SYNTHESIS | Lifecycle framing. |

## 6. Listener tool — Interface Contract Sheet
For one interface capture:
| Field | Question |
|---|---|
| Interface ID/name | What boundary are we defining? |
| Side A / owner | Which subsystem/team owns this side? |
| Side B / owner | Which subsystem/team owns the other side? |
| Function | What must cross the boundary? |
| Physical definition | geometry/connector/datums/etc. |
| Electrical/data/thermal/fluid behavior | limits, protocol, states, loads, flow etc. |
| Tolerances/variation | what variation must be absorbed? |
| Environment | conditions at the interface |
| Failure modes | how can the interaction fail? |
| Verification | how will compatibility be demonstrated? |
| Configuration dependencies | which HW/FW/BOM versions matter? |
| Temporary assumptions/TBDs | what is still provisional? |
| Expiration trigger | when must the interface become controlled? |

## 7. Integration Risk Review
Ask for each critical interface:
1. What happens if both sides are “within spec” but incompatible?
2. Which assumption exists only on one side?
3. What tolerance stack/variation can accumulate?
4. What happens during startup/shutdown/fault/recovery, not only nominal operation?
5. Which environmental condition changes interaction behavior?
6. Can manufacturing/test access still work after enclosure/tooling decisions?
7. What supplier/configuration change would require re-verification?
8. Is there one accountable owner for resolving cross-boundary conflict?

## 8. Worked examples
### Mechanical/electrical connector
Mechanical team reserves envelope but not mating/service clearance; electronics team places connector at edge; enclosure closes but cable cannot be inserted after assembly.

### Thermal/electronics
Electronics meets bench function; enclosure/material/thermal path changes create junction-temperature risk under field duty cycle.

### Firmware/hardware state
Hardware revision changes sensor startup behavior; firmware assumes prior timing and passes bench testing only under warm restart.

### Production-test interface
Final enclosure design removes access to programming/test points; late fixture becomes complex or requires extra connector/process step.

## 9. Sentinel Node interface example
Critical connector interface includes:
- board-side connector geometry/location;
- mating part/supplier configuration;
- insertion direction and access;
- seating/retention characteristics;
- electrical pinout/current/signal;
- sealing contribution;
- fixture alignment;
- detection/verification of full seating;
- service/rework rules;
- approved configuration/lot/change dependencies.

Episode lesson: “uses connector X” is not an interface contract.

## 10. Common failure modes
- CAD-fit-only interface review.
- Pinout/protocol documented but startup/error states undefined.
- Each discipline assumes the other side absorbs tolerance.
- Supplier drawing becomes de facto interface spec without internal ownership.
- Test/programming/service access discovered after enclosure lock.
- Interface change treated as local ECO even though interaction evidence changes.

## 11. Applicability statement
This episode teaches general multidisciplinary interface discipline. It does not prescribe a particular systems-engineering documentation standard or regulated interface-control process. Safety-critical/regulated programs may require more formal ICDs, analyses, reviews and verification records.

## 12. What this episode must NOT claim
- every interface needs a large formal ICD in early DEV;
- interfaces are only connectors/mechanical boundaries;
- subsystem compliance proves system interaction;
- one side of an interface can unilaterally define all requirements;
- freezing interfaces early is always beneficial;
- a checklist replaces specialist analysis for safety/regulatory interfaces.

## 13. Research backlog before CLAIM SET STABLE
1. Package authoritative systems-engineering/interface-management support.
2. Cross-check A2 ownership and A7 verification boundaries.
3. Verify language around configuration-linked interaction evidence.
4. Add one real-world case only if it improves teaching.
5. Technical review: systems + mechanical + electronics/embedded.

## 14. Current assessment
Episode structure: STRONG
Audience fit: STRONG
Navigation fit: STRONG
Standards burden: LOW-MEDIUM
Quantitative burden: LOW
Backbone risk: LOW
Source verification: OPEN

Next status target:
`RESEARCH PACK OPEN → CLAIM SET STABLE`
