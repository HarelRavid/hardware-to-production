# Source-Lock Wave 03 — Pilot / Capacity / Ramp / Economics Shared Source Register

status: SHARED SOURCE REGISTER LOCKED
checked: 2026-09-19
scope: EP26 / EP27 / EP28 / EP29 / EP30 / EP31 + P2.04 / P2.05
backbone: Pilot/PVT/Run-at-Rate/Capacity/Ramp + Process Economics/CapEx/NRE/NPV/Sensitivity

## 1. Purpose

Lock the authoritative/public source layer shared by the production-validation, ramp, capacity and economics episodes.

Wave 03 separates:
- authoritative production-readiness / flow / investment premises;
- internal Hardware-to-Production frameworks and illustrative Sentinel calculations;
- customer/industry-specific Run-at-Rate / PVT / PPAP requirements that remain applicability gated.

No universal pilot quantity, run duration, ramp-exit threshold, capacity margin, payback target or discount rate is introduced.

## 2. Current authoritative source register

### W3-S01 — NASA NPR 7123.1D
Owner: NASA
Title: NASA Systems Engineering Processes and Requirements
Current status checked: NPR 7123.1D, Updated with Change 2
Effective: 2023-07-05
Expiration: 2028-07-05
Official source:
https://nodis3.gsfc.nasa.gov/displayDir.cfm?Internal_ID=N_PR_7123_001D_&page_name=Preface

Applicability:
Mandatory for NASA employees/programs/projects inside its stated scope.
For this podcast it is used as authoritative NASA evidence and as a source of transferable production-readiness categories, not as a universal startup requirement.

### W3-S02 — NASA NPR 7123.1D Appendix G / Production Readiness Review
Owner: NASA
Source:
https://nodis3.gsfc.nasa.gov/displayDir.cfm?Internal_ID=N_PR_7123_001D_&page_name=AppendixG

Current PRR location:
Appendix G, G.9, Table G-8.

Strong support:
- PRR determines readiness to efficiently produce the required number of systems/units;
- production engineering problems/nonconformances should be resolved;
- production documentation/plans are required;
- critical process controls/control limits/procedures are part of production planning;
- production-enabling resources, facilities, tooling/test equipment, personnel and suppliers are part of readiness;
- production processes/methods must be consistent with quality requirements;
- supplier quality-control readiness is explicitly considered.

Episode use:
EP26/27/30 and ramp-exit synthesis.

Guardrail:
NASA PRR criteria are NASA review criteria. Our Pilot Build Plan, Production Validation Matrix and RAMP 10 are internal synthesis.

### W3-S03 — NASA Systems Engineering Handbook Appendix / PRR definition
Owner: NASA
Source:
https://www.nasa.gov/reference/system-engineering-handbook-appendix/

Support:
PRR evaluates whether developers are ready to efficiently produce the required number of systems and whether production plans/fabrication/assembly/integration enabling products/operational support/personnel are ready.

Use:
listener-friendly authoritative definition support.

### W3-S04 — Lean Enterprise Institute — Takt Time
Owner: Lean Enterprise Institute
Source:
https://www.lean.org/lexicon-terms/takt-time/

Support:
takt time = available production time divided by customer demand; intended to match production pace with demand.

Episode use:
EP29.

Applicability:
recognized lean-practice source, not statutory/normative requirement.

### W3-S05 — Lean Enterprise Institute — Cycle Time
Owner: Lean Enterprise Institute
Source:
https://www.lean.org/lexicon-terms/cycle-time/

Support:
cycle time is actual measured time to produce a part or complete a process; related definitions distinguish operator/machine/effective machine cycle time.

Episode use:
EP29.

### W3-S06 — NIST manufacturing analytical services / Little's Law and utilization
Owner: NIST
Source:
https://tsapps.nist.gov/publication/get_pdf.cfm?pub_id=920909

