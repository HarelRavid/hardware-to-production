# Source-Lock Wave 06E — Composite Manufacturing Shared Source Register

status: SHARED SOURCE REGISTER LOCKED
checked: 2026-09-19
scope: EP15 — Composite Manufacturing
dependencies: Wave 06A process selection + Wave 06D joining + Wave 02 measurement/quality + Wave 01 configuration

## 1. Purpose

Lock the authoritative/public premises required to teach composite manufacturing as a coupled material-architecture/process system without importing aerospace allowables, material-specific cure cycles or generic defect limits into a cross-industry episode.

EP15 teaches:
reinforcement + matrix + architecture + process + cure/consolidation + defects + inspection + evidence transfer.

## 2. CMH-17 source family

### W6E-S01 — Composite Materials Handbook-17 overview/current release
Owner: CMH-17
Official:
https://www.cmh17.org/HOME/About-CMH-17
https://www.cmh17.org/HOME/FAQ

Current public status checked 2026-09-19:
- Polymer Matrix Composite Volumes 1–3: current Release H family.
- Vol. 1 Rev H: Guidelines for Characterization of Structural Materials.
- Vol. 2 Rev H: Polymer Matrix Composite Material Properties.
- Vol. 3 Rev H: Materials Usage, Design and Analysis.

Public support:
CMH-17 is an authoritative composite-materials handbook framework linking material characterization, process/raw-material control, design, fabrication, testing and maintenance.

Episode use:
generic composite evidence architecture.

Guardrail:
CMH-17 aerospace/structural-composite rigor is not imposed as a universal commercial product requirement.

### W6E-S02 — CMH-17 Volume 3 Rev H public change summary
Official public summary:
https://www.cmh17.org/Portals/0/Summary%20of%20Changes%20%281%29.pdf

Public support:
Volume 3 includes topics on:
- constituent materials;
- product-form processing;
- shipping/storage;
- construction;
- cure/consolidation;
- bonded assembly;
- process control;
- manufacturing process simulation/control;
- production-material/process quality control;
- managing changes in materials and processes.

Episode use:
process/material-state/control/change coupling.

### W6E-S03 — CMH-17 roadmaps / qualification & equivalency
Official:
https://www.cmh17.org/HOME/FAQ

Public support:
CMH-17 explicitly distinguishes:
- qualification of new material;
- development/use of material data;
- equivalency for revised material/process;
- equivalency for second-source material;
- bolted/bonded joint testing;
- repair design/analysis/fabrication.

Episode use:
change/equivalency and coupon-to-application evidence boundaries.

Guardrail:
exact CMH-17 procedures remain controlled handbook content and aerospace-oriented context.

## 3. Composite test-method source family

### W6E-S04 — ASTM D3039/D3039M-17(2025)
Owner: ASTM International
Title: Standard Test Method for Tensile Properties of Polymer Matrix Composite Materials
Official:
https://store.astm.org/d3039_d3039m-17r25.html

Current status:
Active, reapproved 2025.

Public support:
tensile response may depend on:
- material;
- material preparation/lay-up;
- stacking sequence;
- specimen preparation;
- conditioning;
- test environment;
- void content;
- reinforcement volume;
- test setup variables.

Episode use:
coupon result is configuration/process dependent.

### W6E-S05 — ISO 527-5:2021
Owner: ISO
Title: Plastics — Determination of tensile properties — Part 5: Test conditions for unidirectional fibre-reinforced plastic composites
Official:
https://www.iso.org/standard/80370.html

Current status:
Edition 3, published/current.

Public support:
tensile properties are test-condition/specimen/material-orientation specific.

### W6E-S06 — ISO 14125:1998 + Amd1:2011
Owner: ISO
Title: Fibre-reinforced plastic composites — Determination of flexural properties
Official:
https://www.iso.org/standard/23637.html

Current status:
- Edition 1 remains current;
- confirmed 2024;
- Amendment 1:2011 applies.

Episode use:
another example that composite property evidence is test-configuration specific.

## 4. FAA composite-structure guidance as scoped corroboration

### W6E-S07 — FAA AC 20-107B — Composite Aircraft Structure
Owner: U.S. FAA
Official:
https://www.faa.gov/airports/resources/advisory_circulars/index.cfm/go/document.information/documentNumber/20-107B

Current status:
Active.

