# Source-Lock Wave 06F — Ceramics / Powder Processing / Sintering Shared Source Register

status: SHARED SOURCE REGISTER LOCKED
checked: 2026-09-19
scope: EP16 — Ceramics, Powder Processing and Sintering
dependencies: Wave 06A process selection + Wave 02 measurement/quality + Wave 03 change/economics + Wave 01 configuration

## 1. Purpose

Lock the authoritative/public premises required to teach powder-to-part processing as a coupled state transformation:

powder/feedstock
→ forming
→ green body
→ debinding/drying where applicable
→ sintering
→ density/microstructure
→ final geometry/properties.

EP16 does not teach one material-specific sintering recipe, shrink factor, furnace atmosphere or density threshold.

## 2. Ceramic powder / green-body source family

### W6F-S01 — NIST TWA 27 — Characterisation Methods for Ceramic Powders and Green Bodies
Official:
https://www.nist.gov/publications/twa-27-characterisation-methods-ceramic-powders-and-green-bodies

Public support:
ceramic manufacturing benefits from explicit characterization of:
- powder properties;
- suspensions;
- green bodies.

Episode use:
powder and green-body states are real engineering/evidence objects, not disposable intermediates.

### W6F-S02 — NIST Assessment of Powder Characterization Methods for Advanced Ceramics
Official:
https://www.nist.gov/publications/assessment-powder-characterization-methods-advanced-ceramics

Public support:
characterization can include:
- particle dispersion;
- spray-dried powder flow;
- particle-size distribution;
- moisture/binder content;
- green-body bulk density and strength.

Episode use:
powder/feedstock/green-body variability can matter before sintering.

### W6F-S03 — NIST Green Body Density Measurement Techniques
Official:
https://www.nist.gov/publications/green-body-density-measurement-techniques

Public support:
green-body density is measurable and relevant to ceramic manufacturing/process control; multiple measurement methods exist.

Episode use:
green density is an intermediate process-state metric, not just a lab curiosity.

## 3. Ceramic sintering / density source family

### W6F-S04 — ISO 21821:2019
Title: Fine ceramics — Determination of densification properties of ceramic powders on natural sintering
Official:
https://www.iso.org/standard/71877.html

Current status:
Edition 1; confirmed 2025; current.

Public support:
test method characterizes how ceramic powder compacts densify during pressureless/natural sintering under a stated thermal/gas condition.

Episode use:
sintering changes density/state; densification is material/process dependent.

Guardrail:
the standard does not provide a universal production sintering recipe.

### W6F-S05 — ISO 18754:2020
Title: Fine ceramics — Determination of density and apparent porosity
Official:
https://www.iso.org/standard/69745.html

Current status:
Edition 3; published/current; under review.

Public support:
bulk density/apparent porosity require defined measurement methods and method applicability has limits.

Episode use:
final density/porosity evidence is measurement-method/context dependent.

### W6F-S06 — ISO 18753:2017
Title: Fine ceramics — Determination of absolute density of ceramic powders by pycnometer
Official:
https://www.iso.org/standard/65414.html

Current status:
Edition 2; confirmed 2022; current.

Public support:
powder absolute density is a distinct measurable property.

Episode use:
powder identity/state and final-part density are not the same measurement object.

## 4. Powder metallurgy source family

### W6F-S07 — ASTM B962-23
Title: Standard Test Methods for Density of Compacted or Sintered Powder Metallurgy Products Using Archimedes’ Principle
Official:
https://store.astm.org/b0962-23.html

Current status:
Active.

Public support:
- green density is used during press setup/quality control;
- sintered density is used as a quality-control measure;
- method applicability depends on product porosity state.

Episode use:
green and sintered density are distinct process/evidence states.

### W6F-S08 — ISO 2738:2026
Title: Sintered metal materials, excluding hardmetals — Permeable sintered metal materials — Determination of density, oil content and open porosity
Official:
https://www.iso.org/standard/85913.html

Current status:
Edition 4; published 2026-01; replaced ISO 2738:1999.

Public support:
density/open-porosity characterization for porous sintered metal products.

Episode use:
final porosity/density characterization is product/method scoped.

## 5. NIST process-history examples

