# Source-Lock Index — Hardware-to-Production

status: ACTIVE — SEASON-FIRST EVIDENCE / HANDOFF PHASE
updated: 2026-09-19
purpose: Canonical index for shared-source-family evidence locking after completion of the 68-asset production architecture.

## Rule

Source lock is organized by **shared evidence family**, not by episode number.

A source may support many episodes, but reuse is valid only when:
1. the claim meaning matches;
2. applicability matches;
3. source version/status is still current for the intended statement;
4. no downstream episode turns guidance into a stronger normative claim.

Source lock does not equal PODCAST READY.

Pipeline:
`Production Blueprint → Source/Claim Lock → Technical Review → Script/Outline → Editorial/Source Notes → PODCAST READY`

## Wave status

### Wave 01 — Requirements / Verification / Configuration
Status: **PASS — CORE EVIDENCE LOCKED**

Primary scope:
- A1 Requirements
- A7 Verification
- A8 Configuration
- P2.02 Configuration & Change Control

Canonical records:
- `evidence/source-lock/wave-01/WAVE_01_MANIFEST.md`
- `evidence/source-lock/wave-01/W1_SHARED_SOURCE_REGISTER.md`
- `evidence/source-lock/wave-01/W1_A1_A7_A8_CLAIM_LOCK.md`

Primary source families:
- NASA Systems Engineering Handbook §§4, 5.3, 6.2, 6.5 + appendices;
- NASA NPR 7123.1D for NASA-specific applicability/current procedural context;
- ISO/IEC/IEEE 29148:2018 official status/scope watch;
- ISO 10007:2017 official status/scope watch.

### Season 1 — Handoff Completion Locks
Status: **PASS — 18/18 CLAUDE HANDOFF READY**

Shared completion registers:
- `evidence/source-lock/SOURCE_LOCK_SEASON_1_S1A_OPENING_FOUNDATIONS_REGISTER.md`
- `evidence/source-lock/SOURCE_LOCK_SEASON_1_S1B_READINESS_NPI_REGISTER.md`
- `evidence/source-lock/SOURCE_LOCK_SEASON_1_S1C_DFX_TEST_TOL_RELIABILITY_REGISTER.md`

Technical reviews:
- `evidence/source-lock/season-1/S1A_INTERNAL_TECHNICAL_REVIEW.md`
- `evidence/source-lock/season-1/S1B_INTERNAL_TECHNICAL_REVIEW.md`
- `evidence/source-lock/season-1/S1C_INTERNAL_TECHNICAL_REVIEW.md`

Season exit:
- `podcast/season-1/SEASON_1_CLAUDE_HANDOFF_EXIT_AUDIT.md`

Handoff artifacts:
- 18 manifests;
- 18 Claude writing prompts;
- 0 missing mandatory handoff paths.

Season 1 handoff is complete. Season 2 handoff is also complete; current active preparation is Season 3.

### Wave 02 — Quality Chain + Supplier Approval Evidence
Status: **PASS — PUBLICATION PACKAGES COMPLETE FOR CURRENT GENERIC SCRIPT SCOPE**

Direct episode scope:
- EP23 — DFMEA, PFMEA, Control Plans and Quality Gates
- EP24 — Production Testing and Measurement-System Capability
- EP32 — Process Capability / SPC
- EP39 — RFQ Technical Package / First Production Approval
- EP40 — Supplier Quality / Dual Sourcing / Resilience

Canonical records:
- `evidence/source-lock/SOURCE_LOCK_WAVE_02_QUALITY_SUPPLIER_REGISTER.md`
- `evidence/source-lock/wave-02/WAVE_02_MANIFEST.md`
- `evidence/source-lock/wave-02/W2_EP23_EP24_EP32_EP39_EP40_CLAIM_LOCK.md`
- `evidence/source-lock/wave-02/W2_INTERNAL_TECHNICAL_REVIEW.md`
- `evidence/source-lock/wave-02/WAVE_02_PUBLICATION_GATE.md`

Publication packages completed:
- script outlines;
- full script drafts;
- script reviews;
- source notes.

Current source findings checked 2026-09-19:
- APQP 3rd Edition / Control Plan 1st Edition — Mar 2024;
- MSA-4 and PPAP-4 current public AIAG listings;
- AIAG & VDA SPC Manual 1st Edition — Jul 2026;
- IAQG 9102 Rev C public resource/forms family;
- NIST measurement/capability guidance locked for generic technical claims.

