# Pass 2.01 Worked Example — Sentinel Node

status: ACTIVE REFERENCE EXAMPLE
created_on: 2026-08-11
maps_to: Opening Arc A1–A8; Episodes 1–5, 26–31, 60
parent: P2_01_HARDWARE_READINESS_DEFINITIONS.md
provenance: engineering synthesis constrained by NASA TRL/PRR and DoD MRL evidence; fictional product

## Purpose
Provide one fictional but technically plausible hardware product that can travel through the full Hardware Evolution Ladder. The example exists to teach how evidence, configuration, manufacturing debt and production realism change over time. It is not a universal development recipe and is not intended to imply NASA/DoD lifecycle compliance.

## Product definition
**Sentinel Node** is a compact industrial condition-monitoring device mounted near rotating equipment.

Representative functions:
- tri-axial vibration sensing;
- temperature sensing;
- local processing/health indication;
- wired industrial communications;
- 24 VDC input;
- field-replaceable installation;
- operation in a dusty/wet industrial environment;
- serial number and firmware/configuration identity.

Why this product works as the recurring example:
- mechanical enclosure, sealing and mounting;
- PCB/electronics/firmware;
- connectors and cable interfaces;
- thermal/environmental requirements;
- purchased components and supplier risk;
- machining, additive prototypes, molding/casting alternatives;
- manual assembly and later fixtures/semi-automation;
- calibration/test strategy;
- traceability and field-return learning;
- enough complexity to expose cross-functional interfaces without becoming an industry-specific regulated product.

## Initial business scenario
A small team believes vibration/temperature trends can identify abnormal equipment behavior earlier than existing manual checks. Initial market uncertainty is high. The team expects:
- 1–5 early laboratory prototypes;
- 10–30 engineering/field units;
- 100–300 early customer/LVP units;
- possible later demand in the thousands per year.

These quantities are narrative assumptions only. They are deliberately not universal thresholds for DEV/LVP/SVP.

# Hardware Evolution Story

## 1. Idea
### Physical state
No product yet. A sensor concept, a rough enclosure sketch and assumptions about where/how the node will be installed.

### Question being retired
Is there a valuable technical problem and a plausible sensing concept?

### Evidence generated
- target use case;
- rough signal/noise expectations;
- initial environmental assumptions;
- initial installation and power assumptions;
- list of major unknowns.

### Evidence not yet present
- product architecture;
- validated sensor performance;
- production process;
- supplier readiness;
- cost model beyond rough order of magnitude.

### Manufacturing debt risk
Low if assumptions remain visible. High if early sketches silently become requirements.

### Exit trigger
Enough measurable requirements exist to design experiments rather than merely discuss the idea.

---

## 2. Requirements
### Physical state
Still mostly paper/model-level definition.

### Example requirements
- detect vibration over a defined frequency/amplitude range;
- temperature measurement accuracy over intended operating range;
- survive defined ambient temperature, vibration and ingress exposure;
- mount to a defined machine interface;
- operate from specified industrial supply range;
- communicate over a selected wired interface;
- allow installation/service without opening process equipment;
- preserve device/firmware identity.

### Evidence generated
- requirement IDs and rationale;
- measurable acceptance methods for critical requirements;
- assumptions separated from requirements;
- first CTQ candidates.

### Manufacturing debt exposed
A requirement such as “small as possible” without installation envelope, service clearance or connector constraints can create later redesign.

### Exit trigger
Requirements are sufficient to choose system architecture and identify the riskiest technical hypotheses.

---

## 3. Architecture
### Physical state
Block diagram and interface definition.

### Example architecture
- sensor PCB;
- MCU/communications PCB or combined PCB;
- 24 V power conditioning;
- industrial connector;
- metal/polymer enclosure;
- gasket/seal;
- mounting interface;
- firmware/configuration layer;
- programming/debug/test interface.

### Evidence generated
- power/data/load/environmental interfaces;
- subsystem ownership;
- preliminary make/buy decisions;
- preliminary verification strategy;
- critical component availability risks.

### Manufacturing debt example
Choosing a connector only because it is available on a development board may later force enclosure, cable, sealing and assembly changes.

### Exit trigger
The highest-risk technical functions can be isolated and tested through a POC.

---

## 4. POC
### Physical state
Commercial accelerometer breakout board + development MCU board + bench power supply + laptop logging software; sensors attached temporarily to a machine using adhesive/magnet.

### Question being retired
Can the sensing/algorithm concept distinguish the target machine behavior with useful signal quality?

### Evidence generated
- critical sensing function demonstrated;
- first signal-processing data;
- known test conditions;
- evidence tied to a specific prototype configuration.

### What does NOT transfer
- PCB EMC/thermal behavior;
- final connector/power behavior;
- enclosure resonance;
- final mounting transfer function;
- ingress protection;
- production calibration method;
- assembly time/yield/cost.

### Manufacturing debt warning
The POC is successful only if the team records that these production questions remain open. A successful graph is not evidence that the product can be manufactured.

