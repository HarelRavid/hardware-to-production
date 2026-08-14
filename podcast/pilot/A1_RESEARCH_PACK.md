# A1 Research Pack — From an Idea to Engineering Requirements

status: CLAIM SET STABLE
season: Season 1 — Build the Right Thing
primary_audience: Audience A — founders / early hardware development teams
secondary_audience: systems, mechanical, electronics, embedded, test, NPI leads
lifecycle: DEV-FIRST / CROSS-STAGE
entry_point: PRIMARY SERIES ENTRY
technical_depth: foundation
source_note: podcast/pilot/A1_SOURCE_VERIFICATION_NOTE.md

## 1. Episode promise

Help a hardware team turn an idea into a small, controlled set of engineering requirements that is useful enough to guide architecture and prototyping without pretending that every production detail is already known.

The episode should prevent two opposite mistakes:

1. building immediately from an idea with no explicit constraints; and
2. attempting to fully specify an immature product before learning has begun.

Canonical listener question:

> What do we need to decide, write down and test before CAD, PCB and prototype work become expensive to unwind?

## 2. Navigation card

**You are here:** Idea → Requirements → Architecture

**Best for:** founder, first hardware engineer, small multidisciplinary team, engineering manager starting a physical-product program.

**You should already know:** nothing beyond the problem/product idea.

**In this episode:** convert intent and assumptions into a minimum useful requirement baseline.

**You will leave with:** a Minimum Useful Requirements Sheet + Requirement Quality Check.

**Prototype shortcut:** incomplete requirements are acceptable when explicitly marked as assumptions/TBDs and paired with a learning plan.

**Shortcut expires when:** a requirement begins controlling interfaces, safety/compliance, supplier selection, irreversible tooling, qualification, production acceptance or field behavior.

**Next:** A2 Hardware Team Map → A3 System Architecture & Interfaces → A4 Prototype Technologies.

## 3. Audience contract

### DEV takeaway
Write down enough product truth to stop disciplines from solving different versions of the product.

### Prototype shortcut
Use bounded assumptions, target ranges and TBDs where evidence does not yet justify a fixed value.

### Shortcut expiration
An assumption cannot remain informal when another discipline, supplier, verification activity or production-control decision depends on it.

### LVP change
Requirements must become testable, configuration-linked and strong enough to drive CTQs, supplier specifications, inspection/test limits and controlled change.

### SVP evidence
Critical requirements must be supported by controlled verification/validation and linked to production/process evidence where manufacturing influences compliance or performance.

### Manufacturing-debt prevention
Capture interfaces, environments, expected use, safety/regulatory constraints, service assumptions and likely production-critical characteristics before prototype choices harden around unstated assumptions.

### Listener action
Create a one-page Minimum Useful Requirements Sheet before the next major prototype iteration.

## 4. Core conceptual chain

Need / user problem
→ intended function
→ operating context
→ constraints
→ interfaces
→ measurable requirement
→ verification intent
→ architecture/design decision
→ prototype learning
→ requirement refinement
→ controlled baseline

Requirements are not a one-time waterfall handoff. They mature with evidence, but changes should remain visible once they start driving dependent engineering decisions.

## 5. Core claim register — stable set

| ID | Claim | Class | Priority | Evidence state | Applicability / note |
|---|---|---|---|---|---|
| A1-C01 | A product idea is not yet an engineering requirement set; teams need explicit functional, interface and constraint statements before detailed design becomes coordinated. | V6 supported by V2/V5 | P0 | SUPPORTED / synthesis boundary explicit | General systems-engineering principle; not presented as a universal normative statement. |
| A1-C02 | Useful engineering requirements should be clear enough to support verification or an explicit method of determining satisfaction. | V2/V6 | P0 | STRONGLY SUPPORTED | NASA requirements-verification guidance supports planning verification while developing requirements. |
| A1-C03 | Requirements and assumptions should be traceable to the need/constraint they serve and to downstream verification/design evidence where practical. | V2/V6 | P1 | PARTIALLY SUPPORTED | NASA supports requirement identity/source/verification linkage; broader traceability remains to be packaged if used strongly. |
| A1-C04 | Interfaces deserve explicit ownership because multidisciplinary failures often arise from incompatible assumptions across subsystem boundaries. | V5/V6 | P1 | OPEN | Narrative/general engineering synthesis; source support can be added before script ready. |
| A1-C05 | A prototype-stage requirement may legitimately remain a range, target or TBD when uncertainty is acknowledged and a learning activity is defined. | V6 | P1 | SYNTHESIS | Internal lifecycle guidance, not an external standard requirement. |
| A1-C06 | Safety, regulatory and environmental constraints should be surfaced early because they can constrain architecture, materials, electrical design, enclosure, testing and manufacturing choices. | V2/V6 | P0 | OPEN / scoped | Do not imply specific regulation without product/jurisdiction. |
| A1-C07 | Not every requirement should become a production CTQ; CTQs are the subset where variation/control matters materially to product/process outcomes. | V6 + P2.03 | P0 | BACKBONE-SUPPORTED | Preview only; canonical quality language comes from P2.03. |
| A1-C08 | Once a requirement controls supplier specifications, tooling, acceptance criteria or compliance evidence, changing it becomes a configuration/change-control event rather than casual prototype editing. | V6 + P2.02 | P0 | BACKBONE-SUPPORTED | Configuration/change principle inherited from P2.02. |
| A1-C09 | Development verification and production acceptance testing are different evidence problems even when they measure related characteristics. | V6 + P2.03 | P1 | PARTIALLY SUPPORTED | NASA V&V supports verification planning; production-acceptance distinction remains lifecycle synthesis. |
| A1-C10 | Requirements maturity should increase from DEV to LVP to SVP rather than being treated as either “none” or “fully frozen.” | V6 | P1 | SYNTHESIS | Hardware Evolution Ladder application. |

