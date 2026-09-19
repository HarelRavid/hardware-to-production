# Season 4 S4-B — Make/Buy / Supplier Capability Shared Source Register

status: SHARED SOURCE REGISTER LOCKED
checked: 2026-09-19
scope: EP37 / EP38
governed_by: podcast/season-4/SEASON_4_CLAUDE_HANDOFF_DELIVERY_BOARD.md
dependencies: Wave 02 supplier evidence + Wave 03 economics/capacity + Wave 01 configuration/change

## 1. Purpose

Lock the generic engineering premises required to decide make/buy and assess supplier capability without reducing sourcing to piece price, certificates or equipment lists.

## 2. NIST supplier-management source family

### S4B-S01 — NIST MEP Supply Chain Management
Official:
https://www.nist.gov/mep/supply-chain

Public support:
- supplier evaluation/selection;
- supplier segmentation;
- total cost of ownership;
- supplier metrics/scorecards;
- supplier development;
- supply-chain mapping/risk assessment.

Use:
EP37/EP38.

### S4B-S02 — NIST MEP Supplier Scouting
Official:
https://www.nist.gov/mep/supply-chain/supplier-scouting

Public support:
supplier scouting is based on matching actual manufacturing capabilities/business interest to production/technical requirements.

Use:
EP38 capability-first supplier discovery context.

## 3. Investment / economics source family

### S4B-S03 — NIST AMS 200-5 Investment Analysis Methods
Reuse from Wave 03.

Support:
NPV, IRR, payback and manufacturing-investment decision analysis.

Use:
EP37.

### S4B-S04 — NIST Smart Investment Tool / capital investment analysis
Reuse from Wave 03.

Support:
manufacturing investment alternatives should be compared with explicit cash flows/assumptions/uncertainty.

Use:
EP37.

## 4. Supplier approval / capability source family

### S4B-S05 — NIST MEP supplier-development context
Reuse Wave 02 W2-S11.

Support:
supplier evaluation, metrics, development and quality-system support.

### S4B-S06 — IAQG 9102 public FAI scope
Reuse Wave 02 W2-S12.

Support:
first-article/configuration verification is a bounded evidence question in aviation/space/defense context.

### S4B-S07 — AIAG PPAP public scope
Reuse Wave 02 W2-S05.

Support:
automotive production-part approval asks whether engineering requirements can be consistently met using actual production processes at production rates.

Applicability guard:
automotive/customer-specific requirements are not generalized.

## 5. Shared S4-B claims

### S4B-C01 — make/buy is a capability/control/economics decision, not a piece-price comparison
Status: VERIFIED PREMISE + V6 SYNTHESIS.
Sources: S4B-S01/S03/S04.

### S4B-C02 — internal manufacturing CAPEX should account for utilization, maintenance, support and opportunity cost where material
Status: VERIFIED PREMISE + Wave03 synthesis.
Sources: S4B-S03/S04.

### S4B-C03 — outsourcing can transfer execution but does not transfer product-conformity/accountability automatically
Status: V6 SYNTHESIS.

### S4B-C04 — strategic knowledge/IP/change-speed/supply-risk can be decision variables even when they are not captured in supplier piece price
Status: V6 SYNTHESIS supported by S4B-S01.

### S4B-C05 — supplier certification/equipment list/sample parts do not by themselves establish source capability
Status: VERIFIED PREMISE + V6 SYNTHESIS.
Sources: S4B-S01/S05/S06/S07.

### S4B-C06 — supplier capability should be evaluated against actual product/process/CTQ/measurement/capacity/change/recovery requirements
Status: VERIFIED PREMISE + V6 SYNTHESIS.
Sources: S4B-S01/S02/S05 + Waves02/03.

### S4B-C07 — supplier sample evidence and sustained production capability are distinct
Status: VERIFIED.
Sources: S4B-S06/S07 + NIST capability principles.

### S4B-C08 — sub-tier/special-process dependencies can be common-mode capability/resilience risks
Status: V6 SYNTHESIS + EP40 dependency.

### S4B-C09 — make/buy decision can change with lifecycle stage, demand, design stability and evidence maturity
Status: V6 SYNTHESIS + Wave03 economics.

### S4B-C10 — supplier assessment/audit should be proportional to consequence and actual process/evidence risk
Status: V6 SYNTHESIS.

## 6. Hard guardrails

1. no cheapest-quote-wins rule;
2. no universal make/buy volume threshold;
3. no universal CAPEX/payback hurdle;
4. no certification = process capability shortcut;
5. no equipment list = capability shortcut;
6. no sample approval = sustained source approval shortcut;
7. no universal audit checklist;
8. no mandatory second-source rule;
9. no industry-specific PPAP/FAI requirement generalized;
10. no outsourcing = accountability transfer.

## 7. Episode mapping

EP37:
S4B-S01/S03/S04 + Wave03 economics.

EP38:
S4B-S01/S02/S05/S06/S07 + Wave02 supplier/capability evidence.

## 8. Current generic blockers

No intended EP37–38 script requires protected PPAP/FAI detail, customer-specific supplier approval rules or organization-specific finance thresholds.

Current generic-script P0 blockers: 0.
