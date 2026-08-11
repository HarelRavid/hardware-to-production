# Phase 2 — Evidence Campaign Tracker

status: PASS 1 AUDIT COMPLETE — PASS 2 READY / A9 OPEN
started_on: 2026-08-09
updated_on: 2026-08-11

## Pass 1 — Breadth tracker

| Priority | Evidence package | Podcast leverage | Status |
|---|---|---|---|
| A0 | Early hardware development / Opening Arc | A1–A8 + bridge to Episodes 1–10 | BREADTH COMPLETE |
| A1 | Product development / NPI / production readiness | Episodes 1–5 | BREADTH COMPLETE |
| A2 | DFM / DFA / DFT foundations | Episodes 6–10 | BREADTH COMPLETE |
| A3 | Manufacturing process selection / lifecycle economics | Episode 11 + process arc | BREADTH COMPLETE |
| A4 | Quality foundations: PFMEA/control plan/MSA/SPC/capability | Episodes 23–24, 32 | BREADTH COMPLETE |
| A5 | Pilot/PVT/ramp/yield/capacity | Episodes 26–31 | BREADTH COMPLETE |
| A6 | Supplier industrialization / qualification / change control | Episodes 30, 37–40 | BREADTH COMPLETE |
| A7 | Automation business case / qualification / OEE | Episodes 41–46 | BREADTH COMPLETE |
| A8 | Manufacturing Data Hub standards / semantic integration / OT-ICS | Episodes 47–52 | BREADTH COMPLETE |
| A9 | Case studies & cross-industry synthesis | Episodes 53–60 | OPEN — CASE CAMPAIGN |

## Pass 1 result
A0–A8 breadth packages are complete. The cross-domain audit is recorded in `evidence/PASS1_CROSS_DOMAIN_AUDIT.md`.

Audit decision: **PASS WITH CONTROLLED GAPS**.
No architecture-breaking contradiction was identified. Main governance issue is duplicated ownership of cross-domain concepts, now resolved through canonical-owner rules.

## Canonical ownership summary
- A0: early prototype representativeness / manufacturing debt
- A1: product maturity / production intent / configuration-readiness governance
- A2: DFM/DFA/DFT
- A3: process selection / bridge manufacturing / generic lifecycle economics
- A4: PFMEA / Control Plan / MSA / SPC / process capability
- A5: pilot / PVT / ramp / rate / yield / capacity
- A6: supplier qualification / FAI-PPAP boundary / supplier change / sub-tier control
- A7: automation qualification / OEE / automation TCO / machinery-cell integration
- A8: semantic identity / genealogy / provenance / system-of-record / OT-ICS integration
- A9: documented case studies / cross-industry transfer / Episode 60 synthesis

## Controlled gaps from audit
1. electronics manufacturing depth for Opening A6 and downstream DFT/production-test coverage;
2. reliability-engineering bridge into manufacturing controls;
3. serviceability/repair/field-return feedback loop;
4. product/regulatory safety must be handled through scoped applicability rather than a universal regulation package;
5. Episodes 53–60 require A9 case-study evidence.

## Pass-2 first priority queue
P0:
1. A0/A1 lifecycle/readiness definitions and Hardware Evolution Ladder evidence mapping;
2. A1 configuration baseline/change-control worked example;
3. A4 PFMEA→Control Plan→MSA→SPC→Capability worked example;
4. A5 Pilot/PVT/run-at-rate/capacity exit-criteria worked example.

P1:
5. A3 quantitative process-selection/bridge-manufacturing economics;
6. A6 supplier qualification ladder and applicability;
7. A7 automation ROI/TCO + FAT/SAT/production qualification;
8. A8 ISA-95/OPC UA/IEC 62443 + genealogy/effectivity/write-back reference architecture;
9. electronics manufacturing gap package;
10. reliability-to-manufacturing-control worked example.

P2:
11. A9 case-study population and cross-industry applicability matrices;
12. Episode 60 end-to-end composite decision story;
13. integrated Manufacturing Atlas implementation-validation scenarios.

## Important terminology guardrails from audit
- product/design validation ≠ production validation ≠ supplier qualification ≠ FAT/SAT;
- process capability ≠ production capacity ≠ supplier capability;
- metrological traceability ≠ product genealogy/provenance;
- semantic integration ≠ system-of-record ownership;
- first article conformity ≠ serial capability;
- high local OEE/utilization ≠ good system flow/profitability.

## Campaign rule
Breadth complete does not mean EVIDENCE VALIDATED or PODCAST READY.
Pass 2 deepens canonical claims once, then reuses them across episodes.

## Immediate sequence
1. Open/populate A9 enough to establish case-study candidate coverage for Episodes 53–60.
2. Begin Pass-2 P0 with lifecycle/readiness definitions and the first configuration/change-control worked example.
3. Continue through P0 before broad P1 execution unless new evidence exposes an architecture gap.