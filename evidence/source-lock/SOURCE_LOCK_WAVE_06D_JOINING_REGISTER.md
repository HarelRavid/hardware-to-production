# Source-Lock Wave 06D — Joining Shared Source Register

status: SHARED SOURCE REGISTER LOCKED
checked: 2026-09-19
scope: EP14 — Joining: Welding, Adhesives, Brazing, Soldering and Fasteners
dependencies: Wave 06A process selection + Wave 02 quality/measurement + Wave 03 economics/change + Season 1 EP07 assembly

## 1. Purpose

Lock the public/authoritative premises required to compare joining routes by joint function, material/interface state, process variables, inspectability, repairability and evidence — without teaching one industry's qualification regime as universal.

EP14 is a joining-selection episode, not a welding-code, soldering-standard or fastener-design course.

## 2. Fusion welding source family

### W6D-S01 — ISO 3834-1:2021
Title: Quality requirements for fusion welding of metallic materials — Part 1
Edition: 3
Official:
https://www.iso.org/standard/81650.html

Public support:
- fusion-welding quality requirements are selected according to application/context;
- welding quality is a manufacturing-quality system/process issue, not only final visual inspection;
- applies to workshop and field fabrication.

Use:
welding as a controlled manufacturing process.

Guardrail:
ISO 3834 is not asserted as universally mandatory for every welded hardware product.

### W6D-S02 — ISO 15614-1:2017 + Amd1:2019
Title: Specification and qualification of welding procedures for metallic materials — Welding procedure test — Part 1
Official:
https://www.iso.org/standard/51792.html

Current status checked:
- published/current;
- revision active;
- ISO/DIS 15614-1 Edition 3 has progressed toward FDIS.

Public support:
procedure qualification demonstrates that a proposed welding process can produce joints with required properties inside its qualification range.

Use:
coupon/procedure qualification vs actual production context.

### W6D-S03 — ISO 9606-1:2012
Title: Qualification testing of welders — Fusion welding — Part 1: Steels
Official:
https://www.iso.org/standard/54936.html

Current status:
- published/current;
- confirmed 2023;
- revision active / replacement project underway.

Public support:
manual/partly mechanized welder qualification is distinct from procedure qualification.

Use:
personnel/process/equipment evidence distinctions.

Guardrail:
EP14 does not prescribe a welder-qualification scheme generically.

## 3. Adhesive bonding source family

### W6D-S04 — ISO 17212:2012
Title: Structural adhesives — Guidelines for surface preparation of metals and plastics prior to adhesive bonding
Official:
https://www.iso.org/standard/50596.html

Current status:
confirmed/current.

Public support:
surface preparation is a defined process input for structural adhesive bonding.

### W6D-S05 — ISO 21368:2022
Title: Adhesives — Guidelines for fabrication of adhesively bonded structures and reporting procedures suitable for risk evaluation
Official:
https://www.iso.org/standard/77454.html

Current status:
- published/current;
- confirmed 2025;
- revision underway;
- ISO/CD 21368-1 is intended to replace it.

Public support:
fabrication/reporting records and process controls matter for bonded-structure quality/risk evaluation.

### W6D-S06 — ASTM D1002-10(2019)
Title: Standard Test Method for Apparent Shear Strength of Single-Lap-Joint Adhesively Bonded Metal Specimens
Official:
https://store.astm.org/standards/d1002

Current status:
active.

Public support:
the test is primarily comparative and useful for evaluating variables such as surface preparation/environmental durability.

Episode boundary:
a lap-shear coupon result is not automatically a universal design allowable for another joint geometry/service state.

## 4. Brazing / soldering source family

### W6D-S07 — ISO 13585:2021
Title: Brazing — Qualification testing of brazers and brazing operators
Official:
https://www.iso.org/standard/75561.html

Current status checked:
- published/current;
- expected to be replaced by ISO/FDIS 13585 Edition 3.

Public support:
brazing personnel qualification is process/application scoped.

Episode use:
brazing is a controlled thermal/filler/wetting process; exact qualification remains application specific.

### W6D-S08 — IPC J-STD-001J
Owner: IPC
Title: Requirements for Soldered Electrical and Electronic Assemblies
Current revision: J, April 2024
Sources:
https://www.ipc.org/news-release/ipc-releases-j-revisions-two-leading-standards-electronics-assembly
https://www.ipc.org/ipc-document-revision-table

Public support:
electronics soldering has process/material requirements and acceptance frameworks in its intended industry context.

Episode use:
electronics soldering example only.

