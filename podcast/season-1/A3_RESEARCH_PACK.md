# A3 Research Pack — System Architecture & Interfaces: Preventing Cross-Discipline Integration Failure

status: CLAIM SET STABLE
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

**Shortcut expires when:** another subsystem, supplier, verification activity, tooling, enclosure, compliance or field-service decision depends on the interface.

**Next:** A4 prototype technology selection → A5/A6 serious prototypes → A7 verification.

## 3. Audience contract
### DEV takeaway
Write down interface assumptions before different disciplines silently optimize around different versions of the product.

### Prototype shortcut
Temporary connectors, jumper wires, oversize envelopes and provisional protocols are acceptable when their temporary nature is explicit.

### Shortcut expiration
An interface must become controlled when dependent teams/suppliers/tests need a stable contract.

### LVP change
Interfaces need released drawings/specifications, tolerances, pinouts/protocols, service/access requirements and controlled verification appropriate to the product.

### SVP evidence
Interface compatibility must remain controlled across supplier lots, configuration changes, manufacturing variation and field/service conditions.

### Manufacturing-debt prevention
Do not let interface definition live only in CAD screenshots, chat messages or one engineer’s memory.

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
- regulatory/safety boundary: product-specific constraints where applicable.

This taxonomy is an internal teaching aid, not a normative external classification.

## 5. Stable claim register
| ID | Claim | Class | Priority | Status | Publication note |
|---|---|---|---|---|---|
| A3-C01 | Subsystems that function individually can still fail at system level because the interaction/interface conditions were not compatible or demonstrated. | V6 + V2 | P0 | CLAIM STABLE / SOURCE VERIFICATION OPEN | General systems-engineering support required. |
| A3-C02 | Useful interface definition can include physical, functional, behavioral, state, tolerance, environmental and ownership information depending on the interaction claim. | V6 + V2 | P0 | CLAIM STABLE / SOURCE VERIFICATION OPEN | Do not imply one universal ICD format. |
| A3-C03 | Cross-boundary ownership should be explicit because an interface normally depends on at least two sides and often several disciplines. | V6 + A2 | P0 | SYNTHESIS STABLE | A2 owns responsibility mapping. |
| A3-C04 | Interface verification should address relevant failure conditions and variation, not only nominal fit/function. | V6 + V2 | P0 | CLAIM STABLE / SOURCE VERIFICATION OPEN | A7 owns verification-planning depth. |
| A3-C05 | Manufacturing/test interfaces can constrain architecture and should be considered before enclosure/tooling/test access is irreversibly locked. | V6 + P2.01/P2.03 | P1 | BACKBONE-SUPPORTED / STABLE | Product-specific timing. |
| A3-C06 | A change on one side of an interface can invalidate interaction evidence when the changed dependency contributes to the demonstrated claim. | V6 + INTERACTION CLAIM/P2.02 | P0 | BACKBONE-SUPPORTED / STABLE | Preserve evidence-impact logic. |
| A3-C07 | Naming a connector, API, mounting pattern or protocol does not necessarily define all conditions needed to prove interface compatibility. | V6 | P1 | SYNTHESIS STABLE | Practical guardrail. |
| A3-C08 | Interface maturity can increase progressively DEV→LVP→SVP; early teams need visible assumptions, not maximal documentation from day one. | V6 | P1 | SYNTHESIS STABLE | Lifecycle framing. |

Core claims: 8. Open P0 source families: systems/interface management + verification support.

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
Final enclosure design removes access to programming/test points; late fixture becomes complex or requires an extra connector/process step.

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

## 10. Boundary with adjacent episodes
- A2 owns **who owns/reviews the responsibility**.
- A3 owns **what the interface contract must make visible**.
- A4 owns **whether a prototype implementation represents the eventual claim**.
- A7 owns **how the claim will be verified**.
- A8 owns **how interface/configuration identity and changes remain controlled**.

This boundary prevents Season 1 from repeating the same systems-engineering material under different titles.

## 11. Common failure modes
- CAD-fit-only interface review.
- Pinout/protocol documented but startup/error states undefined.
- Each discipline assumes the other side absorbs tolerance.
- Supplier drawing becomes de facto interface spec without internal ownership.
- Test/programming/service access discovered after enclosure lock.
- Interface change treated as local ECO even though interaction evidence changes.

## 12. Applicability statement
This episode teaches general multidisciplinary interface discipline. It does not prescribe a particular systems-engineering documentation standard or regulated interface-control process. Safety-critical/regulated programs may require more formal ICDs, analyses, reviews and verification records.

## 13. What this episode must NOT claim
- every interface needs a large formal ICD in early DEV;
- interfaces are only connectors/mechanical boundaries;
- subsystem compliance proves system interaction;
- one side of an interface can unilaterally define all requirements;
- freezing interfaces early is always beneficial;
- a checklist replaces specialist analysis for safety/regulatory interfaces.

## 14. Evidence backlog after claim stabilization
Before EVIDENCE VERIFIED:
1. Attach authoritative systems-engineering/interface-management support.
2. Attach authoritative support for planning verification against interface requirements/conditions.
3. Verify any product-specific safety/regulatory examples only when their applicability is explicit.
4. Technical review: systems + mechanical + electronics/embedded.
5. Real-world case remains optional; do not add one merely to satisfy a format.

## 15. Current assessment
Episode structure: STRONG
Audience fit: STRONG
Navigation fit: STRONG
Standards burden: LOW-MEDIUM
Quantitative burden: LOW
Backbone risk: LOW
Claim set: STABLE
Source verification: CONTROLLED BACKLOG

Next status target:
`CLAIM SET STABLE → EVIDENCE VERIFIED`
