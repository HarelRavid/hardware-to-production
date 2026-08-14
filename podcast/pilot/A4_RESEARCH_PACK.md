# A4 Research Pack — Choosing Prototype Technologies Without Trapping the Product

status: RESEARCH PACK OPEN
season: Season 1 — Build the Right Thing
primary_audience: Audience A — founders / early hardware development teams
secondary_audience: mechanical, electronics, embedded, test, NPI, supplier leads
lifecycle: DEV-FIRST / CROSS-STAGE
entry_point: ALTERNATIVE SERIES ENTRY FOR TEAMS ALREADY PROTOTYPING
technical_depth: foundation-practitioner
backbone_anchor: `domains/dfx-foundations/PROTOTYPE_REPRESENTATIVENESS_CROSS_PROCESS_GATE.md`

## 1. Episode promise

Teach a team to use fast prototype technologies aggressively without confusing prototype success with production evidence.

Canonical listener question:

> Which parts of what this prototype taught us can safely travel forward — and which conclusions expire when the material, process, supplier, tooling, software or production rate changes?

The episode should make prototyping faster, not more conservative. The goal is to preserve learning while preventing evidence from being carried beyond the envelope that generated it.

## 2. Navigation card

**You are here:** Architecture / POC → Integrated Prototype → Engineering Prototype

**Best for:** teams already building with dev boards, 3D-printed/CNC parts, temporary harnesses, lab fixtures or prototype suppliers.

**You should already know:** product intent and the rough function/interfaces being tested. A1/A3 are useful but not mandatory; include a concise recap.

**In this episode:** choose prototype routes according to the question being answered, then mark exactly when the shortcut expires.

**You will leave with:** Prototype Evidence Transfer Matrix + Shortcut Expiration Card.

**Prototype shortcut:** use non-production materials/processes/components when they accelerate learning and their representativeness limits are explicit.

**Shortcut expires when:** the next decision depends on a dimension the prototype does not represent.

**Next:** A5/A6 discipline-specific serious-prototype design → A7 verification → A8 configuration; later Episode 2/6/11 for production-intent/process selection.

## 3. Audience contract

### DEV takeaway
Pick the fastest prototype method that answers the current engineering question — not the method that looks most like a factory by default.

### Prototype shortcut
Dev boards, printed/machined bridge parts, hand wiring, manual assembly and temporary fixtures can be entirely legitimate.

### Shortcut expiration
A shortcut expires when decisions about product performance, reliability, compliance, manufacturing capability, supplier qualification, tooling, rate or cost depend on properties the shortcut does not reproduce.

### LVP change
Prototype routes must progressively give way to production-intent components/materials/processes or be deliberately retained as bridge manufacturing with controlled specifications, inspection and economics.

### SVP evidence
Evidence used to release serial production must come from representative configuration/process/supplier/tooling/measurement/rate conditions for the claim being made.

### Manufacturing-debt prevention
For every shortcut, record what it proves, what it does not prove, and the event that forces replacement or revalidation.

### Listener action
Take the current prototype BOM/build and tag every temporary choice with an expiration condition.

## 4. Canonical representativeness principle

Backbone rule:

> Prototype evidence transfers only to the dimensions for which the prototype is representative.

Representativeness vector:
- geometry;
- material;
- manufacturing process;
- surface/finish;
- joining/assembly;
- tooling;
- supplier;
- process variation;
- inspection/test;
- software/configuration;
- environment/load;
- production rate.

The vector is not a score where “more production-like is always better.” It is a map of which claims the prototype can and cannot support.

## 5. Core claim register — draft