Public scope:
acceptable means of compliance/guidance for composite aircraft structures; includes design, manufacturing and maintenance considerations.

Episode use:
corroborates that composite design/manufacturing/maintenance evidence are tightly linked.

Guardrail:
aviation certification requirements are NOT generalized to non-aircraft hardware.

## 5. EP15 engineering claims

### W6E-C01 — “carbon fiber” / “composite” is not a complete material definition
Status: VERIFIED PREMISE + V6 SYNTHESIS.
Support: W6E-S01/S02/S04.

### W6E-C02 — composite properties depend on reinforcement/matrix/architecture/process state together
Status: VERIFIED.
Sources: W6E-S01/S02/S04/S05.

### W6E-C03 — ply/fiber orientation and stacking sequence are part of the structural/material definition, not merely manufacturing detail
Status: VERIFIED PREMISE.
Source: W6E-S04/S05 + CMH-17 context.

### W6E-C04 — storage/handling/cure/consolidation history can be part of the material/process evidence
Status: VERIFIED PUBLIC-SCOPE PREMISE.
Sources: W6E-S02/S03.

### W6E-C05 — voids, wrinkles, delamination, dry/resin-rich regions, fiber misorientation and contamination are process-created defect families whose consequence/detectability are application dependent
Status: V6 SYNTHESIS supported by CMH-17/FAA/domain evidence.
No universal defect limit.

### W6E-C06 — coupon property evidence does not automatically equal part/structure performance
Status: VERIFIED + V6 SYNTHESIS.
Sources: W6E-S04/S05/S06/S03.

### W6E-C07 — coupon-to-part transfer depends on representative material architecture, geometry/process state, conditioning/environment, loading and inspection/evidence
Status: VERIFIED PREMISE + V6 SYNTHESIS.
Sources: W6E-S03/S04/S07.

### W6E-C08 — tooling/cure/process sequence can create dimensional state and variation that must be part of production evidence
Status: VERIFIED PREMISE + V6 SYNTHESIS.
Source: W6E-S02 + composite domain.

### W6E-C09 — trim/drill/inserts/bonded joints are not automatically minor secondary operations; they can change damage/load-transfer/inspection requirements
Status: V6 SYNTHESIS + EP14 dependency.

### W6E-C10 — NDT/inspection selection is defect-, material-, geometry- and criticality-dependent
Status: VERIFIED PREMISE + V6 SYNTHESIS.
Source: CMH-17/FAA/domain evidence.
No universal NDT method or POD threshold.

### W6E-C11 — material/process/supplier changes may require equivalency/reassessment when they affect demonstrated evidence
Status: VERIFIED PREMISE + Wave01 invariant.
Source: W6E-S03.

### W6E-C12 — manual prototype layup success does not establish controlled serial-process capability
Status: DEPENDENCY — A4/Wave02/Wave03.

## 6. Process-family map for EP15

High-level comparison only:
- hand/wet layup;
- vacuum-bag/infusion;
- prepreg/autoclave/OOA;
- RTM/closed-mold;
- compression molding/SMC/BMC;
- filament winding/pultrusion;
- ATL/AFP where relevant.

No process family is ranked universally by maturity.

## 7. Hard guardrails

1. no universal fiber volume, void, porosity or defect acceptance limit;
2. no universal prepreg storage/out-time/cure recipe;
3. no universal autoclave pressure/temperature;
4. no coupon property used as arbitrary part allowable;
5. no aerospace certification requirement generalized;
6. no claim carbon fiber is one material;
7. no claim autoclave = highest maturity;
8. no universal NDT method/detection threshold;
9. no supplier/material substitution assumed equivalent by trade name;
10. no laminate-property value without exact material/architecture/test context;
11. no composite repair/allowable rule without applicable source;
12. dense layup/defect spatial detail should move to companion visual rather than overloading audio.

## 8. Current-status lock

Checked 2026-09-19:
- CMH-17 PMC current public release family: H.
- ASTM D3039/D3039M-17(2025): active.
- ISO 527-5:2021: current.
- ISO 14125:1998 + Amd1:2011: current/confirmed.
- FAA AC 20-107B: active guidance; aviation scope only.

## 9. Episode gate

EP15 can proceed to claim lock/technical review without material-specific cure windows, allowables or aerospace acceptance criteria.

Current generic-script P0 blockers: 0.
