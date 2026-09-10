# Source-Lock Index — Hardware-to-Production

status: ACTIVE — PUBLICATION EVIDENCE PHASE
updated: 2026-09-10
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

### Wave 02 — Quality Chain + Supplier Approval Evidence
Status: **NEXT**

Backbone:
- P2.03 Quality Chain
- P2.06 Supplier Industrialization where PPAP/FAI/change evidence overlaps

Primary episode families:
- EP23/24
- EP28/30 where quality/supplier evidence is reused
- EP32/33
- EP38/39/40
- EP56 automotive methods

Source targets:
- AIAG Core Tools current editions/status;
- APQP / Control Plan / PPAP / FMEA / MSA / SPC applicability;
- IAQG 9102 FAI distinction where needed;
- NIST/authoritative statistics/metrology support;
- customer-specific requirements only when deliberately selected.

Hard rule:
Do not infer manual content from public marketing/index pages. Exact normative/quasi-normative claims require controlled source text.

### Wave 03 — Pilot / Capacity / Ramp / Economics
Status: PLANNED

Backbone:
- P2.04
- P2.05

Primary episodes:
- EP26–31
- EP41–46 economics/rate dependencies
- EP55 startup scale application
- EP60 synthesis

Source targets:
- NASA PRR/readiness guidance;
- manufacturing-readiness source family where current authoritative access is available;
- operations/capacity equations;
- finance/economic-method references;
- independent arithmetic lock of Sentinel examples.

### Wave 04 — Automation / Machinery Safety / OEE
Status: PLANNED

Backbone:
- P2.07

Primary episodes:
- EP41–46
- supporting EP25/29/52/59 interfaces

Source targets:
- ISO 12100;
- ISO 13849 series;
- IEC 62061;
- ISO 10218 series;
- IEC 60204-1;
- OEE authoritative definition/formula source;
- jurisdiction-specific machinery safety kept separate.

### Wave 05 — Manufacturing Atlas / Digital Thread / OT Security
Status: PLANNED

Backbone:
- P2.08
- P2.09

Primary episodes:
- EP35
- EP47–52
- EP59 recovery/configuration reuse

Source targets:
- ISA-95 / IEC 62264;
- OPC UA / companion-specification boundaries;
- NIST digital-thread/manufacturing-data guidance;
- IEC 62443 family;
- NIST SP 800-82 Rev.3.

### Wave 06 — Manufacturing Process Families
Status: PLANNED

Primary episodes:
- EP11–19
- DFM/DFA/tolerance support from EP06–09

Source lock will be split by process family rather than one giant wave if source burden becomes too heterogeneous:
- polymers;
- metals/machining/forming/casting;
- joining;
- composites;
- ceramics/powders/sintering;
- additive;
- surface/cleaning/heat treatment;
- process-chain selection.

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