Support:
- capacity optimization must account for rising cycle/queue time and WIP at high utilization;
- WIP = throughput × queue/cycle-time relationship is explicitly used via Little's Law;
- system throughput cannot be inferred from isolated resource speed alone.

Episode use:
EP29 run-at-rate / WIP / queue reasoning.

### W3-S07 — NIST Inventory and Flow Time in U.S. Manufacturing
Owner: NIST
Publication: NIST TN 1890
Source:
https://www.nist.gov/publications/inventory-and-flow-time-us-manufacturing-industry

Support:
inventory, waiting and rework/defects are manufacturing-flow wastes; flow time includes time a unit spends in process.

Episode use:
EP28/29 flow/WIP context.

### W3-S08 — NIST Flow Time Innovations
Owner: NIST
Publication: NIST AMS 100-25
Source:
https://www.nist.gov/publications/flow-time-innovations-effect-productivity-and-production-us-manufacturing

Support:
flow-time changes can materially affect manufacturing productivity/production; WIP flow time is economically meaningful.

Episode use:
EP28/29 supporting context.
Guardrail:
population-level historical estimates are not used as universal shop-floor improvement percentages.

### W3-S09 — NIST MEP supplier/capacity improvement case family
Owner: NIST Manufacturing Extension Partnership
Representative sources:
- https://www.nist.gov/mep/successstories/2025/learning-doubling-throughput-and-having-fun
- https://www.nist.gov/mep/successstories/2022/utilizing-robots-and-process-improvement-techniques-improve-turnaround-time

Use:
illustrative practitioner evidence that WIP, synchronization, process improvement and throughput are linked in real manufacturing work.

Guardrail:
case percentages are case-specific, not general benchmarks.

### W3-S10 — NIST AMS 200-5 Investment Analysis Methods
Owner: NIST
Title: Investment Analysis Methods: A practitioner's guide to understanding the basic principles for investment decisions in manufacturing
Published: 2017
Source:
https://www.nist.gov/publications/investment-analysis-methods-practitioners-guide-understanding-basic-principles

Strong support:
manufacturing investments can be evaluated using methods including NPV, IRR, payback and related investment-analysis methods.

Episode use:
P2.05 and downstream automation-business-case episodes.

### W3-S11 — NIST Capital Investment Analysis / Smart Investment Tool
Owner: NIST
Sources:
- https://www.nist.gov/el/applied-economics-office/manufacturing/capital-investment-analysis
- https://www.nist.gov/services-resources/software/smart-investment-tool
- https://www.nist.gov/publications/guide-smart-investment-tools

Current tool guide:
NIST AMS 100-62, published 2024.

Strong support:
- NPV = present-value inflows minus outflows over the investment period;
- IRR = discount rate at which NPV is zero;
- payback = time to recoup investment;
- sensitivity/Monte Carlo can be used to examine uncertainty;
- manufacturing investment alternatives can be compared using detailed cash flows.

Episode use:
economics layer reused by EP29/EP41–46/EP55/EP60.

### W3-S12 — NIST AMS 200-11
Owner: NIST
Title: Guide for Environmentally Sustainable Investment Analysis Based on ASTM E3200
Published: 2021
Source:
https://www.nist.gov/publications/guide-environmentally-sustainable-investment-analysis-based-astm-e3200

Strong support:
NPV, IRR, payback, hurdle-rate and sensitivity/Monte Carlo techniques are valid investment-analysis tools.

Guardrail:
the sustainability framing is source-specific; the generic investment methods are used without implying ASTM E3200 applies to every manufacturing investment.

### W3-S13 — NIST maintenance economics
Owner: NIST
Sources:
- NIST AMS 100-18: https://www.nist.gov/publications/costs-and-benefits-advanced-maintenance-manufacturing
- NIST AMS 100-34: https://www.nist.gov/publications/economics-manufacturing-machinery-maintenance-survey-and-analysis-us-costs-and-benefits

Support:
maintenance costs and losses due to inadequate maintenance strategy are economically material manufacturing factors.

