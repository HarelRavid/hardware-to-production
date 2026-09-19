# Source-Lock Wave 06H — Surface Engineering / Cleaning / Heat Treatment Shared Source Register

status: SHARED SOURCE REGISTER LOCKED
checked: 2026-09-19
scope: EP18 — Surface Engineering, Cleaning and Heat Treatment
dependencies: EP14 joining + Wave02 measurement/quality + Wave01 configuration/change + EP13/17 material-state context

## 1. Purpose

Lock the public/authoritative premises required to teach post-primary-process state transformations without treating cleaning, coatings or heat treatment as cosmetic finishing.

EP18 owns:
- cleanliness as a defined functional/process state;
- surface preparation/coating/masking/thickness;
- heat treatment as material-state transformation;
- sequencing/interactions;
- rework/stripping/change impact.

## 2. Cleanliness / surface-preparation source family

### W6H-S01 — ISO 14644-9:2022
Title: Cleanrooms and associated controlled environments — Part 9: Assessment of surface cleanliness for particle concentration
Official:
https://www.iso.org/standard/76889.html

Current status:
Edition 2; published/current.

Public support:
surface cleanliness can be defined/measured by particle concentration using scoped methods in controlled-environment applications.

Episode use:
“clean” must be defined by contaminant/measurement/application, not appearance alone.

Guardrail:
cleanroom particle-cleanliness requirements are not generalized to all manufactured parts.

### W6H-S02 — ISO 8501-1:2007
Title: Preparation of steel substrates before application of paints and related products — Visual assessment of surface cleanliness — Part 1
Official:
https://www.iso.org/standard/43426.html

Current status:
published/current; replacement DIS active.

Public support:
surface-preparation state can be specified/assessed before coating.

Episode use:
surface preparation is part of the coating system.

Guardrail:
steel-paint preparation grades are not generic cleanliness levels for all materials/processes.

### W6H-S03 — ISO 8501-4:2020
Title: Preparation of steel substrates before application of paints and related products — Part 4: water-jetting conditions/preparation grades
Official:
https://www.iso.org/standard/73861.html

Current status:
confirmed 2026/current.

Use:
another scoped example showing preparation method/state matters.

## 3. Coating / surface-state measurement source family

### W6H-S04 — ISO 2178:2016
Title: Non-magnetic coatings on magnetic substrates — Measurement of coating thickness — Magnetic method
Official:
https://www.iso.org/standard/63004.html

Current status:
confirmed 2026/current.

Public support:
coating thickness is a measurable process/product characteristic for applicable substrate/coating combinations.

### W6H-S05 — ISO 2360:2017
Title: Non-conductive coatings on non-magnetic electrically conductive base metals — Measurement of coating thickness — Eddy-current method
Official:
https://www.iso.org/standard/69943.html

Current status:
confirmed/current.

Public support:
measurement method applicability depends on coating/substrate combination.

### W6H-S06 — ISO 4518:2021
Title: Metallic coatings — Measurement of coating thickness — Profilometric method
Official:
https://www.iso.org/standard/78375.html

Use:
coating thickness may require specific measurement method and geometry/surface conditions.

### W6H-S07 — ASTM E376-26
Title: Measuring Coating Thickness by Magnetic-Field or Eddy Current Testing Methods
Official:
https://store.astm.org/e0376-26.html

Current status:
active, 2026 revision.

Public support:
instrument applicability depends on coating/substrate combination and measurement conditions.

Episode use:
measurement method must match final surface system.

### W6H-S08 — ASTM D1654-24e1
Title: Evaluation of Painted or Coated Specimens Subjected to Corrosive Environments
Official:
https://store.astm.org/d1654-24e01.html

Current status:
active.

Use:
corrosion/coating performance tests are comparative/scoped to system/test conditions.

Guard:
accelerated test outcome is not automatically direct field life.

## 4. Heat-treatment / pyrometry source family

### W6H-S09 — SAE AMS2750H
Title: Pyrometry
Owner: SAE International
Official:
https://saemobilus.sae.org/standards/ams2750h-pyrometry

Current revision:
H, revised 2024-07-15.

Public scope:
pyrometric requirements for thermal-processing equipment used for metallic materials, including sensors, instrumentation, equipment, system accuracy and temperature uniformity.

Episode use:
thermal-processing evidence can require controlled measurement/equipment state.

