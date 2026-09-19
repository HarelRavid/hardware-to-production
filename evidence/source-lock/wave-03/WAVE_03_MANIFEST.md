# Source-Lock Wave 03 — Pilot / Capacity / Ramp / Economics

status: ACTIVE — SHARED SOURCES LOCKED; CLAIM LOCK IN PROGRESS
opened: 2026-09-19
scope_type: shared-source-family wave
baseline_head_at_open: 55c0f1742636388bddd7f5227d677f4b7b41a7da

## 1. Purpose

Advance the canonical Season 3 ramp family from production architecture into controlled publication packages.

Pipeline:
Shared Source Lock → Episode Claim Lock → Internal Technical Review → Script Outline → Full Script Draft → Script Review → Source Notes → Publication Gate.

## 2. Direct episode scope

- EP26 — How to Plan a Pilot Build
- EP27 — What a Production Validation Build Must Prove
- EP28 — Yield, Rework, Scrap and the Learning Curve
- EP29 — Capacity, Bottlenecks, Takt Time and Line Balance
- EP30 — Supplier Readiness and Contract-Manufacturer Management
- EP31 — Engineering Changes During Ramp-Up

Backbone:
- P2.04 Pilot / PVT / Run-at-Rate / Capacity / Ramp Exit
- P2.05 Process Economics / CapEx / NRE / Break-even / NPV / Sensitivity

## 3. Canonical shared register

evidence/source-lock/SOURCE_LOCK_WAVE_03_RAMP_ECONOMICS_REGISTER.md

## 4. Source strategy

Open authoritative/public sources carry the generic production-readiness, flow and economics premises:
- NASA NPR 7123.1D + Appendix G PRR;
- NASA Systems Engineering Handbook PRR definition;
- NIST manufacturing analytical/flow-time research;
- Lean Enterprise Institute takt/cycle-time definitions;
- NIST manufacturing-investment guides/tools;
- NIST maintenance economics.

Customer/industry-specific items stay gated:
- exact PVT definitions;
- exact customer Run-at-Rate duration/acceptance thresholds;
- PPAP production-rate submission requirements;
- organization-specific financial hurdle/payback criteria.

## 5. Current source status checked 2026-09-19

NASA:
- NPR 7123.1D, Updated with Change 2;
- effective 2023-07-05;
- expiration 2028-07-05;
- G.9 / Table G-8 contains current PRR criteria.

NIST investment-analysis source family:
- AMS 200-5 — manufacturing investment-analysis methods;
- AMS 200-11 — NPV/IRR/payback/hurdle/sensitivity/Monte Carlo;
- Smart Investment Tool v1.0.2, last updated 2024-06-07;
- AMS 100-62 Smart Investment Tool guide, published 2024.

## 6. Quantitative verification

All current Sentinel Wave 03 arithmetic has been independently recomputed.

Capacity:
- 80 accepted units / 420 min → takt 315 s/unit.
- 360 s serial constraint → 70 theoretical cycles/shift.
- 90% availability → 63 first-pass cycles.
- 92% FPY → 57.96 first-pass accepted.
- illustrative queue growth before rework ≈2.43 units/hour.

Economics:
- manual→semi break-even ≈5,692 accepted units.
- semi→automation break-even 50,000 accepted units.
- simple payback at 10k units/year: ≈0.57 y and 5.0 y respectively.
- support allocation and accepted-unit/yield calculations checked.

All are illustrative, not field data or universal thresholds.

## 7. Wave-wide guardrails

1. No universal pilot/PVT sample size.
2. No universal run-at-rate duration.
3. No universal ramp-exit threshold.
4. No universal acceptable yield/FPY.
5. No customer-specific rate/PPAP rule unless sourced.
6. Takt, cycle time, throughput, capacity and lead time remain distinct.
7. Short target-rate burst is not sustainable capacity.
8. Rework load must remain visible.
9. Forecast demand is not demonstrated demand.
10. No universal discount/hurdle/payback rate.
11. Payback is not NPV.
12. A low unit cost does not automatically justify irreversible CapEx.
13. Changes during ramp inherit Wave 01 configuration/effectivity discipline.
14. Supplier readiness inherits Wave 02 supplier-evidence discipline.

## 8. Completion criterion

Wave 03 closes when EP26–31 each have:
- claim lock;
- technical review;
- source-linked outline;
- full script draft;
- script review;
- source notes;
- explicit customer/industry/finance gates;
- wave publication-gate record.

Later reuse of P2.05 in automation/startup/synthesis episodes requires claim-specific mapping rather than blanket citation reuse.