## 6. Source package status

See `podcast/pilot/A1_SOURCE_VERIFICATION_NOTE.md`.

Primary sources located:
- NASA Systems Engineering Handbook / Requirements Verification Matrix and V&V planning guidance;
- ISO/IEC/IEEE 29148:2018 official ISO record;
- ISO/IEC/IEEE DIS 29148 Edition 3 revision-watch record.

Standards guardrail:
- ISO/IEC/IEEE 29148:2018 remains the current published edition in the checked ISO record and was confirmed in 2024;
- an Edition 3 DIS is under development in 2026;
- the draft must not be substituted for the current published standard;
- exact normative claims remain blocked until the licensed/full text and clause support are available.

## 7. Requirement taxonomy for the episode

The listener should learn a practical taxonomy, not an encyclopedic standards taxonomy.

### A. Functional
What must the product do?

Examples:
- detect an event;
- move a load;
- maintain a temperature;
- communicate data;
- deliver a specified output.

### B. Performance
How well, how fast, how accurately, how much?

Examples:
- force;
- speed;
- accuracy;
- capacity;
- response time;
- power consumption;
- throughput where product-level relevant.

### C. Interface
What must connect or interact with what?

Examples:
- mechanical envelope;
- mounting points;
- connectors;
- voltage/current;
- communications protocol;
- fluid connection;
- user/service interfaces.

### D. Environmental / operating context
Where and under what conditions must it work or survive?

Examples:
- temperature;
- humidity;
- vibration/shock;
- dust/water;
- chemicals;
- UV/corrosion;
- indoor/outdoor;
- storage/transport.

### E. Safety / regulatory / compliance constraints
What hazards or regulated boundaries may alter architecture/design/test choices?

Do not teach generic compliance as if one standard applies to all products.

### F. Reliability / life / maintenance
How long, how often, and under what service model?

Examples:
- useful life target;
- duty cycle;
- maintenance interval;
- replaceable parts;
- permitted downtime.

### G. Manufacturing / supply constraints
What production realities materially constrain design?

Examples:
- intended volume range;
- preferred/forbidden processes;
- critical supplier dependency;
- target production geography where material;
- assembly/service accessibility;
- calibration/test requirements.

These are practical constraints that should become visible early if they affect architecture; they are not all formal “manufacturing requirements” in every methodology.

## 8. The Minimum Useful Requirements Sheet — listener tool

One page / one controlled document containing:

### Product intent
- Who is the user/customer?
- What problem is being solved?
- What is explicitly out of scope?

### Top functions
- 5–15 essential functions/outcomes.

### Critical measurable targets
For each critical function:
- target/value/range;
- unit;
- tolerance if known;
- current evidence level;
- verification idea.

### Interfaces
- mechanical;
- electrical/power;
- data/communications;
- thermal/fluid where relevant;
- user/service.

### Operating envelope
- use environment;
- storage/transport;
- duty cycle;
- abuse/misuse conditions worth considering.

### Safety / compliance watchlist
- known hazards;
- markets/jurisdictions;
- candidate regulatory/standards families requiring later applicability review.

### Production horizon
- DEV quantity expectation;
- LVP expectation;
- plausible SVP scale;
- process/supplier assumptions that may change with volume.

### Assumptions / TBD register
For each TBD:
- current assumption;
- why unknown;
- what experiment/decision resolves it;
- owner;
- latest date/lifecycle transition by which it must be resolved.

## 9. Requirement Quality Check — listener tool

For every requirement/constraint ask:

1. **WHY** — what need, hazard, interface or business constraint drives it?
2. **WHAT** — what observable outcome is actually required?
3. **HOW MUCH** — is a value/range/unit needed?
4. **WHERE/WHEN** — under which operating conditions?
5. **WHO/WHAT INTERFACE** — which subsystem/team/supplier depends on it?
6. **VERIFY** — how could we know it is satisfied?
7. **MATURITY** — known requirement, target, assumption or TBD?
8. **CHANGE IMPACT** — who must know if it changes?

This is an internal listener framework unless later mapped to a named external method.

## 10. Sentinel Node worked example — requirement evolution