### Exit trigger
The sensing principle is credible enough to justify integrated hardware.

---

## 5. Integrated Prototype
### Physical state
Custom or semi-custom PCB in a large CNC/3D-printed enclosure; temporary harnesses; debug connector exposed; manual sensor calibration; several COTS parts retained.

### Question being retired
Do the subsystems operate together, and what integration problems appear?

### Evidence generated
- electrical/firmware/mechanical integration;
- power/communications behavior;
- first thermal observations;
- interface failures discovered;
- initial configuration-controlled BOM/firmware revision.

### Example discovery
The final mounting location amplifies a structural resonance that did not exist in the bench POC. The sensor data are therefore not directly equivalent to POC data.

### Evidence invalidated/limited
The original POC algorithm evidence must be reinterpreted because mounting/enclosure dynamics changed.

### Manufacturing debt remaining
- hand-soldered rework wires;
- oversized enclosure;
- temporary connector;
- no controlled assembly torque;
- no production test fixture.

### Exit trigger
Integration is stable enough that the next prototype can intentionally represent critical product requirements rather than merely connect subsystems.

---

## 6. Engineering Prototype
### Physical state
Custom PCB revision; near-final sensing architecture; realistic enclosure size; intended connector family; representative mounting; prototype gasket; firmware versioning; dedicated engineering test fixture.

### Question being retired
Does a representative design satisfy critical engineering requirements under realistic conditions?

### Evidence generated
- requirement verification results;
- environmental/load/boundary tests;
- thermal behavior;
- connector/mounting performance;
- failure modes and design changes;
- initial DFM/DFA/DFT review.

### Example failure
Ingress test shows water reaching the PCB because gasket compression varies with manually tightened fasteners.

### Design response
- redesign sealing land;
- define fastener/torque strategy;
- add assembly access and torque verification;
- update PFMEA/control thinking.

### Evidence transfer rule
Previous dry-environment functional tests still support function, but they do not prove the redesigned sealing interface. The changed mechanical configuration requires targeted re-verification.

### Exit trigger
The design is sufficiently mature to choose production-intent materials/components/processes and freeze controlled interfaces for the next build.

---

## 7. Production-Intent Hardware
### Physical state
- production-intent PCB stack-up/components where feasible;
- controlled PCB fabrication/assembly supplier;
- intended industrial connector;
- intended enclosure material and manufacturing route or a documented bridge route;
- defined gasket specification;
- production-intent fasteners;
- serial-number label/identity;
- production test/calibration concept;
- released drawings/BOM revisions.

### Question being retired
Can hardware representative of the intended product be built and verified with controlled definition and realistic production methods?

### Evidence generated
- released configuration baseline;
- CTQs/key characteristics;
- supplier/process assumptions;
- inspection/test plan;
- preliminary work instructions;
- fixture/test-equipment requirements;
- process-risk controls.

### Bridge-manufacturing example
Enclosure is CNC-machined from production-intent material for 30 units while injection-mold tooling is not yet justified.

### Critical applicability statement
Successful CNC enclosure validation does not automatically validate a future molded enclosure. Material family may be similar while residual stress, wall geometry, draft, sink/warp, surface, tolerance distribution and sealing behavior differ. Evidence transfer must be assessed characteristic by characteristic.

### Exit trigger
Documentation, tooling, measurement, suppliers and process controls are sufficient to attempt repeatable LVP without constant designer intervention.

---

## 8. LVP — 100–300 narrative units
### Physical/production state
Manual or semi-automated assembly cells; controlled fixtures; torque tools; barcode/serial capture; production test fixture; supplier lots; formal nonconformance and change logging.

### Question being retired
Can ordinary trained production personnel repeatedly build conforming units using the defined process?

### Evidence generated
- FPY/rework/defect Pareto;
- assembly/test cycle times;
- operator learning observations;
- supplier incoming issues;
- calibration/test distributions;
- fixture problems;
- genealogy records;
- real unit-cost drivers.

### Example discovery
15% of units initially fail final communications test. Root cause is connector pin damage during manual insertion, not PCB electronics.

### Response
- improve insertion fixture/alignment;
- modify work instruction;
- add visual/poka-yoke feature;
- update PFMEA/control plan;
- verify effect on FPY.

### Lesson
The product design was functionally mature, but the production system was not yet mature. LVP generated manufacturing evidence that engineering prototypes could not provide.

### Exit trigger
Repeated builds provide enough representative evidence to validate production controls and expose dominant yield/capacity risks.

---

## 9. Production Validation
### Production state
Representative operators, suppliers, equipment, fixtures, work instructions, test systems and product configuration are used for a deliberately controlled validation build/run.

### Question being retired
Does the production system work as a system under representative conditions?

### Evidence generated
- repeated FPY/rework performance;
- process-control/reaction-plan behavior;
- measurement adequacy on CTQs;
- downtime/recovery modes;
- material/supplier flow;
- configuration/genealogy reconstruction;
- demonstrated rate for a defined duration and mix.

### Example failure
Nominal assembly cycle time suggests demand can be met, but the test station becomes the system constraint because calibration retries and data-upload latency were omitted from the original capacity model.

