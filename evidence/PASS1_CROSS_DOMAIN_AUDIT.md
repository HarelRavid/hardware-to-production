# Pass 1 Cross-Domain Audit — A0–A8

status: COMPLETE — PASS 2 PRIORITY QUEUE DEFINED
version: 1.0
date: 2026-08-11
scope: evidence/foundations A0–A8 + PODCAST_MAP Opening Arc and Episodes 1–60

## Purpose
Audit the completed breadth campaign before deep research. The audit prevents duplicated research, assigns canonical ownership for cross-domain claims, identifies conceptual gaps and creates the first Pass-2 execution queue.

## Executive result
Pass 1 breadth is coherent enough to proceed to Pass 2. No architecture-breaking contradiction was identified across A0–A8.

The main risk is not contradiction but duplicated ownership: configuration/change, validation/readiness, measurement/quality, supplier/process capability, traceability and lifecycle economics appear in multiple packages. Pass 2 must deepen these claims once under a canonical owner and reuse them elsewhere.

A second gap exists in Episodes 53–60: the synthesis/case-study arc is mapped to WBS Section 10 but does not yet have a dedicated evidence/case-study package. Create A9 before declaring the podcast research architecture complete.

## Canonical ownership map

### Product maturity, configuration and readiness
Canonical owner: A1 Product Readiness / NPI.
Reused by: A0, A2, A5, A6, A7, A8.
Rule: definitions of design maturity, production intent, configuration baselines and readiness gates live in A1. Other packages add domain-specific evidence only.

### Early prototype representativeness and manufacturing debt
Canonical owner: A0 Early Hardware Development.
Reused by: A1, A2, A3, A5.
Rule: the DEV→LVP→SVP editorial interpretation is owned here; process-specific transferability belongs to the relevant process package.

### DFM/DFA/DFT
Canonical owner: A2.
Reused by: A0, A1, A3, A4, A5.
Rule: design-method claims live in A2; process-selection economics remain A3 and quality-control consequences remain A4.

### Process selection, bridge manufacturing and lifecycle economics
Canonical owner: A3.
Reused by: A0, A2, A5, A6, A7.
Rule: NRE/variable-cost/break-even/cost-per-good-part and bridge-route logic live in A3. Supplier TCO adds supplier-specific evidence in A6; automation TCO adds automation-specific evidence in A7.

### PFMEA, control plans, MSA, SPC and capability
Canonical owner: A4.
Reused by: A1, A5, A6, A7.
Rule: statistical/measurement definitions and core quality logic live only in A4. Other packages reference them and add application evidence.

### Pilot/PVT/ramp/rate/yield/capacity
Canonical owner: A5.
Reused by: A1, A4, A6, A7.
Rule: definitions of production validation, sustainable rate, yield and capacity live in A5. Supplier run-at-rate evidence in A6 maps back here.

### Supplier qualification and supplier change
Canonical owner: A6.
Reused by: A3, A4, A5.
Rule: supplier selection/qualification, FAI/PPAP boundary, sub-tier dependency and supplier change control live in A6.

### Automation qualification, OEE and machinery/cell integration
Canonical owner: A7.
Reused by: A3, A4, A5, A8.
Rule: FAT/SAT/SIT, automation TCO, OEE guardrails, machinery/robot integration and maintenance/recovery live in A7.

### Manufacturing semantic identity, genealogy, provenance and OT/ICS integration
Canonical owner: A8.
Reused by: A1, A4, A5, A6, A7.
Rule: semantic IDs, source-of-record boundaries, temporal/effectivity truth, genealogy/provenance and read/write OT authority live in A8.

## Cross-domain consistency findings
1. **Validation language:** A1/A5/A6/A7 all discuss validation. No contradiction, but Pass 2 must explicitly separate design/product validation, production validation, supplier qualification and equipment/automation acceptance.
2. **Capability language:** A4 process capability, A5 production capacity and A6 supplier capability are different concepts. Editorial material must never use “capability” without context.
3. **Traceability language:** A4 measurement traceability and A8 product/data genealogy/provenance are distinct. NIST metrological traceability applies to measurement results; do not use it as a synonym for product genealogy.
4. **Change control:** A1 owns configuration/change governance; A6 owns supplier-change consequences; A7 owns automation requalification; A8 owns historical/effectivity reconstruction. These should link rather than duplicate.
5. **Economics:** A3 owns generic lifecycle/process economics; A6/A7 only specialize supplier and automation economics.
6. **Evidence transfer:** A0/A3/A5 consistently support the principle that evidence generated on a prototype/bridge route may not transfer completely after process/configuration changes.
7. **Standards applicability:** no package should say “compliant with ISO/ISA/NIST” at family level. Standard part, edition, role, scope and applicability must be explicit in Pass 2.

