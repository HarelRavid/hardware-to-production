# Supplier Industrialization / Qualification / Change Control — Evidence Source Map

status: IN PROGRESS — FAI/PPAP/CRITICAL-PROCESS BACKBONE CAPTURED
campaign: A6
maps_to: MASTER_WBS Section 7 and 5.8; PODCAST_MAP Episodes 30, 37–40
provenance: primary-source-first

## Purpose
Build the evidence backbone for selecting, qualifying and scaling suppliers based on demonstrated manufacturing capability, quality systems, process control, capacity, change discipline and resilience rather than quotation quality or presentation quality alone.

## Source backbone

### NIST MEP supplier selection / TCO / resilience guidance
Evidence role:
- supplier capability includes quality, workforce, equipment, maintenance, logistics and total cost of ownership;
- capability and capacity are separate questions;
- resilience requires understanding sub-tier and common-mode dependencies.

### SAE AS9102C — First Article Inspection Requirements
Evidence role:
- establishes requirements for performing and documenting First Article Inspection (FAI);
- FAI verifies a defined first-article/configuration and manufacturing-process result;
- standard is aerospace-specific and complementary to customer/statutory/regulatory requirements.
Applicability boundary: AS9102C is not a universal supplier-qualification rule outside its applicable aerospace/customer context.

### AIAG PPAP
Evidence role:
- focuses on demonstrating that supplier production processes can produce parts meeting engineering requirements consistently during an actual production run at production rates;
- ties production-part approval to engineering records/specifications and production evidence;
- includes submission, notification and resubmission/change rules in automotive/customer-specific contexts.
Applicability boundary: PPAP is an automotive/customer-specific framework and should be used as transferable engineering evidence only where not contractually applicable.

### PRI / Nadcap critical-process accreditation
Evidence role:
- demonstrates an industry-managed accreditation model for critical/special processes in aerospace, defense and space;
- audit criteria are process-specific and industry governed;
- recurring audits and performance oversight reinforce that critical-process qualification is not a one-time paperwork event;
- relevant process families include heat treatment, welding, NDT, surface enhancement, electronics and other critical processes.
Applicability boundary: Nadcap accreditation is sector/customer specific; the transferable principle is that some critical processes require process-specific technical control beyond generic final inspection.

## Core boundary: FAI vs PPAP vs ongoing capability
### First Article Inspection (FAI)
Primary question: did the defined first production/configuration article and associated documentation satisfy the specified design characteristics and FAI requirements?

### Production Part Approval / production-process approval
Primary question: does the production process, under actual production conditions/rates and defined controls, demonstrate ability to consistently meet engineering requirements?

### Ongoing serial capability
Primary question: after approval, does the process remain controlled/capable as people, materials, tools, maintenance, environment, suppliers and time change?

Editorial rule: a conforming first article is necessary evidence in many contexts but is not equivalent to production-rate or long-term capability evidence.

## Supplier change-control model
Potential qualification-impacting changes include, where applicable:
- product/design revision;
- material/source change;
- manufacturing-process or sequence change;
- equipment/tooling/fixture change;
- production location/site/line transfer;
- software/firmware/test-method revision;
- inspection/measurement-system change;
- sub-tier or special-process supplier change;
- significant maintenance/rebuild affecting process state;
- capacity/rate change that alters process conditions.

Decision sequence:
Change proposed -> applicability/risk review -> customer/internal notification requirement -> evidence impact -> required requalification/resubmission/FAI/PPAP/test -> approved effectivity/cut-in -> genealogy/traceability -> post-change monitoring.

## Critical / special-process principle
Some process outputs cannot be adequately assured by inspecting only the finished product. Supplier qualification may therefore need to evaluate the process itself, including:
- procedure/specification control;
- equipment qualification/calibration;
- operator/personnel qualification;
- material/consumable control;
- process parameters and records;
- heat/lot/load traceability;
- maintenance and environmental controls;
- destructive/NDT validation where applicable;
- sub-tier approval and flow-down.

Do not generalize one sector's accreditation scheme to all industries; preserve applicability.

## Supplier qualification ladder
1. Can they quote the requirement?
2. Do they understand the engineering requirement and CTQs?
3. Do they possess the required process/material capability?
4. Can they produce a conforming first article?
5. Can they repeat it under controlled production conditions?
6. Can they demonstrate measurement/process control?
7. Can they achieve required production rate/capacity?
8. Can they control changes and maintain qualification evidence?
9. Can they manage critical sub-tier/special-process dependencies?
10. Can the supply route survive foreseeable disruptions?