Illustrative product: Sentinel Node.

### Weak idea statement
“Build a rugged wireless sensor node for industrial use.”

Useful for product intent, insufficient for coordinated engineering.

### Early DEV requirement set — illustrative

- Product shall detect the selected physical condition within an initial target accuracy range [TBD after sensor characterization].
- Product shall operate from the selected supply/battery architecture for the target duty profile [initial assumption].
- Enclosure shall fit within the target installation envelope.
- Product shall communicate using the selected interface candidate within the intended installation environment.
- Product shall expose programming/debug/test access during development.
- Product shall survive the initial environmental test envelope chosen for the target use case.

Important: these are pedagogical examples, not claims that this is sufficient specification for a real industrial sensor.

### What happens next
Sensor characterization may refine accuracy.
Thermal testing may alter enclosure/power architecture.
Connector selection may create sealing/service constraints.
EMC/safety/regulatory investigation may add architecture constraints.
LVP test strategy may convert one product-performance characteristic into a production CTQ/test requirement.

The requirement record therefore matures with evidence rather than pretending all numbers were known on day one.

## 11. Prototype-shortcut expiration examples

| DEV shortcut | Initially acceptable because | Expires when |
|---|---|---|
| “Use available 12 V lab supply” | proving core function | power architecture, safety, thermal behavior or field supply becomes design-critical |
| “3D-print enclosure” | learn geometry/access | sealing, strength, thermal, UV/chemical exposure or production process must be represented |
| “Any equivalent connector” | bench integration | mating compatibility, sealing, current, lifecycle, supply or production test depends on connector configuration |
| “Sensor accuracy TBD” | sensor principle still being characterized | architecture/control decision, customer claim, calibration or acceptance test depends on accuracy |
| “Firmware build on engineer laptop” | very early bench work | multiple units/tests need configuration identity and reproducibility |

## 12. Common failure modes to cover narratively

### Failure 1 — Starting CAD from a sentence
Each discipline invents missing requirements locally; integration conflict appears late.

### Failure 2 — Writing requirements as design solutions
Example: “use motor X” when the actual requirement is torque/speed/environment/interface. Sometimes a component really is mandated; the episode teaches the distinction.

### Failure 3 — False precision
A startup writes a tolerance or lifetime because a spreadsheet wants a number, not because evidence or customer need supports it.

### Failure 4 — Invisible assumptions
The most dangerous requirement is often the one nobody wrote because “everyone knew.”

### Failure 5 — No verification intent
A requirement reaches later validation before anyone asks how it will be measured.

### Failure 6 — Compliance discovered after architecture lock
A regulatory/safety/environment constraint forces enclosure, isolation, spacing, materials, firmware behavior or test architecture to change late.

## 13. Applicability statement

This episode teaches a lightweight requirements discipline for multidisciplinary hardware development from early DEV through production maturity. It does not prescribe a universal formal requirements-management process, certification scheme or specific standard for every hardware product. Regulated industries, safety-critical systems and contractual programs may require substantially more formal methods and records.

## 14. What this episode must NOT claim

- that every startup needs enterprise requirements software;
- that requirements should be fully frozen before prototyping;
- that every requirement becomes a CTQ;
- that ISO/IEC/IEEE 29148 automatically applies contractually to all hardware;
- that manufacturing concerns should fully determine early product architecture;
- that one generic checklist replaces industry-specific safety/regulatory analysis.

## 15. Recap / prerequisite burden

No prerequisite episode required.

Definitions introduced briefly:
- requirement;
- assumption/TBD;
- interface;
- verification;
- CTQ preview;
- configuration/change preview.

Do not fully teach CTQ, verification hierarchy or configuration management here. Point forward to A7/A8 and quality episodes.

## 16. Recommended next navigation

Primary:
- A2 — Hardware Team Map
- A3 — System Architecture and Interfaces

For a team already prototyping:
- A4 — Choosing Prototype Technologies Without Trapping the Product
- A8 — Configuration Management from Prototype #1

Related tracks:
- Product & Systems Engineering
- DFX / Industrialization / NPI
- Reliability / Validation / Compliance

## 17. Remaining backlog before EVIDENCE VERIFIED

1. Acquire/licence full ISO/IEC/IEEE 29148 if clause-level normative claims will appear in script.
2. Add exact support references for any P0 29148 claim used authoritatively.
3. Add interface-focused support if A1-C04 becomes a strong causal claim.
4. Add product-neutral safety/regulatory support only if the script makes a consequential claim beyond scoped engineering guidance.
5. Reuse verified P2.02/P2.03 evidence for configuration/CTQ boundaries.
6. Technical systems-engineering review.

## 18. Current assessment

Episode structure: STRONG
Audience fit: STRONG
Navigation entry-point fit: STRONG
Standards burden: LOW–MEDIUM
Quantitative burden: LOW
Backbone risk: LOW
Claim-set stability: PASS
Source verification: STARTED

Current maturity:

`CLAIM SET STABLE`

Next target:

`EVIDENCE VERIFIED`
