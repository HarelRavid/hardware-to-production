# Source-Lock Wave 06A — Manufacturing Process Selection Shared Source Register

status: SHARED SOURCE REGISTER LOCKED
checked: 2026-09-19
scope: EP11 — How to Select a Manufacturing Process
dependencies: DFX source map + Wave 03 economics + Waves 01/02/03 supplier/quality/capacity

## 1. Purpose

Lock the generic engineering premises required to compare manufacturing routes before process-specific Episodes 12–18.

EP11 must teach decision architecture, not universal numeric limits for molding, machining, casting, joining, additive or other process families.

## 2. Authoritative source register

### W6A-S01 — NIST Manufacturing Process and Material Selection During Conceptual Design
Owner: NIST
Published: 1997-05-01
Source:
https://www.nist.gov/publications/manufacturing-process-and-material-selection-during-conceptual-design

Strong support:
- material and manufacturing-process decisions should be considered together;
- early design has imprecise requirements/characteristics;
- alternatives should be identified early and balanced against functional and economic concerns.

Episode use:
multi-attribute material/process selection.

### W6A-S02 — NIST Conceptual Process Planning
Owner: NIST
Published: 1999-08-01
Source:
https://www.nist.gov/publications/conceptual-process-planning-definition-and-functional-decomposition

Strong support:
- conceptual process planning lets designers evaluate manufacturability and manufacturing cost during early design;
- major manufacturing cost is committed through product specification/design;
- process planning and design should be integrated early.

Episode use:
DFM/process-selection timing.

### W6A-S03 — NIST Incorporating Process Planning into Conceptual Design
Owner: NIST
Published: 1999-09-01
Source:
https://www.nist.gov/publications/incoporating-process-planning-conceptual-design

Support:
design/process-planning integration and early manufacturability/cost assessment.

### W6A-S04 — NIST Information Modeling on Conceptual Process Planning Integrated with Conceptual Design
Owner: NIST
Published: 2000
Source:
https://www.nist.gov/publications/information-modeling-conceptual-process-planning-integrated-conceptual-design

Support:
conceptual process planning includes process selection, resource selection, cost and time estimation.

Episode use:
process-chain/resource/economic decision dimensions.

### W6A-S05 — NIST Decision Support for Material and Manufacturing Process Selection
Owner: NIST
Published: 1997
Source:
https://www.nist.gov/publications/decision-support-system-material-and-manufacturing-process-selection

Support:
material/process selection is a multi-attribute decision made amid uncertain/imprecise early requirements.

Episode use:
Process Selection Decision Grid.

Guardrail:
the podcast does not reuse the paper's specific possibility-theory ranking method as a universal process-selection algorithm.

### W6A-S06 — NIST Manufacturing Cost Guide Version 2.0 Primer
Owner: NIST
Publication: NIST AMS 100-83
Published: 2026-08-11
Source:
https://www.nist.gov/publications/manufacturing-cost-guide-version-20-primer

Use:
current manufacturing-economics/supply-chain context.

Boundary:
the Cost Guide 2.0 operates at industry/supply-chain input-output level; it is not a direct process-level part-cost calculator for EP11.

### W6A-S07 — NIST Manufacturing Cost Guide software v2.0
Owner: NIST
Updated: 2026-08-19
Source:
https://www.nist.gov/services-resources/software/mcg-supply-chain-statistics

Use:
revision/current-tool context only.

### W6A-S08 — NIST SP 1176 Additive Manufacturing Cost Effectiveness
Owner: NIST
Published: 2014
Source:
https://www.nist.gov/publications/costs-and-cost-effectiveness-additive-manufacturing

Support:
technology/process economics are context dependent; additive is not universally cheaper; utilization/material/tooling economics matter.

Episode use:
example showing process-name decisions require cost boundary/context.

### W6A-S09 — NIST Additive Manufacturing Supply Chain Perspective
Owner: NIST
Published: 2016
Source:
https://www.nist.gov/publications/costs-benefits-and-adoption-additive-manufacturing-supply-chain-perspective

Support:
part-level cost comparisons can omit inventory/transport/supply-chain effects; total advantage depends on system boundary.

Episode use:
cost-boundary discipline.

## 3. Shared EP11 engineering claims

### W6A-C01 — manufacturability/process planning belongs in design, not only after release
Status: VERIFIED OPEN SOURCE.
Sources: W6A-S02/S03.

### W6A-C02 — material and manufacturing-process selection are coupled
Status: VERIFIED OPEN SOURCE.
Sources: W6A-S01/S05.

### W6A-C03 — process selection is multi-attribute, not geometry-only or piece-price-only
Status: VERIFIED + V6 SYNTHESIS.
Sources: W6A-S01/S04/S05.

### W6A-C04 — early uncertainty does not prevent process-selection work
Status: VERIFIED.
Source: W6A-S01/S05.
Claim:
early teams can use ranges/sets/candidates rather than falsely precise fixed inputs.

### W6A-C05 — process-chain economics require a declared system boundary
Status: VERIFIED + V6 SYNTHESIS.
Sources: W6A-S04/S08/S09 + Wave 03.

### W6A-C06 — supplier/equipment capability is part of route feasibility
Status: DEPENDENCY — Waves 02/03 supplier/capacity.
Claim:
theoretical process capability is not demonstrated source capability.

### W6A-C07 — prototype-route evidence does not automatically transfer to a production route with different material/process mechanisms
Status: DEPENDENCY — A4/Wave 01 representativeness + V6.
Example:
CNC polymer enclosure evidence does not automatically prove molded shrink/warp/sealing behavior.

### W6A-C08 — bridge manufacturing is legitimate when its evidence/economic limits and exit trigger are explicit
Status: V6 LOCKED AS SYNTHESIS.
No universal volume threshold.

### W6A-C09 — “high-volume process” is not automatically the better route
Status: VERIFIED + V6 SYNTHESIS.
Support: process/material/economic sources + Wave 03.

### W6A-C10 — compare cost per accepted final product/process chain, not only primary-operation quote
Status: VERIFIED PREMISE + V6 SYNTHESIS.
Sources: W6A-S04/S09 + Wave 02 yield + Wave 03 economics.

## 4. EP11 Process Selection Decision Grid ownership

Internal synthesis:
Function → material/state → geometry → tolerance/surface → lifecycle stage/volume → candidate route → capability evidence → inspection → supplier/resource → tooling/NRE → yield/secondary ops → cost per good unit → exit trigger.

This is not a NIST standard or universal scoring formula.

## 5. Hard guardrails

1. no universal volume threshold for injection molding, machining, casting or AM;
2. no universal process tolerance/capability value in EP11;
3. material trade name alone does not define final state;
4. quoted piece price is not total route economics;
5. prototype success is not production-route qualification;
6. supplier brochure capability is not demonstrated source capability;
7. NIST Manufacturing Cost Guide 2.0 is not represented as a part-cost calculator;
8. process-specific standards and numeric limits are deferred to 06B–06H;
9. bridge-process exit is evidence/economics based, not one unit-count rule;
10. scoring tools cannot average away hard functional/safety/regulatory constraints.

## 6. Episode gate

EP11 can proceed using generic process-selection evidence without opening process-family-specific numeric claims.

Current generic-script P0 blockers: 0.