## Claim register

### C-SUP-001 — Lowest supplier quote is not sufficient evidence of lowest total manufacturing cost or risk
status: STRONG
Evidence basis: NIST MEP supplier-selection/TCO guidance + A3.

### C-SUP-002 — Supplier selection and supplier qualification are different decisions
status: STRONG SYNTHESIS
Selection chooses a candidate; qualification demonstrates suitability for the defined product/process/configuration and evidence requirement.

### C-SUP-003 — A conforming first article does not by itself prove serial process capability
status: STRONG
Evidence basis: AS9102C addresses FAI, while AIAG PPAP explicitly addresses consistent production during actual production runs at production rates.

### C-SUP-004 — Supplier capability includes process, measurement, tooling, people and capacity, not only nominal machine list
status: STRONG DIRECTION
Evidence basis: NIST supplier guidance + PPAP/process-readiness logic.

### C-SUP-005 — Supplier/sub-tier/process changes can invalidate prior qualification evidence
status: STRONG
Evidence basis: PPAP notification/resubmission framework plus configuration/effectivity principles.
Boundary: exact notification/requalification rules are industry/customer specific.

### C-SUP-006 — Dual sourcing is not automatically resilience if two sources share the same hidden sub-tier/process/geographic dependency
status: STRONG SYNTHESIS
Evidence basis: NIST supply-chain resilience guidance encouraging sub-tier/common-dependency mapping.

### C-SUP-007 — Supplier performance metrics should include more than on-time delivery and incoming rejects
status: STRONG SYNTHESIS
Potential dimensions: escapes, responsiveness, process changes, CAPA effectiveness, capacity, lead-time stability and quality-at-source.

### C-SUP-008 — Some critical/special processes require qualification/control of the process itself, not only final-product inspection
status: STRONG WITH SECTOR APPLICABILITY
Evidence basis: PRI/Nadcap process-specific accreditation framework and recurring oversight in aerospace/defense/space.

### C-SUP-009 — Supplier approval is configuration/effectivity dependent
status: STRONG SYNTHESIS
A supplier approved for one part revision, material, process route, site, tooling state or sub-tier chain is not automatically approved for materially changed conditions.

## DEV / LVP / SVP lens
### DEV
Use suppliers for speed/learning but record process, material and configuration assumptions. Avoid accidental sole-source lock-in where future scale is foreseeable.

### LVP
Qualify critical suppliers/processes enough to support repeatable tens/hundreds: controlled drawing/spec revision, material certificates where needed, agreed inspection/test, change notification, traceable lots, first-article evidence and capacity assumptions.

### SVP
Formalize supplier approval, production validation, capacity/rate evidence, ongoing performance monitoring, sub-tier/special-process controls, change governance, resilience and recovery plans according to risk/industry/customer requirements.

## Myth register
- 'The first article passed, so the supplier is qualified for production' — REJECT as universal claim.
- 'PPAP and FAI are basically the same thing' — REJECT.
- 'An ISO 9001 certificate proves the supplier can make my part' — REJECT as universal claim.
- 'Two approved suppliers means we have resilient dual sourcing' — REJECT as universal claim.
- 'If final inspection passes, the special process is controlled' — REJECT as universal claim.
- 'Once approved, a supplier stays approved regardless of process/site/sub-tier changes' — REJECT.

## Breadth gaps to close
1. stronger supplier-change notification examples beyond automotive PPAP;
2. ongoing supplier-performance/scorecard evidence;
3. capacity/run-at-rate examples at supplier;
4. sub-tier/special-process escape case studies;
5. dual-source hidden-common-mode case studies;
6. industry comparison: general manufacturing vs automotive vs aerospace/medical.

## Pass-2 targets
- worked supplier capability audit/checklist;
- FAI vs PPAP vs ongoing capability comparison;
- supplier change/effectivity case;
- sub-tier/special-process escape case;
- supplier capacity/run-at-rate example;
- dual-source hidden-common-mode example;
- supplier TCO comparison;
- critical-process applicability map by sector.

## Readiness
Source map: IN PROGRESS — FAI/PPAP/CRITICAL-PROCESS BACKBONE CAPTURED
Critical claims identified: YES
Primary-source backbone: STRONG FOR FAI/PPAP/CRITICAL-PROCESS PRINCIPLES
Applicability conflicts visible: YES
Resilience/case depth: PARTIAL
Podcast Ready: NO