## Conceptual coverage audit — Opening Arc + Episodes 1–52
Broad coverage is sufficient to begin Pass 2, with these controlled gaps:

### Gap G1 — Electronics manufacturing depth
Opening A6 already flags this. PCB fabrication/assembly, IPC workmanship/acceptability, electronics DFM/DFT, component lifecycle, harness production and electronics production test need deeper evidence before electronics-heavy episodes are Podcast Ready.
Action: create a focused Pass-2 electronics manufacturing subpackage rather than changing the WBS immediately.

### Gap G2 — Regulatory/product-safety applicability
The map mentions regulatory/safety requirements, but cross-industry compliance strategy is not yet a dedicated breadth package.
Action: handle by episode/product context; do not create a universal “all regulations” package. Build applicability maps for selected case products.

### Gap G3 — Reliability engineering bridge
Reliability appears across development, validation and production but needs a clearer bridge between engineering reliability evidence and manufacturing controls.
Action: Pass-2 worked example linking failure mechanism → verification → PFMEA/control → field/reliability feedback.

### Gap G4 — Serviceability/repair/field feedback
Lifecycle support is present in the ladder but weakly represented in A0–A8.
Action: add field-return/FRACAS/service feedback to a synthesis case and evaluate whether a future controlled WBS enrichment is warranted.

## Episodes 53–60 audit
Episodes 53–60 require evidence that is qualitatively different from foundational source maps: well-documented cases, counterfactual discipline and cross-industry transferability.

Create **A9 — Case Studies & Cross-Industry Synthesis** covering:
- failed hardware launches and industrialization failures;
- successful industrialization patterns;
- startup speed/manufacturing-debt cases;
- automotive lessons and limits of transfer;
- medical-device lessons and limits of transfer;
- aerospace lessons and limits of transfer;
- industrial-equipment lessons;
- one end-to-end fictional/composite decision story for Episode 60 built only from evidence-backed principles.

Case-study rule: distinguish documented facts, attributed interpretation and our synthesis. Avoid folklore cases unless primary/credible evidence exists.

## Pass-2 priority queue
Priority is based on podcast sequence × engineering consequence × evidence weakness × cross-domain leverage.

### P0 — Foundational definitions and gates
1. A0/A1: lifecycle/readiness definitions and Hardware Evolution Ladder evidence mapping.
2. A1: configuration baseline/change-control worked example.
3. A4: PFMEA→Control Plan→MSA→SPC→Capability worked example.
4. A5: Pilot/PVT/run-at-rate/capacity exit-criteria worked example.

### P1 — High-leverage decision frameworks
5. A3: quantitative process-selection and bridge-manufacturing economics example.
6. A6: supplier qualification ladder with FAI/PPAP/run-at-rate/change-control applicability.
7. A7: automation ROI/TCO + FAT/SAT/production qualification example.
8. A8: ISA-95/OPC UA/IEC 62443 applicability + genealogy/effectivity/write-back reference architecture.

### P1 — Opening Arc gap closure
9. Electronics manufacturing evidence package for Opening A6 and downstream DFT/production-test episodes.
10. Reliability-to-manufacturing-control worked example.

### P2 — Case-study architecture
11. A9 case-study source map and case-selection rubric.
12. Cross-industry applicability matrices for automotive, medical device, aerospace and industrial equipment.
13. Episode 60 end-to-end decision story.

### P2 — Implementation validation
14. Integrated Manufacturing Atlas mock/reference dataset.
15. Conflicting system-of-record and historical-effectivity reconstruction scenario.
16. Controlled read-only analytics versus operational write-back scenario.

## Pass-2 execution rule
For each priority item:
1. state the exact claim/decision question;
2. identify canonical owner;
3. extract strongest primary/authoritative evidence;
4. capture standard edition/part/clause where legally/copyright-permissible and available;
5. create Applicability Statement;
6. capture conflicts/limits;
7. create one quantitative or worked example where useful;
8. create/reuse Decision Object;
9. map to episodes;
10. evaluate Podcast Ready gate.

## Promotion criteria
A claim can move from breadth evidence toward EVIDENCE VALIDATED when the evidence directly supports the scoped claim, applicability is explicit, conflicts are represented and the source is strong enough for the consequence of the advice.

An episode can move to PODCAST READY only when its critical claims—not every background fact—meet that bar and its case/example layer is credible.

## Decision
**PASS 1 AUDIT: PASS WITH CONTROLLED GAPS.**
Proceed to Pass 2 using the queue above. Create A9 before Episodes 53–60 are treated as research-covered.