| ID | Claim | Class | Priority | Status | Applicability / note |
|---|---|---|---|---|---|
| A4-C01 | Prototype evidence should transfer only to the characteristics for which the prototype is sufficiently representative. | V6 + DFX backbone | P0 | BACKBONE-SUPPORTED / external verification open | Core episode thesis. |
| A4-C02 | A prototype made by a different process may validate geometry/function while failing to validate production-process-specific failure mechanisms or economics. | V6 | P0 | SYNTHESIS / worked-example supported | Example: CNC prototype vs future casting/molding. |
| A4-C03 | “Prototype vs production” is not binary; representativeness differs by geometry, material, process, assembly, configuration, test, environment and rate. | V6 | P0 | SYNTHESIS | Canonical representativeness vector. |
| A4-C04 | A temporary component/process is acceptable in DEV when the team can state the learning objective, limitations and expiration trigger. | V6 | P1 | SYNTHESIS | Editorial lifecycle rule. |
| A4-C05 | Production-intent transition should be triggered by evidence need, risk, economics and lifecycle maturity rather than by a fixed prototype-generation number. | V6 | P1 | SYNTHESIS | Avoid universal EVT/DVT/PVT prescriptions. |
| A4-C06 | Changing material/process/supplier/tooling/software can invalidate only the claims dependent on the changed attributes, not automatically all prior evidence. | V6 + P2.02 | P0 | BACKBONE-SUPPORTED | Change/evidence-dependency rule. |
| A4-C07 | Bridge manufacturing can remain valid into LVP if quality, configuration, rate, cost and risk remain acceptable; it need not be replaced merely because a “mass-production” method exists. | V6 + P2.05 | P1 | BACKBONE-SUPPORTED | Economics/applicability must be explicit. |
| A4-C08 | A visually or dimensionally similar prototype does not automatically represent reliability, environmental performance or compliance behavior. | V6 | P0 | OPEN | Needs careful source support for any strong external claim. |
| A4-C09 | Prototype suppliers and prototype fixtures can hide process variation that appears at production volume/rate. | V6 + P2.04/P2.06 | P1 | BACKBONE-SUPPORTED | Rate/supplier evidence link. |
| A4-C10 | Teams should preserve prototype identity/configuration so later failures can be related to the exact shortcut/configuration used. | V6 + P2.02/P2.08 | P1 | BACKBONE-SUPPORTED | Cross-link A8/Atlas. |

## 6. Prototype Evidence Transfer Matrix — listener tool

For each prototype/build, list the claim being tested and score representativeness qualitatively:

| Dimension | Same/Representative? | Difference | Which claim is still valid? | Which claim is NOT valid? | Next evidence needed |
|---|---|---|---|---|---|
| Geometry | | | | | |
| Material | | | | | |
| Manufacturing process | | | | | |
| Surface/finish | | | | | |
| Joining/assembly | | | | | |
| Tooling/fixture | | | | | |
| Supplier/source | | | | | |
| Process variation | | | | | |
| Inspection/test | | | | | |
| Software/configuration | | | | | |
| Environment/load | | | | | |
| Rate/volume | | | | | |

The question is not “Is this prototype representative?”

The better question is:

> Representative enough for which claim?

## 7. Shortcut Expiration Card — listener tool

For every temporary choice:

1. **Shortcut** — what are we doing differently from the likely production route?
2. **Why now** — what learning/speed/cost advantage does it buy?
3. **What it proves** — which claims can legitimately use this evidence?
4. **What it does NOT prove** — which dimensions/failure modes are not represented?
5. **Expiration trigger** — what decision/lifecycle event makes the shortcut unacceptable?
6. **Replacement route** — what production-intent alternative is currently expected?
7. **Revalidation** — which prior claims must be repeated/rechecked after the transition?
8. **Owner/date** — who ensures the shortcut does not become invisible manufacturing debt?

## 8. Worked examples

### Example A — CNC prototype → injection-molded housing

DEV CNC housing may be excellent for:
- package geometry;
- mounting/interface fit;
- service access;
- gross structural/layout learning.

It may provide weak/no evidence for:
- mold flow/weld lines/sink/warpage;
- draft/ejection constraints;
- molded surface behavior;
- resin/process variation;
- production tooling capability;
- molded-part unit economics/rate.