Guardrail:
AMS2750H is not a universal requirement for every heat-treatment application.

### W6H-S10 — NIST residual-stress / thermal-processing evidence
Examples:
https://www.nist.gov/publications/experimental-investigation-residual-stress-and-its-impact-machining-hybrid
https://www.nist.gov/publications/part-deflection-measurements-am-bench-in718-3d-build-artifacts

Public support:
thermal/process history and residual stress can change dimensional state; later machining/heat treatment can change distortion/microstructure.

Episode use:
sequence and thermal history matter.

## 5. EP18 engineering claims

### W6H-C01 — final product definition can include surface/cleanliness/metallurgical state, not geometry alone
Status: VERIFIED PREMISE + V6 SYNTHESIS.
Sources: W6H-S01–S10.

### W6H-C02 — “clean” is not binary; requirement should identify relevant contamination, location, measurement and preservation point
Status: VERIFIED PREMISE + V6 SYNTHESIS.
Source: W6H-S01 + clean-manufacturing domain.

### W6H-C03 — surface preparation is part of coating/adhesive/process performance where applicable
Status: VERIFIED.
Sources: W6H-S02/S03 + EP14 adhesive sources.

### W6H-C04 — coating thickness can affect functional dimensions/interfaces and requires an applicable measurement method
Status: VERIFIED PREMISE + V6 SYNTHESIS.
Sources: W6H-S04/S05/S06/S07.

### W6H-C05 — masking/racking/contact/coverage strategy is part of the surface-processing route when it changes treated/untreated areas or process access
Status: V6 SYNTHESIS.

### W6H-C06 — accelerated corrosion/coating tests compare behavior under defined exposure and do not automatically equal field life
Status: VERIFIED PREMISE.
Source: W6H-S08 + reliability guardrail.

### W6H-C07 — heat treatment can change material state/properties and dimensions; furnace setpoint recipe alone is not the complete realized thermal history
Status: VERIFIED PREMISE + V6 SYNTHESIS.
Sources: W6H-S09/S10 + heat-treatment domain.

### W6H-C08 — furnace/load/fixture/instrumentation state can matter to heat-treatment evidence where the governing process/specification requires it
Status: VERIFIED PREMISE + V6 SYNTHESIS.
Source: W6H-S09.

### W6H-C09 — cleaning/surface treatment/heat-treatment sequence can enable or invalidate downstream joining, coating, sealing, machining or measurement evidence
Status: V6 SYNTHESIS + EP14/EP19 dependency.

### W6H-C10 — stripping/rework/recoat/reheat can create a new material/surface/configuration state requiring impact review
Status: GLOBAL INVARIANT + V6 SYNTHESIS.

### W6H-C11 — inspection before a later state-changing process may not prove final-product geometry/surface/property
Status: VERIFIED PREMISE + V6 SYNTHESIS.
Sources: coating thickness / residual-stress / process-state sources.

### W6H-C12 — exact cleanliness limit, coating thickness, surface preparation, furnace class/uniformity, time-temperature cycle and property acceptance are application/material/process specific
Status: APPLICABILITY GUARDRAIL.

## 6. Hard guardrails

1. no universal cleanliness level;
2. no universal cleaning chemistry/time/temperature;
3. no steel-paint preparation grade generalized to other substrates/processes;
4. no universal coating thickness;
5. no universal corrosion-test-hours → service-life conversion;
6. no universal masking/racking rule;
7. no AMS2750H requirement generalized to every heat-treatment process;
8. no furnace class/TUS/SAT interval/tolerance from memory;
9. no universal heat-treatment recipe/hardness/property value;
10. no assumption hardness alone proves required metallurgical state;
11. no stripping/recoat/reheat assumed harmless;
12. no dimensional inspection before a state-changing process treated as final evidence without analysis.

## 7. Current-status lock

Checked 2026-09-19:
- ISO 14644-9:2022 current.
- ISO 8501-1:2007 current; revision project active.
- ISO 8501-4:2020 current/confirmed 2026.
- ISO 2178:2016 current/confirmed 2026.
- ISO 2360:2017 current.
- ISO 4518:2021 current.
- ASTM E376-26 active/current.
- ASTM D1654-24e1 active.
- SAE AMS2750H current revision, July 2024.

## 8. Episode gate

EP18 can proceed without application-specific cleaning limits, coating systems or heat-treatment recipes.

Current generic-script P0 blockers: 0.
