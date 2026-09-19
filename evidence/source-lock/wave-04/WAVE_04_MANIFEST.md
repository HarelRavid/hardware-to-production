# Source-Lock Wave 04 — Automation / Machinery Safety / OEE

status: ACTIVE — SHARED SOURCES LOCKED; CLAIM LOCK IN PROGRESS
opened: 2026-09-19
scope_type: shared-source-family wave
baseline_head_at_open: 199e97df7fffd1670071cd1a51de93a122b87dc1

## 1. Purpose

Advance EP41–46 and P2.07 from production architecture into controlled publication packages while preserving strict separation among:
- automation engineering guidance;
- machinery/robot safety-standard scope;
- jurisdiction-specific legal obligations;
- OEE/loss analysis;
- automation economics;
- automated test/measurement;
- qualification/recovery/release.

Pipeline:
Shared Source Lock → Episode Claim Lock → Internal Technical Review → Script Outline → Full Script Draft → Script Review → Source Notes → Publication Gate.

## 2. Direct episode scope

- EP41 — When Not to Automate
- EP42 — Building the Business Case for Automation
- EP43 — Semi-Automation, Robotics and Machine Vision
- EP44 — Automated Inspection and End-of-Line Test
- EP45 — Automation Qualification, OEE and Maintenance
- EP46 — Scaling Without Automating Defects

Backbone:
- P2.07 — Automation / Qualification / OEE / Failure-Recovery / Release

Dependencies:
- Wave 01 — configuration/change/effectivity
- Wave 02 — measurement/quality/supplier evidence
- Wave 03 — capacity/constraint/economics/ramp evidence

## 3. Canonical shared register

evidence/source-lock/SOURCE_LOCK_WAVE_04_AUTOMATION_SAFETY_OEE_REGISTER.md

## 4. Current standards status checked 2026-09-19

- ISO 12100:2010 — current published edition; revision project active.
- ISO 13849-1:2023 — current published Part 1.
- ISO 13849-2:2012 — current published Part 2; revision draft active.
- IEC 62061:2021 + AMD1:2024 + AMD2:2026 — current consolidated family.
- ISO 10218-1:2025 — current industrial-robot Part 1.
- ISO 10218-2:2025 — current robot-application/cell Part 2.
- IEC 60204-1:2016 + AMD1:2021 — current public consolidated family.
- IEC 62381:2024 — current FAT/FIT/SAT/SIT edition.
- ANSI/ISA-62381-2026 — national adoption/status reference only; protected content not reproduced.
- ISO 22400-2:2014 + Amd1:2017 — current published KPI standard; Edition 2 revision active.

## 5. OEE arithmetic control

Sentinel semi-automatic station:
- Availability = 90.00%
- Performance = 93.253968%
- Quality = 95.957447%
- OEE = 80.535714%

Equal-OEE comparison:
- Cell A = 82% × 99% × 99% = 80.3682%
- Cell B = 99% × 99% × 82% = 80.3682%

All are illustrative and independently recalculated.

## 6. Wave-wide guardrails

1. No universal OEE benchmark.
2. OEE is a loss lens, not root-cause/capacity proof.
3. Automation is not a maturity badge.
4. Robot/cobot label is not application-level safety evidence.
5. Exact safety PL/SIL/guarding/electrical requirements stay clause/applicability gated.
6. Standards are not automatically legal obligations in every jurisdiction.
7. FAT/SAT/SIT are acceptance layers, not automatic production release.
8. Automated test inherits Wave 02 measurement-system requirements.
9. Automation economics inherits Wave 03 demand/capacity/NPV/sensitivity controls.
10. Replicated cells require equivalence evidence; machine count is not scale proof.
11. Restart after intervention does not automatically restore release trust.
12. Changes inherit Wave 01 impact/effectivity logic.

## 7. Completion criterion

Wave 04 closes when EP41–46 each have:
- claim lock;
- internal technical review;
- source-linked outline;
- full script draft;
- script review;
- source notes;
- explicit safety/legal/standard application gates;
- publication-gate record.