Guardrail:
IPC J-STD-001J is not generalized to structural brazing/welding or every soldered hardware application.

## 5. Mechanical fastening source family

### W6D-S09 — ISO 898-1:2013
Title: Mechanical properties of fasteners made of carbon steel and alloy steel — Part 1
Official:
https://www.iso.org/standard/60610.html

Current status:
- published/current;
- confirmed 2025;
- revision project exists.

Public support:
fastener mechanical properties are tied to property classes/material/scope.

### W6D-S10 — ISO 16047:2005 + Amd1:2012
Title: Fasteners — Torque/clamp force testing
Official:
https://www.iso.org/standard/27788.html
Amendment:
https://www.iso.org/standard/61463.html

Current status:
current/confirmed.

Public support:
torque and clamp force are related through a test context; torque is not itself a universal direct measure of achieved preload independent of joint/friction conditions.

Episode use:
fastener preload/torque-context lesson.

Guardrail:
no universal torque-to-preload conversion or tightening value.

## 6. Shared EP14 engineering claims

### W6D-C01 — joining process selection starts from joint function and service consequence, not process familiarity or static strength alone
Status: V6 SYNTHESIS supported by all source families.

### W6D-C02 — joining route changes the product/process evidence envelope
Status: VERIFIED PREMISE + V6 SYNTHESIS.
Examples:
heat input/metallurgy/distortion; surface/cure; filler/wetting; preload/friction; inspection/repair.

### W6D-C03 — welding procedure qualification, personnel qualification and production-joint evidence are distinct questions
Status: VERIFIED PUBLIC SCOPE.
Sources: W6D-S01/S02/S03.

### W6D-C04 — adhesive surface preparation is part of the bonding process
Status: VERIFIED.
Source: W6D-S04.

### W6D-C05 — adhesive fabrication/process records matter because final inspection alone may not reconstruct every consequential process variable
Status: VERIFIED PREMISE.
Source: W6D-S05.

### W6D-C06 — standardized adhesive coupon results are not automatically transferable as universal joint design allowables
Status: VERIFIED.
Source: W6D-S06.

### W6D-C07 — brazing/soldering performance depends on material/filler/wetting/cleanliness/thermal-cycle/joint-geometry context
Status: VERIFIED PREMISE + V6 SYNTHESIS.
Sources: W6D-S07/S08.

### W6D-C08 — threaded-fastener torque is not a universal proxy for achieved clamp load independent of joint/friction state
Status: VERIFIED PREMISE + V6 SYNTHESIS.
Sources: W6D-S09/S10.

### W6D-C09 — serviceability, inspectability and rework/repair should be part of joining-process selection where they affect lifecycle risk/cost
Status: V6 SYNTHESIS + Season1 EP07/EP10.

### W6D-C10 — hybrid joints can solve multiple functions while also adding interacting failure modes/process controls
Status: V6 SYNTHESIS.

### W6D-C11 — prototype/coupon success does not automatically establish serial-process capability for the real joint geometry/process/operator/equipment/environment
Status: DEPENDENCY — A4/Wave02/Wave03.

### W6D-C12 — exact qualification/acceptance/operator requirements remain industry/product/joint-specific
Status: APPLICABILITY GUARDRAIL.

## 7. Revision watch

Recheck before final Claude dialogue freeze/publication if named materially:
- ISO 15614-1:2017 — replacement revision is advanced.
- ISO 9606-1:2012 — revision active.
- ISO 13585:2021 — FDIS replacement imminent.
- ISO 21368:2022 — replacement project underway.
- ISO 898-1:2013 — revision project exists.
- IPC J-STD-001J — current public revision as checked 2026-09-19.

## 8. Hard guardrails

1. no universal welding procedure/qualification code;
2. no claim every welded product requires ISO 3834/15614/9606;
3. no universal weld heat input, preheat, acceptance defect level or NDT method;
4. no universal adhesive surface-prep recipe;
5. no universal adhesive cure/bondline/strength value;
6. no lap-shear coupon → arbitrary joint allowable shortcut;
7. no universal brazing/soldering filler or thermal cycle;
8. no IPC electronics requirement generalized outside applicability;
9. no universal fastener torque value or torque-to-preload equation;
10. no “strongest process wins” ranking;
11. no hybrid-joint benefit without considering added interfaces/process controls;
12. all qualification/customer/regulatory obligations remain scoped.

## 9. Episode gate

EP14 can proceed to claim lock/technical review using process-selection principles without clause-level standards teaching.

Current generic-script P0 blockers: 0.