### W6F-S09 — NIST low-temperature compaction of nanosize powders
Official:
https://www.nist.gov/publications/low-temperature-compaction-nanosize-powders

Support:
green-body density/compaction state can affect later sintering behavior.

Episode use:
mechanism-level corroboration only.

### W6F-S10 — NIST ceramic database / processing records
NIST Structural Ceramics Database:
https://srdata.nist.gov/CeramicDataPortal/Scd/

Public support:
documented examples show powder preparation, binder/green-body formation, debinding/thermal processing, sintering atmosphere/time/temperature and final density/microstructure as linked process history.

Episode use:
process-history concept only.

Guardrail:
individual material recipes are NOT generalized.

## 6. EP16 engineering claims

### W6F-C01 — powder/feedstock state matters to downstream processing
Status: VERIFIED.
Sources: W6F-S01/S02/S06.

### W6F-C02 — green-body density/strength/uniformity are meaningful intermediate process states
Status: VERIFIED.
Sources: W6F-S01/S02/S03/S07.

### W6F-C03 — binder/debinding/drying stages can be failure-prone state transformations rather than incidental preparation
Status: VERIFIED PREMISE + V6 SYNTHESIS.
Support: NIST processing examples + domain evidence.

### W6F-C04 — sintering changes density/microstructure and typically dimensions; densification is material/process dependent
Status: VERIFIED.
Sources: W6F-S04/S05/S07/S08.

### W6F-C05 — one global shrink factor should not be assumed universally valid across geometry/orientation/green state/furnace condition
Status: VERIFIED PREMISE + V6 SYNTHESIS.
Sources: W6F-S04 + green-body/process-state evidence.

### W6F-C06 — final geometry can depend on green density, support/fixture, furnace load/position, atmosphere and thermal history where relevant
Status: VERIFIED PREMISE + V6 SYNTHESIS.
Sources: W6F-S04/S09/S10 + domain evidence.

### W6F-C07 — final density/porosity is not a universal proxy for every mechanical/functional property
Status: V6 SYNTHESIS.
Support: W6F-S05/S07/S08 measurement scopes.

### W6F-C08 — density/porosity measurements have method/applicability limits and should not be interpreted outside the test context
Status: VERIFIED.
Sources: W6F-S05/S07/S08.

### W6F-C09 — powder/material lot, forming state, debind/sinter history and final evidence should remain linked when they affect the product claim
Status: DEPENDENCY — Wave01/05 genealogy + W6F source family.

### W6F-C10 — dimensional compensation should be evidence based and may require feature/orientation/location-specific data rather than one scalar
Status: V6 SYNTHESIS.

### W6F-C11 — furnace recipe text alone is not complete thermal/process evidence if actual part/load/atmosphere/fixture state changes the result
Status: V6 SYNTHESIS + domain evidence.

### W6F-C12 — prototype or small-furnace success does not automatically establish loaded-furnace/serial capability
Status: DEPENDENCY — A4/Wave03.

## 7. Hard guardrails

1. no universal sintering temperature/time/atmosphere;
2. no universal debinding ramp/hold;
3. no universal shrinkage factor;
4. no universal green-density target;
5. no universal final density/porosity acceptance;
6. no claim density alone proves strength/reliability;
7. no assumption one furnace recipe reproduces same part state at different load/fixture/zone conditions;
8. no material-specific ceramic/PM recipe generalized;
9. no pressure-assisted sintering claims generalized from ISO 21821, which explicitly covers natural/pressureless sintering scope;
10. no method-specific density result interpreted outside method applicability;
11. no universal furnace/pyrometry requirement unless exact application/standard is source locked;
12. any dimensional compensation model must remain empirical/application specific.

## 8. Current-status lock

Checked 2026-09-19:
- ISO 21821:2019 current/confirmed 2025.
- ISO 18754:2020 current/published, under review.
- ISO 18753:2017 current/confirmed.
- ASTM B962-23 active.
- ISO 2738:2026 current, replacing 1999.

## 9. Episode gate

EP16 can proceed to claim lock/technical review without material-specific furnace recipes or acceptance thresholds.

Current generic-script P0 blockers: 0.