Transition trigger:
When enclosure decisions depend on molded process behavior, production material, sealing under actual surface/warpage, tooling or cost/rate.

### Example B — 3D-printed enclosure → production polymer

Useful for:
- volume/shape;
- cable routing;
- ergonomics;
- mounting access.

Potentially nonrepresentative for:
- isotropy/strength;
- creep;
- sealing;
- UV/chemical resistance;
- thermal behavior;
- fire/compliance properties;
- long-term dimensional stability.

Guardrail: exact differences depend on print technology/material and production material; do not generalize one failure mechanism to every AM process.

### Example C — dev board → custom PCB

Useful for:
- sensor/processor concept;
- firmware logic;
- communications proof;
- algorithm development.

Does not automatically prove:
- final power integrity;
- PCB thermal behavior;
- EMC;
- connector architecture;
- production programming/test access;
- component lifecycle/supply risk;
- final firmware/hardware configuration behavior.

### Example D — hand-wired harness → production harness

Useful for:
- pinout/function/interface learning.

May not prove:
- strain relief;
- crimp quality;
- routing/abrasion;
- assembly repeatability;
- identification/traceability;
- production inspection/test.

### Example E — bench fixture → LVP fixture

A hand-held jig may prove sequence or access but not cycle-time distribution, ergonomic burden, mistake-proofing, maintenance or repeatability at tens/hundreds of units.

## 9. Sentinel Node example — staged evolution

### DEV-0
- dev board;
- off-the-shelf sensor module;
- printed enclosure;
- bench supply;
- jumper wiring;
- laptop logging.

Claims earned:
- sensing principle can work;
- basic firmware/communications concept works under bench conditions.

Claims NOT earned:
- production power consumption;
- final environmental sealing;
- final thermal behavior;
- final EMC/compliance;
- assembly repeatability;
- supplier/process capability;
- production rate/economics.

### DEV-1 / serious prototype
- custom PCB Rev A;
- representative connector candidate;
- more representative enclosure material/geometry;
- controlled firmware identity;
- instrumented environmental/load testing.

New evidence becomes available, but it still does not prove LVP production capability.

### Production-intent / LVP transition
- released PCB/mechanical configuration;
- approved suppliers/parts where critical;
- intended assembly method/fixture;
- controlled programming/calibration/test;
- serial genealogy;
- representative process variation and operator conditions.

The lesson is not to jump directly from DEV-0 to a factory. It is to deliberately close the representativeness gaps that matter to the next decision.

## 10. Prototype shortcut library

| Shortcut | Good DEV use | Common trap | Expiration trigger |
|---|---|---|---|
| Dev board | prove architecture/firmware | assumed equivalent to final electronics | custom PCB/power/thermal/EMC/test decisions |
| 3D print | geometry/access/iteration | assumed equivalent to final material/process | structural/environment/sealing/compliance/process evidence needed |
| CNC bridge part | geometry/function/low-volume bridge | assumed to prove casting/molding behavior | production-process-specific risks/economics matter |
| Temporary connector | bench integration | carried into prototype fleet without configuration control | reliability/sealing/current/service/supply/test depends on it |
| Hand wiring | quick interface proof | hidden variation / nonrepeatable build | multiple units, reliability, harness qualification, production assembly |
| Lab supply | isolate functional learning | hides battery/power/thermal behavior | field power architecture becomes part of claim |
| Manual inspection | learn failure modes | assumed scalable/capable | throughput, measurement system, operator variation or traceability matter |
| Prototype supplier | fast parts | quality attributed to future production source | supplier/process/rate approval matters |

## 11. Common failure modes

### Failure 1 — “It passed on the prototype”
No statement of which dimensions changed between prototype and production intent.

### Failure 2 — Production theater
A startup spends time and NRE making early prototypes look production-like without gaining useful evidence.

### Failure 3 — Shortcut fossilization
Temporary connector, adhesive, sensor, fixture or manual inspection becomes the de facto production solution because nobody recorded an expiration trigger.

