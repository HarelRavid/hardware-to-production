# Source-Lock Wave 01 — Requirements, Verification & Configuration

status: COMPLETE — EVIDENCE LOCKED FOR CURRENT NON-NORMATIVE SCRIPT SCOPE
opened: 2026-09-10
closed: 2026-09-10
baseline_head_at_open: 37c5210433bcb26e06b93d8fc670aee7698581d2
scope_type: shared-source-family wave

## 1. Purpose

Lock one authoritative evidence layer that can be reused across the podcast instead of re-researching requirements, verification and configuration-management premises episode by episode.

This wave does **not** make a claim PODCAST READY by itself. It advances the selected claims from source discovery to evidence lock. Technical review and script/source-note packaging remain separate gates.

## 2. Primary scope

Direct episode scope:
- A1 — From an Idea to Engineering Requirements
- A7 — Verification Planning Before DVT/PVT Thinking
- A8 — Configuration Management from Prototype #1

Backbone scope:
- P2.02 — Configuration & Change Control
- selected P2.01 readiness/requirements interfaces where they rely on the same NASA systems-engineering source family

Downstream reuse candidates:
- EP01–EP05 readiness / industrialization transition
- EP20–EP31 controlled production / engineering change
- EP35 genealogy/evidence retention
- EP39 supplier approval/change
- EP53 case reconstruction
- EP60 full decision story

Reuse is allowed only when the downstream claim has the same meaning and applicability. This wave is not a blanket citation license.

## 3. Locked source family

Canonical shared source register:
`evidence/source-lock/wave-01/W1_SHARED_SOURCE_REGISTER.md`

Claim lock:
`evidence/source-lock/wave-01/W1_A1_A7_A8_CLAIM_LOCK.md`

## 4. Source strategy

The wave intentionally separates **open authoritative engineering guidance** from **licensed normative standards**.

### Open sources used for evidence lock
NASA Systems Engineering Handbook web content is used for requirements definition/management, product verification and configuration management because it provides public, inspectable section-level support.

NASA applicability is always explicit: NASA handbook/process language is authoritative for NASA practice/guidance, not a universal contractual requirement for commercial hardware teams.

### Standards used as status/scope controls
- ISO/IEC/IEEE 29148:2018
- ISO 10007:2017

Their official ISO records are used to lock title, edition, publication/current-status and scope-level metadata.

They are **not** used to support clause-level SHALL claims in this wave because no controlled licensed full-text copy is present in the repository.

## 5. Standards status locked on 2026-09-10

### ISO/IEC/IEEE 29148
Current published edition:
`ISO/IEC/IEEE 29148:2018`, Edition 2, published 2018-11.

Official ISO lifecycle status checked:
- current published standard remains 2018 edition;
- revision activity is active;
- Edition 3 DIS is under development in 2026.

Rule:
The DIS must not be cited as the current published normative edition.

### ISO 10007
Current published edition:
`ISO 10007:2017`, Edition 3, published 2017-03.

Official ISO lifecycle status checked:
- current published standard remains 2017 edition;
- revision activity is active;
- Edition 4 working-draft project is under development.

Rule:
The draft project must not be treated as having replaced ISO 10007:2017.

## 6. Wave-level source-vs-synthesis boundary

### External premises locked
The source family supports these premises:
- requirements should be explicit, managed and traceable;
- technical requirements include functional/performance/interface and crosscutting constraints;
- requirements change should be impact-assessed and controlled;
- verification should be planned against defined requirements and documented procedures/conditions;
- verification records should preserve the verified product version, requirement version, method/equipment context, anomalies and results;
- configuration management includes planning, identification, change management, status accounting and verification;
- baselines provide a known configuration against which change is managed;
- approved change management includes proposal/evaluation, incorporation and verification of implementation.

### Internal synthesis retained
These remain Hardware-to-Production frameworks, not NASA/ISO requirements:
- Minimum Useful Requirements Sheet;
- Requirement Quality Check;
- Verification Intent Sheet;
- Evidence-to-Claim Review;
- Minimum Prototype Configuration Record;
- Change Impact Check;
- DEV/LVP/SVP Lens;
- shortcut-expiration logic;
- `Definition → As-built/As-run → Evidence` formulation;
- `rework adds history` invariant;
- targeted evidence invalidation / re-verification based on affected dependencies.

## 7. Gate result

A1: `EVIDENCE VERIFIED FOR CURRENT NON-NORMATIVE SCRIPT SCOPE — TECHNICAL REVIEW PENDING`

A7: `EVIDENCE VERIFIED FOR CURRENT NON-NORMATIVE SCRIPT SCOPE — TECHNICAL REVIEW PENDING`

A8: `EVIDENCE VERIFIED FOR CURRENT NON-NORMATIVE SCRIPT SCOPE — TECHNICAL REVIEW PENDING`

P2.02 shared backbone: `CORE AUTHORITATIVE SOURCE LOCKED — INDUSTRY-SPECIFIC/NORMATIVE EXTENSIONS REMAIN AS NEEDED`

## 8. Remaining hard gates

Before any of A1/A7/A8 becomes PODCAST READY:
1. technical review by a competent systems/test/configuration practitioner;
2. exact source-note packaging for every consequential external statement actually retained in the script;
3. if ISO 29148 or ISO 10007 is quoted or presented normatively, obtain controlled licensed full text and verify exact clause/edition/applicability;
4. product-specific safety/regulatory claims remain outside this generic wave and require product/jurisdiction evidence;
5. measurement-system claims deeper than the A7 preview remain owned by P2.03 / later quality source lock;
6. supplier-change obligations deeper than the A8 preview remain owned by P2.06 / supplier source lock.

## 9. Decision

**SOURCE-LOCK WAVE 01: PASS**

The selected episode architecture does not require redesign. Source work now supports moving A1/A7/A8 into technical review without using unsupported standards language.