### Response
Improve test architecture/data flow or add parallel capacity only after understanding root cause and economics.

### Exit trigger
Dominant production risks are understood and the line can enter ramp with explicit capacity/yield/change assumptions rather than hope.

---

## 10. Ramp
### Production state
Volume rises; more supplier lots/operators/shifts appear; engineering intervention should decrease; actual cost and reliability data replace assumptions.

### Question being retired
Can the system sustain increasing output without hidden degradation in quality, delivery, cost or control?

### Evidence generated
- sustained throughput and constraint behavior;
- WIP/queue patterns;
- downtime/MTTR and maintenance demand;
- supplier delivery/quality trends;
- learning curve;
- actual cost per good unit;
- change cut-in effectiveness;
- field-return signals.

### Example change
A sensor IC becomes constrained. Alternate component is electrically compatible but has different noise/temperature characteristics.

### Change-control response
Do not treat it as a purchasing substitution only. Assess requirements, firmware calibration, verification evidence, supplier/process controls, configuration identity and field traceability before cut-in.

### Exit trigger
Rate, yield, supply, quality and change-control systems behave predictably enough for serial/commercial operation under defined demand assumptions.

---

## 11. SVP — Serial / Commercial Production
### Production state
Stable production architecture with controlled suppliers/processes/test/data; automation only where justified; field/service feedback connected to engineering and quality.

### Evidence expected
- sustained capacity under defined operating assumptions;
- process/measurement capability for critical characteristics where statistically justified;
- supplier and change-control discipline;
- maintenance/spares/recovery system;
- actual TCO/cost behavior;
- genealogy/configuration history;
- field reliability/service evidence;
- continuous-improvement loop.

### Important warning
SVP does not mean “no changes.” It means changes occur through a production system capable of understanding and controlling their impact.

# Cross-stage Evidence Ledger

| Evidence item | POC | Eng Prototype | Production Intent | LVP | Validation/Ramp |
|---|---|---|---|---|---|
| Critical sensing principle | strong initial | reconfirmed in representative hardware | monitor | monitor | field correlation |
| Final mounting transfer behavior | weak | strong | strong if unchanged | distribution emerges | sustained evidence |
| Enclosure sealing | none | prototype evidence | production-intent evidence | build variation evidence | process capability/control evidence |
| PCB functional behavior | partial/dev-board | representative | production-intent | supplier/process variation | sustained evidence |
| Assembly repeatability | none | engineering-only | preliminary | real evidence | mature evidence |
| Production test coverage | debug tests | engineering fixture | production strategy | real escapes/false failures visible | validated operational coverage |
| Unit cost | guess | estimate | supplier/process model | actual drivers appear | production economics |
| Capacity | none | none | modeled | observed cycle/constraints | sustained system evidence |
| Supplier readiness | none | samples | qualification begins | lot behavior | sustained delivery/quality |
| Genealogy | minimal config | controlled prototype | planned/implemented | unit/lot traceability | reconstruction validated |

# Manufacturing Debt Register Example

Debt is acceptable only when explicit, owned and given an expiration condition.

| Debt | Acceptable during | Expiration trigger | Risk if carried forward |
|---|---|---|---|
| Dev board | POC | architecture/custom PCB | size, EMC, supply, connectors, cost |
| Hand wiring | POC/integration | engineering prototype | variation, assembly error, serviceability |
| 3D-printed/CNC bridge enclosure | DEV/early LVP depending on need | serial route decision | false confidence in molding/casting behavior |
| Manual calibration spreadsheet | engineering prototype | LVP | data integrity, operator dependence, throughput |
| Designer-assisted assembly | engineering prototype/very early LVP | repeatability validation | hidden tribal knowledge |
| Uncontrolled supplier substitution | never acceptable once evidence depends on configuration | n/a | invalid verification/traceability |

# Podcast Teaching Pattern
At each stage ask the same six questions:
1. What are we trying to learn now?
2. What physically changed since the previous stage?
3. What evidence did this build create?
4. Which previous evidence still transfers, and which no longer does?
5. What manufacturing debt is intentionally being carried?
6. What evidence must exist before moving on?

# Standards/evidence boundary
This fictional example is a synthesis. NASA TRL supports reasoning about demonstrated technology maturity and environment. NASA PRR supports evidence categories for readiness to repeatedly produce required quantities. DoD MRL supports progression through production-relevant, pilot-line, low-rate and full-rate manufacturing environments. None of those sources mandates the Sentinel Node lifecycle, quantities, terminology or exact gates.

# Next use
- reuse selected Sentinel Node moments in Opening Arc A1–A8;
- use the full story as the spine of Episode 60;
- reuse the CNC-to-molding change in process-selection episodes;
- reuse connector damage in PFMEA/control-plan/quality episodes;
- reuse test-station bottleneck in pilot/ramp episodes;
- reuse sensor substitution in supplier/change-control episodes;
- reuse genealogy/configuration history in Manufacturing Atlas episodes.