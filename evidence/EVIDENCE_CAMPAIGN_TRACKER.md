# Phase 2 — Evidence Campaign Tracker

status: ACTIVE
started_on: 2026-08-09

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
| A8 | Manufacturing Data Hub standards / semantic integration / OT-ICS | Episodes 47–52 | IN PROGRESS — ACTIVE CAMPAIGN |

## A7 — Breadth result
Automation now has a cross-functional evidence backbone covering:
- ISA/IEC FAT, SAT and SIT acceptance boundaries;
- NIST maintenance economics and strategy;
- NIST/ISO 22400 context for manufacturing performance/OEE;
- ISO 10218-1:2025 robot safety versus ISO 10218-2:2025 application/cell integration safety;
- NIST task-based human-robot collaboration risk assessment;
- robotic assembly deployment constraints including expertise, interoperability and error recovery;
- lifecycle/TCO, process maturity, human/automation allocation and DEV/LVP/SVP decision logic.

Editorial conclusions supported:
1. technical feasibility is not sufficient business justification for automation;
2. FAT, SAT/SIT and production qualification answer different questions;
3. automation economics must include lifecycle and recovery costs beyond direct labor;
4. a robot's safety status does not establish application/cell safety;
5. human-robot safety and work allocation are task/application dependent;
6. OEE is not profitability and high local utilization is not automatically good system flow;
7. maintenance, diagnostics, spares, recovery and skills are design/business-case inputs;
8. product/process/configuration change can require automation reassessment/requalification.

A7 Pass-2 targets include worked ROI/TCO sensitivity, premature-automation case, ISO 22400/OEE extraction, machinery-safety applicability map, qualification checklist, maintenance/recovery case and product-change requalification case.

## Campaign rule
Breadth pass does not attempt exhaustive research. Each package must first identify authoritative source families, episode-critical claims, weak/GNR claims, applicability conflicts and Pass-2 depth targets.

## Promotion rule
A package moves to BREADTH COMPLETE when those elements are represented and the strongest primary sources are captured or remaining gaps are explicitly bounded for Pass 2.

## Immediate sequence
1. A8 — Manufacturing Data Hub standards / semantic integration / OT-ICS cybersecurity.
2. Validate the Section 9 conceptual architecture against ISA-95/IEC 62264, OPC UA, system-of-record/temporal patterns and IEC 62443 where applicable.
3. Build at least one concrete Applicability Statement chain and identify the reference-implementation/mock-data requirements.
4. Preserve the distinction DEFINED -> EVIDENCE VALIDATED -> IMPLEMENTATION VALIDATED.
5. After A8 breadth, perform a Pass-1 audit across A0–A8 and prioritize Pass-2 depth by podcast sequence and engineering risk.