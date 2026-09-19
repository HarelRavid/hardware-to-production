# HISTORICAL / SUPERSEDED SOURCE REGISTER

status: SUPERSEDED BY `SOURCE_LOCK_WAVE_06H_SURFACE_CLEANING_HEAT_TREATMENT_REGISTER.md`
superseded: 2026-09-19

Preserved for source-research history only. Do not use as current EP18 claim authority.

---

# Source-Lock Wave 06H — Surface Engineering / Cleaning / Heat Treatment Shared Source Register

status: SHARED SOURCE REGISTER LOCKED
checked: 2026-09-19
scope: EP18 — Surface Engineering, Cleaning and Heat Treatment
dependencies: Wave 06D joining + Wave 06C metals + Wave 02 measurement/quality + Wave 01 configuration/change

## 1. Purpose

Lock the authoritative/public premises required to teach post-primary-process state transformations:

incoming material/surface state
→ cleaning/preparation
→ coating/finish/thermal process
→ dimensional/property side effects
→ verification
→ rework
→ downstream compatibility.

EP18 is not a coating-selection catalogue or heat-treatment recipe course.

## 2. Surface preparation / coating source family

### W6H-S01 — ISO 8501-3:2025
Title: Preparation of steel substrates before application of paints and related products — Visual assessment of surface cleanliness — Part 3
Official:
https://www.iso.org/standard/78818.html

Current status:
Edition 3; published 2025-08.

Public support:
surface imperfections/preparation state can matter to later corrosion-protection performance.

Use:
surface preparation is an engineering/process state.

Scope guard:
steel/paint preparation context only.

### W6H-S02 — ISO 8501-4:2020
Title: Preparation of steel substrates before application of paints and related products — Visual assessment of surface cleanliness — Part 4
Official:
https://www.iso.org/standard/73861.html

Current status:
Edition 2; confirmed 2026; current.

Public support:
cleanliness/preparation state after water jetting is explicitly characterized, including flash-rust condition.

Use:
“looks clean” is not a universal engineering acceptance statement.

### W6H-S03 — ISO 12944-1:2017
Title: Paints and varnishes — Corrosion protection of steel structures by protective paint systems — Part 1
Official:
https://www.iso.org/standard/64833.html

Current status:
published/current but revision underway.

Public support:
corrosion-protection paint systems are selected as systems within project/environment context.

### W6H-S04 — ISO 12944-5:2019
Title: Paints and varnishes — Corrosion protection of steel structures by protective paint systems — Part 5
Official:
https://www.iso.org/standard/77795.html

Current status:
published/current; revision underway.

Public support:
coating system selection depends on environment/surface-preparation context.

Guardrail:
ISO 12944 steel-structure rules are not generalized to arbitrary hardware materials/products.

### W6H-S05 — ISO 9227:2022
Title: Corrosion tests in artificial atmospheres — Salt spray tests
Official:
https://www.iso.org/standard/81744.html

Current status:
Edition 5; current; one amendment exists.

Public support:
salt-spray testing is a defined laboratory method for specific corrosion-protection assessments.
The standard does NOT define universal exposure duration or universal product-result interpretation.

Use:
accelerated corrosion test ≠ universal service-life proof.

## 3. Heat-treatment / pyrometry source family

### W6H-S06 — SAE AMS2750H
Title: Pyrometry
Official:
https://saemobilus.sae.org/standards/ams2750h-pyrometry

Current status:
Revision H; revised 2024-07-15; current SAE record.

Public support:
temperature sensors, instrumentation, thermal-processing equipment, system accuracy tests and temperature-uniformity surveys are part of controlled thermal-processing equipment evidence.

Use:
furnace setpoint alone is not the whole thermal-processing evidence.

Scope guard:
AMS2750H is aerospace-material/thermal-processing context; not universally mandatory.

### W6H-S07 — AIAG CQI-9 Heat Treat System Assessment 4th Edition
Official:
https://www.aiag.org/training-and-resources/manuals/details/CQI-9

Current status checked:
- 4th Edition remains current public AIAG listing;
- AIAG states a new version is anticipated in Q4 2026.

Public support:
automotive heat-treatment quality systems assess process control/pyrometry/process tables and variation-reduction practices.

Use:
industry example of heat treatment as a controlled special process.

Guardrail:
automotive applicability only; exact CQI-9 requirements remain protected/manual specific.

## 4. Metal-state / distortion dependency