### Failure 4 — Revalidate everything
The opposite error: any small change causes total retest because evidence dependencies were never mapped.

### Failure 5 — Scale blindness
A method works for three carefully built units and is assumed to support 300 units despite different operators, rate, supplier lots and variation.

### Failure 6 — Geometry-only thinking
Teams compare only shape and dimensions while material/process/surface/assembly/software/environment differ.

## 12. Decision method — REPRESENT 8

Internal listener framework:

1. **Question** — what are we trying to learn/prove?
2. **Claim** — what conclusion will we make if the prototype succeeds?
3. **Dimensions** — which representativeness dimensions matter to that claim?
4. **Differences** — where does the prototype intentionally differ?
5. **Failure modes** — which mechanisms could be hidden by those differences?
6. **Expiration** — what event makes the shortcut invalid?
7. **Next evidence** — what more representative build/test is required?
8. **Record** — how will configuration and evidence remain reconstructable?

This framework is repository synthesis, not an external industry standard.

## 13. Applicability statement

This episode applies to general multidisciplinary hardware prototyping and industrialization. It provides an evidence-transfer decision method, not universal process-specific qualification rules. Regulated/safety-critical products and specific manufacturing processes may require prescribed prototype/qualification articles, materials, test pedigrees or formal validation beyond this framework.

## 14. What this episode must NOT claim

- that prototypes should always use production materials/processes;
- that non-production prototypes are weak or unprofessional;
- that a production-intent prototype automatically proves process capability;
- that a prototype made by a different process provides zero useful evidence;
- that DEV/LVP/SVP are external standardized lifecycle labels;
- that every change requires full requalification;
- that one representativeness score can replace claim-specific engineering judgment.

## 15. Recap requirements

Standalone entry allowed.

Include a short recap of:
- requirement/claim concept from A1;
- interfaces from A3 if needed;
- DEV/LVP/SVP lens.

No listener should need all of A1–A3 to use the episode.

## 16. Recommended navigation

If listener is still developing architecture:
- A3 → A5/A6.

If listener has a working integrated prototype:
- A7 → A8 → Episode 1.

If listener is choosing the eventual manufacturing route:
- Episode 6 DFM;
- Episode 11 Process Selection;
- process-family deep dive.

Topic tracks:
- Product & Systems Engineering;
- Mechanical / Materials / Manufacturing Processes;
- Electronics / PCB / Embedded;
- DFX / Industrialization / NPI;
- Reliability / Validation / Compliance.

## 17. Research/source backlog before CLAIM SET STABLE

1. Package authoritative sources/case evidence for prototype/qualification representativeness where useful.
2. Verify process-specific examples against authoritative material/process sources before final scripting.
3. Link A4 evidence dependencies explicitly to P2.02 change-control and P2.05 process economics.
4. Decide whether one real-world case materially improves the episode or whether Sentinel examples are cleaner.
5. Technical review across mechanical + electronics + NPI perspectives.
6. Confirm the tool remains useful for both a 2-person startup and an established development team.

## 18. Pilot-test objective

A4 is intentionally different from A1.

A1 tests whether the packaging system can handle a foundation/requirements episode.
A4 tests whether it can handle:
- a highly practical decision episode;
- mixed mechanical/electronics examples;
- explicit shortcut-expiration logic;
- evidence-transfer/applicability reasoning;
- non-linear listener entry.

Pilot PASS signal:
A listener should be able to take one current prototype shortcut and answer, after the episode:

> What does this shortcut prove, what does it not prove, and exactly when must we replace or revalidate it?

## 19. Current assessment

Episode structure: STRONG
Audience fit: STRONG
Navigation entry-point fit: STRONG
Prototype-shortcut contract: STRONG
Standards burden: LOW
Quantitative burden: LOW
Backbone risk: LOW
Source verification: OPEN

Next status target:

`RESEARCH PACK OPEN → CLAIM SET STABLE`
