# Source-Lock Wave 06H — Surface Engineering / Cleaning / Heat Treatment Shared Source Register

status: SHARED SOURCE REGISTER LOCKED
checked: 2026-10-01
scope: EP18 — Surface Engineering, Cleaning and Heat Treatment
dependencies: Wave 06D joining + Wave 06C metals + Wave 01 configuration/change + Wave 02 measurement

## 1. Purpose

Lock the generic engineering premises required to treat cleaning, surface preparation, coatings and heat treatment as controlled state transformations that can change dimensions, properties, interfaces and evidence.

EP18 does not teach one universal surface-treatment or thermal-processing recipe.

## 2. Cleaning / surface-preparation source family

### W6H-S01 — ISO 27831-1:2008
Title: Metallic and other inorganic coatings — Cleaning and preparation of metal surfaces — Part 1: Ferrous metals and alloys
Current status:
reviewed/confirmed 2024/current.
Official:
https://www.iso.org/standard/44347.html

Public support:
- cleaning/preparation is performed to remove unwanted material and prepare surfaces for subsequent treatment;
- the applicable process depends on substrate and downstream coating/treatment context.

Use:
cleaning is a controlled process objective, not “looks clean.”

### W6H-S02 — ISO 27831-2:2008
Title: Cleaning and preparation of metal surfaces — Part 2: Non-ferrous metals and alloys
Current public family listing:
https://www.iso.org/ics/25.220.20/x/

Use:
surface-preparation method is substrate/process specific.

### W6H-S03 — ISO 14644-13:2026
Title: Cleanrooms and associated controlled environments — Part 13: Cleaning of surfaces to achieve defined levels of cleanliness
Edition: 2, published 2026-02.
Official:
https://www.iso.org/standard/91614.html

Public support:
cleaning can be defined against specified particle/chemical surface-cleanliness objectives and associated test methods.

Applicability guard:
cleanroom guidance is not imposed on ordinary manufacturing; used only to demonstrate that “clean” can be a defined/measured state.

## 3. Coating / surface-state measurement family

### W6H-S04 — ASTM E376-26
Title: Measuring Coating Thickness by Magnetic-Field or Eddy Current Methods
Current status:
Active; updated 2026-07-20.
Official:
https://store.astm.org/e0376-26.html

Public support:
measurement suitability depends on coating/substrate combination and instrument limitations; coating thickness is a measurable product/process attribute.

Use:
coating thickness/measurement must match substrate/process/application.

### W6H-S05 — ISO 27830:2017
Title: Metallic and other inorganic coatings — Requirements for designation
Current public listing:
https://www.iso.org/ics/25.220.20/x/

Use:
coating definition/designation is more than generic “finish”; exact coating/system identity matters.

## 4. Heat-treatment / pyrometry source family

### W6H-S06 — AMS2750H
Owner: SAE International
Title: Pyrometry
Current revision:
AMS2750H, 2024-07-15.
Official:
https://saemobilus.sae.org/standards/ams2750h-pyrometry

Public support:
thermal-processing equipment control includes sensors, instrumentation, thermal equipment, system accuracy and temperature uniformity testing to ensure treatment according to applicable specifications.

Use:
thermal recipe execution depends on controlled measurement/equipment, not setpoint text alone.

Applicability guard:
AMS2750H is aerospace material-specification context and is not universal to every heat-treatment process.

### W6H-S07 — ISO 15787:2016
Title: Technical product documentation — Heat-treated ferrous parts — Presentation and indications
Edition: 2; confirmed 2024/current.
Official:
https://www.iso.org/standard/56851.html

Public support:
final heat-treated condition can be part of technical product definition.

Use:
heat-treatment state belongs in product/configuration definition.

## 5. Residual stress / sequence dependency

### W6H-S08 — NIST residual-stress / machining distortion research
Reuse Wave06C:
prior thermal/mechanical state can affect downstream dimensional behavior.

Use:
process sequence can move dimensions/state after earlier inspection.

## 6. EP18 engineering claims

### W6H-C01 — final product definition can include surface/chemical/metallurgical state, not only geometry/material name
Status: VERIFIED PREMISE + V6 SYNTHESIS.
Sources: W6H-S05/S07.

### W6H-C02 — cleaning should be defined by contamination/removal/next-process objective where consequential, not visual appearance alone
Status: VERIFIED PREMISE.
Sources: W6H-S01/S02/S03.

### W6H-C03 — surface preparation is a process input to downstream coating/bonding performance
Status: VERIFIED.
Sources: W6H-S01/S02 + EP14 adhesive evidence.

### W6H-C04 — coatings can change dimensions, interfaces, friction, electrical/thermal behavior, corrosion/wear protection and inspection requirements depending on application
Status: V6 SYNTHESIS supported by W6H-S04/S05.

### W6H-C05 — masking/selective treatment belongs in product/process definition when untreated/treated regions have different functional requirements
Status: V6 SYNTHESIS.

### W6H-C06 — heat treatment is a material-state transformation and execution evidence can depend on equipment/instrumentation/thermal uniformity as required by the applicable process/specification
Status: VERIFIED PREMISE.
Sources: W6H-S06/S07.

### W6H-C07 — thermal/surface processes can change dimensions or invalidate earlier measurement/evidence
Status: VERIFIED PREMISE + V6 SYNTHESIS.
Sources: W6H-S08 + Wave01.

### W6H-C08 — stripping/recoat/reheat/rework can create a new process/configuration history and cannot be assumed equivalent to original state
Status: V6 SYNTHESIS + global rework-history invariant.

### W6H-C09 — process sequencing should consider what the next operation requires and what the current process leaves behind
Status: V6 SYNTHESIS.

### W6H-C10 — final inspection location should account for later transformations that can invalidate dimensions/surface/property evidence
Status: V6 SYNTHESIS + Wave01/02.

## 7. Hard guardrails

1. no universal cleanliness level;
2. no universal cleaning chemistry/process;
3. no universal coating thickness;
4. no universal corrosion-test equivalence;
5. no universal heat-treatment recipe;
6. no furnace class/uniformity requirement generalized from AMS2750H;
7. no AMS aerospace requirement generalized;
8. no coating/heat-treatment rework assumed equivalent;
9. no inspection-before-final-transformation treated as final evidence by default;
10. exact alloy/coating/material process remains application-specific.

## 8. Current-status lock

Checked 2026-10-01:
- ISO 27831-1:2008 current/confirmed 2024.
- ISO 27831-2:2008 current public listing.
- ISO 14644-13:2026 current, cleanroom scope only.
- ASTM E376-26 active.
- ISO 27830:2017 current public listing.
- AMS2750H current SAE revision, July 2024.
- ISO 15787:2016 current/confirmed 2024.

## 9. Episode gate

Current generic-script P0 blockers: 0.