### W6H-S08 — NIST residual stress / machining-distortion mechanism
Dependency:
Wave 06C / NIST residual-stress study.

Use:
thermal/mechanical history can affect later dimensional stability.

### W6H-S09 — Surface / joining dependency
Dependency:
Wave 06D adhesive-bonding source lock.

Use:
cleanliness/surface preparation can affect joining performance.

## 5. EP18 engineering claims

### W6H-C01 — final product definition can include surface, cleanliness and metallurgical state, not only geometry/material designation
Status: VERIFIED PREMISE + V6 SYNTHESIS.
Sources: W6H-S01–S07.

### W6H-C02 — cleaning should be defined by contamination/function/downstream process and verification need rather than “looks clean”
Status: VERIFIED PREMISE + V6 SYNTHESIS.
Sources: W6H-S01/S02 + Wave06D.

### W6H-C03 — surface preparation is part of coating/bonding process state
Status: VERIFIED.
Sources: W6H-S01/S02 + Wave06D adhesive sources.

### W6H-C04 — coating/finish selection is a system decision involving substrate, preparation, environment, thickness, masking, geometry and downstream operations
Status: VERIFIED PREMISE + V6 SYNTHESIS.
Sources: W6H-S03/S04.

### W6H-C05 — coating/thickness/masking can affect fit, sealing, threads, electrical/thermal contact or other functional interfaces
Status: V6 SYNTHESIS + surface-engineering domain evidence.

### W6H-C06 — accelerated corrosion-test results are test-method/product-context evidence, not automatic field-life equivalence
Status: VERIFIED.
Source: W6H-S05.

### W6H-C07 — heat treatment is a material-state transformation; furnace setpoint/program alone does not necessarily describe actual part thermal history
Status: VERIFIED PREMISE + V6 SYNTHESIS.
Sources: W6H-S06/S07 + heat-treatment domain.

### W6H-C08 — load, fixture, atmosphere, transfer/quench/cooling and geometry can matter to heat-treatment outcome where applicable
Status: VERIFIED PREMISE + V6 SYNTHESIS.
Sources: W6H-S06/S07 + domain evidence.

### W6H-C09 — heat treatment can create distortion/residual-stress/property changes that affect later machining/GD&T/surface operations
Status: VERIFIED PREMISE + V6 SYNTHESIS.
Source: W6H-S08 + Wave06C.

### W6H-C10 — rework/stripping/recoat/reheat can create a new product/process state and require impact reassessment
Status: V6 SYNTHESIS + Wave01 invariant.

### W6H-C11 — process sequence matters because one operation can create or destroy the state needed by the next operation
Status: V6 SYNTHESIS + EP19 preview.

### W6H-C12 — exact heat-treatment/coating/cleanliness requirements remain material/process/product/industry specific
Status: APPLICABILITY GUARDRAIL.

## 6. Revision watch

Recheck before final Claude dialogue freeze/publication:
- AMS2750H current SAE status.
- CQI-9: 4th Edition current listing; AIAG anticipates new version Q4 2026.
- ISO 12944 Parts 1/4/5 revision status.
- ISO 9227:2022 amendment/current status.

## 7. Hard guardrails

1. no universal cleanliness acceptance criterion;
2. no universal coating thickness;
3. no universal salt-spray duration/service-life interpretation;
4. no universal anodizing/plating/paint/passivation recipe;
5. no universal furnace class/TUS/SAT requirement;
6. no universal heat-treatment time/temperature;
7. no hardness value treated as universal proof of full microstructure/properties;
8. no automotive/aerospace special-process requirements generalized;
9. no assumption dimensions measured before treatment remain final dimensions;
10. no stripping/rework treated as neutral;
11. no coating name alone defines corrosion/service performance;
12. exact substrate/material/alloy state must remain visible for any specific process claim.

## 8. Current-status lock

Checked 2026-09-19:
- ISO 8501-3:2025 current.
- ISO 8501-4:2020 current/confirmed 2026.
- ISO 12944-1:2017 current with revision underway.
- ISO 12944-5:2019 current with revision underway.
- ISO 9227:2022 current.
- AMS2750H current SAE revision (2024).
- AIAG CQI-9 4th Edition current listing; next version anticipated Q4 2026.

## 9. Episode gate

EP18 can proceed to claim lock/technical review without product-specific coating, cleaning or thermal-process numerical requirements.

Current generic-script P0 blockers: 0.