Hard rule retained:
Exact protected/manual-specific method details, thresholds, submission levels and customer-specific requirements remain gated. Wave 02 scripts intentionally do not require those details.

### Wave 03 — Pilot / Capacity / Ramp / Economics
Status: **PASS — PUBLICATION PACKAGES COMPLETE FOR CURRENT GENERIC SCRIPT SCOPE**

Direct episode scope:
- EP26 — Pilot Build Planning
- EP27 — Production Validation
- EP28 — Yield / Rework / Scrap
- EP29 — Capacity / Bottlenecks / Takt
- EP30 — Supplier Readiness / Contract-Manufacturer Management
- EP31 — Engineering Changes During Ramp

Canonical records:
- `evidence/source-lock/SOURCE_LOCK_WAVE_03_RAMP_ECONOMICS_REGISTER.md`
- `evidence/source-lock/wave-03/WAVE_03_MANIFEST.md`
- `evidence/source-lock/wave-03/W3_EP26_EP27_EP28_EP29_EP30_EP31_CLAIM_LOCK.md`
- `evidence/source-lock/wave-03/W3_INTERNAL_TECHNICAL_REVIEW.md`
- `evidence/source-lock/wave-03/WAVE_03_PUBLICATION_GATE.md`

Publication packages completed:
- script outlines;
- full script drafts;
- script reviews;
- source notes.

Current authoritative context checked 2026-09-19:
- NASA NPR 7123.1D + Appendix G PRR;
- Lean Enterprise Institute takt/cycle definitions;
- NIST flow/WIP/capacity research;
- NIST AMS 200-5 / 200-11 / Smart Investment Tool family;
- NIST maintenance/investment-return studies.

All current Sentinel capacity/economics arithmetic independently checked.

Hard rule retained:
No universal pilot quantity, PVT definition, Run-at-Rate duration, ramp-release threshold, acceptable yield, discount rate or payback target.

### Wave 04 — Automation / Machinery Safety / OEE
Status: **PASS — PUBLICATION PACKAGES COMPLETE FOR CURRENT GENERIC SCRIPT SCOPE**

Direct episode scope:
- EP41 — When Not to Automate
- EP42 — Building the Business Case for Automation
- EP43 — Semi-Automation, Robotics and Machine Vision
- EP44 — Automated Inspection and End-of-Line Test
- EP45 — Automation Qualification, OEE and Maintenance
- EP46 — Scaling Without Automating Defects

Canonical records:
- `evidence/source-lock/SOURCE_LOCK_WAVE_04_AUTOMATION_SAFETY_OEE_REGISTER.md`
- `evidence/source-lock/wave-04/WAVE_04_MANIFEST.md`
- `evidence/source-lock/wave-04/W4_EP41_EP42_EP43_EP44_EP45_EP46_CLAIM_LOCK.md`
- `evidence/source-lock/wave-04/W4_INTERNAL_TECHNICAL_REVIEW.md`
- `evidence/source-lock/wave-04/WAVE_04_PUBLICATION_GATE.md`

Publication packages completed:
- script outlines;
- full script drafts;
- script reviews;
- source notes.

Current standards/status checked 2026-09-19:
- ISO 12100:2010 current published; revision active;
- ISO 13849-1:2023 current;
- ISO 13849-2:2012 current published; revision active;
- IEC 62061:2021+A1:2024+A2:2026 current consolidated family;
- ISO 10218-1/-2:2025 current;
- IEC 60204-1:2016+A1:2021 current public family;
- IEC 62381:2024 current;
- ISO 22400-2:2014+Amd1:2017 current published; revision active.

All current OEE arithmetic independently checked.

Hard rule retained:
No universal OEE benchmark, safety PL/SIL requirement, FAT/SAT release equivalence, machinery-law obligation or automated-test threshold is inferred without exact applicability/source lock.

### Wave 05 — Manufacturing Atlas / Digital Thread / OT Security
Status: **PASS — PUBLICATION PACKAGES COMPLETE FOR CURRENT GENERIC SCRIPT SCOPE**

Direct episode scope:
- EP47 — Systems of Record
- EP48 — Product Genealogy / Recipes / Parameters / Measurements
- EP49 — Standards / Claims / Evidence Knowledge Graph
- EP50 — Manufacturing Atlas Decision System
- EP51 — OPC UA / ISA-95 / Semantic Integration
- EP52 — Engineering-Grade Manufacturing Data / OT Security