Episode use:
P2.05; later automation economics/recovery.

### W3-S14 — NIST AMS 100-50 Efficiency Investment Returns
Owner: NIST
Source:
https://www.nist.gov/publications/efficiency-improvements-us-manufacturing-return-investment-small-and-medium
Supporting topic page:
https://www.nist.gov/el/applied-economics-office/manufacturing/topics-manufacturing/efficiency-investment-returns

Support:
returns vary across investment categories; bottleneck reduction and scheduling appeared among high-IRR categories in the studied dataset.

Use:
supports comparing lower-capital flow/constraint interventions before assuming automation is economically superior.

Guardrail:
does not prove bottleneck reduction universally has higher ROI than automation in every project.

## 3. Shared engineering claims

### W3-C01 — Pilot / production validation is a production-system evidence event
Status: VERIFIED + V6 SYNTHESIS
Support: W3-S02/S03.
Claim:
A production-intent pilot/validation build should generate evidence about the integrated production system, not only product function.

Boundary:
PVT/pilot terminology and exact gates are not universal standards.

### W3-C02 — Production representativeness is multidimensional
Status: VERIFIED PREMISE + V6 SYNTHESIS
Support: W3-S02.
Claim:
production configuration, process controls, resources, tooling/test, personnel and suppliers are all relevant to readiness evidence.

### W3-C03 — One successful batch is not proof of sustainable capacity
Status: VERIFIED + V6 SYNTHESIS
Support: W3-S02, W3-S06, W3-S07.
Claim:
batch completion, instantaneous rate and sustainable accepted throughput are different claims.

### W3-C04 — Takt and cycle time are different metrics
Status: VERIFIED
Support: W3-S04/S05.
Claim:
takt is demand-derived available time per required unit; cycle time is actual process time under stated conditions.

### W3-C05 — WIP/queue growth can expose unstable flow
Status: VERIFIED + V6 SYNTHESIS
Support: W3-S06/S07.
Claim:
when arrivals sustainably exceed departures, queues/WIP grow; adding WIP does not by itself increase physical throughput.

### W3-C06 — Rework consumes real capacity when it reuses constrained resources
Status: VERIFIED BY ARITHMETIC + V6 SYNTHESIS
Support:
flow/capacity fundamentals + Sentinel model.
Claim:
rework is both quality debt and capacity/economic load.

### W3-C07 — Ramp exit requires evidence inside a stated operating envelope
Status: VERIFIED PREMISE + V6 SYNTHESIS
Support: W3-S02.
Claim:
ramp evidence should state configuration, resources, rate/time basis, quality controls, suppliers and abnormal intervention assumptions.

### W3-C08 — Lowest variable/unit cost is not automatically best investment
Status: VERIFIED
Support: W3-S10/S11/S12.
Claim:
investment decisions require cash-flow/time/uncertainty treatment, not only steady-state variable cost.

### W3-C09 — NPV/payback/IRR are decision aids, not universal thresholds
Status: VERIFIED
Support: W3-S10/S11/S12.
Claim:
the appropriate hurdle rate/payback criterion is organization/project specific.

### W3-C10 — Sensitivity analysis is part of honest investment analysis
Status: VERIFIED
Support: W3-S11/S12.
Claim:
uncertain demand, ramp, yield, availability, maintenance and change assumptions should be tested where they can reverse the decision.

### W3-C11 — Maintenance belongs in manufacturing economics
Status: VERIFIED
Support: W3-S13.
Claim:
maintenance/support/downtime affect cost and usable capacity and should not be omitted from significant equipment-investment models.

### W3-C12 — Simpler constraint/flow interventions deserve comparison with capital investment
Status: VERIFIED AS DECISION SYNTHESIS
Support: W3-S14 + P2.04 constraint logic.
Claim:
before irreversible CapEx, compare lower-capital process/flow/scheduling/fixture/parallelization alternatives where they can solve the demonstrated constraint.

## 4. Sentinel arithmetic lock

### P2.04 capacity example
Demand: 80 accepted units / 420 planned production minutes.
Takt:
25,200 s / 80 = 315 s/accepted unit.

Constraint nominal cycle:
360 s → theoretical 70 cycles/shift.

At 90% availability:
22,680 s available → 63 first-pass cycles.

At 92% FPY:
57.96 expected first-pass accepted units;
5.04 expected first-pass failures.

First-order rework burden:
360 + 0.08×240 = 379.2 s launched-unit-equivalent constraint burden before repeat loops.

Arrival rate at demand:
80/7 h = 11.4286 units/h.

90%-available 6-minute service opportunity:
9.0 cycles/h.

Illustrative net queue growth before rework:
≈2.43 units/h.

Status:
ARITHMETIC VERIFIED — ILLUSTRATIVE MODEL.

### P2.05 break-even / payback example
Manual vs semi-auto:
incremental fixed = 37,000;
savings/unit = 6.50;
break-even ≈ 5,692.31 accepted units.

Semi-auto vs automation:
incremental fixed = 135,000;
savings/unit = 2.70;
break-even = 50,000 accepted units.

At 10,000 accepted units/year:
semi-auto vs manual simple payback ≈0.569 years.
automation vs semi-auto simple payback =5.0 years before additional ownership/support/finance effects.

Automation support allocation:
54,000/year / 40,000 units =1.35/unit.
54,000/year / 8,000 units =6.75/unit.

Yield warning example:
4.80/0.90 =5.33 per first-pass-equivalent accepted unit;
7.50/0.99 ≈7.58.

Five-year Y2 launched units:
12,000/0.94 ≈12,765.96;
12,000/0.97 ≈12,371.13;
12,000/0.98 ≈12,244.90.

Status:
ARITHMETIC VERIFIED — ALL VALUES ILLUSTRATIVE.

## 5. Hard guardrails

1. No universal pilot/PVT unit count.
2. No universal run-at-rate duration.
3. No claim that NASA PRR is required outside NASA.
4. No customer-specific Run-at-Rate/PPAP criterion unless exact applicability is sourced.
5. Takt is not cycle time.
6. Short burst rate is not sustainable accepted capacity.
7. WIP is not capacity.
8. Rework cannot be credited as free recovered output.
9. No universal acceptable yield/FPY threshold.
10. No universal hurdle/discount/payback criterion.
11. Forecast demand is not demonstrated demand.
12. Lowest steady-state unit cost is not automatically best investment.
13. Payback is not NPV.
14. NRE/forecast volume is cost allocation, not full cash-flow analysis.
15. Economics must consume measured manufacturing evidence where available rather than overwrite it with optimistic assumptions.

## 6. Episode mapping

EP26:
pilot as evidence-generating build; quantity rationale and stop/exit logic.

EP27:
integrated production validation; representative system evidence.

EP28:
FPY/rework/scrap as learning + capacity/economic burden.

EP29:
takt/cycle/throughput/capacity/constraint/WIP/run-at-rate.

EP30:
supplier readiness during ramp; capacity evidence tied to production source identity; reuses Wave 02 supplier lock.

EP31:
change during ramp; reuses Wave 01 configuration/effectivity lock and Wave 03 evidence-envelope/rate consequences.

P2.05 economics:
direct source reuse in EP29 decision consequences and later EP41–46 / EP55 / EP60. Do not force a standalone economics lecture into EP26–31 where not needed.

## 7. Unresolved application gates

- exact customer Run-at-Rate criteria;
- exact PPAP production-rate demonstration requirements;
- sector/customer PVT definitions;
- customer-specific ramp release thresholds;
- organization-specific finance hurdle rates;
- tax/depreciation/accounting treatment;
- real project CapEx/maintenance/labor/demand inputs.

These are not blockers for the generic Wave 03 scripts when they remain excluded or explicitly illustrative.