Canonical records:
- `evidence/source-lock/SOURCE_LOCK_WAVE_05_ATLAS_DIGITAL_THREAD_OT_SECURITY_REGISTER.md`
- `evidence/source-lock/wave-05/WAVE_05_MANIFEST.md`
- `evidence/source-lock/wave-05/W5_EP47_EP48_EP49_EP50_EP51_EP52_CLAIM_LOCK.md`
- `evidence/source-lock/wave-05/W5_INTERNAL_TECHNICAL_REVIEW.md`
- `evidence/source-lock/wave-05/WAVE_05_PUBLICATION_GATE.md`

Publication packages completed:
- script outlines;
- full script drafts;
- script reviews;
- source notes.

Current source findings checked 2026-09-19:
- ANSI/ISA-95.00.01-2025 current Part 1;
- NIST Digital Thread updated Aug 2026;
- NIST IR 8536 final Sep 9, 2026;
- NIST SP 800-82 Rev.3 current final;
- IEC 62443 role/status family locked at public-scope level.

Final publication watch:
- recheck IEC 62443-2-1:2024 before EP52 final publication lock because IEC stability date is 2026.

Hard rule retained:
No universal system-of-record assignment, ISA-95 software stack, OPC UA ontology claim, IEC 62443 topology/security level, or legal OT-security obligation is inferred without exact applicability.

### Wave 06 — Manufacturing Process Families
Status: **PASS — 06A–06I COMPLETE; SEASON 2 CLAUDE HANDOFF READY**

Master record:
- `evidence/source-lock/wave-06/WAVE_06_MASTER_MANIFEST.md`

Sub-wave status:
- **06A Process Selection / EP11 — PASS**
- **06B Polymers / EP12 — PASS**
- **06C Metals / EP13 — PASS**
- **06D Joining / EP14 — PASS**
- **06E Composites / EP15 — PASS**
- **06F Ceramics / Powder / Sintering / EP16 — PASS**
- **06G Additive Manufacturing / EP17 — PASS**
- **06H Surface / Cleaning / Heat Treatment / EP18 — PASS**
- **06I Process Chains / EP19 — PASS**

Season 2 handoff:
- `podcast/season-2/SEASON_2_CLAUDE_HANDOFF_EXIT_AUDIT.md`
- 9/9 Handoff Manifests
- 9/9 Claude Writing Prompts
- 24/24 mandatory handoff paths validated

Wave 06 rule retained:
No universal process-family numeric limit, tolerance, material state, tooling threshold or qualification requirement is transferred between sub-waves without exact evidence/applicability.

Current active preparation:
**Season 3 — Production System Engineering**

### Season 3 — Handoff Completion Locks
Status: **PASS — 12/12 CLAUDE HANDOFF READY**

Season exit:
- `podcast/season-3/SEASON_3_CLAUDE_HANDOFF_EXIT_AUDIT.md`

Handoff artifacts:
- 12 manifests;
- 12 Claude writing prompts;
- 30/30 mandatory common + episode handoff paths validated.

Current active preparation:
**Season 4 — EP32–EP40**

### Wave 07 — Case-Study Publication Lock
Status: PARTIALLY PRE-BUILT / PLANNED FINAL LOCK

Primary episodes:
- EP53–59

Existing case evidence packs are strong enough for production blueprints. Final source lock will re-check:
- dates/populations/configurations;
- exact official locators;
- causal wording;
- regulator vs manufacturer attribution;
- legal/regulatory current status;
- domain-transfer boundaries.

EP60 is primarily fictional synthesis from evidence-backed principles and does not require invented external case facts.

## Revision-watch register

Revision watch is mandatory for standards/source families that can change between research and publication.

Current watch examples as of 2026-09-10:
- ISO/IEC/IEEE 29148:2018 — published current edition; Edition 3 revision project active.
- ISO 10007:2017 — published current edition; Edition 4 revision project active.
- IATF 16949 revision — active in 2026; publication status must be rechecked before EP56 script lock.
- EU Machinery Regulation 2023/1230 — general application date 2027-01-20; EP59 must use date-qualified wording until then.

## Publication discipline

Never use `VERIFIED` to mean merely:
- source found;
- plausible;
- commonly taught;
- present in a prior model answer;
- appears in a vendor blog;
- appears in a draft standard.

For V1/P0 claims, verify edition + exact support + applicability before publication.

For V6 frameworks, verify the embedded external premises but keep ownership explicit:
`OUR FRAMEWORK / INTERNAL SYNTHESIS`.
