# Source-Lock Wave 06C — Metals / Machining / Casting / Forming Shared Source Register

status: SHARED SOURCE REGISTER LOCKED
checked: 2026-09-19
scope: EP13 — Metal Parts: Casting, Forming or Machining?
dependencies: Wave 06A process selection + Wave 03 economics + Wave 02 quality

## 1. Purpose

Lock the generic engineering premises required to compare machining, casting, forging/forming, extrusion/sheet and near-net + finish-machining routes without universalizing alloy-, geometry-, supplier- or process-specific numbers.

## 2. Authoritative / primary source register

### W6C-S01 — NIST Solidification (2026)
Owner: NIST
Published: 2026-05-15
Source:
https://www.nist.gov/publications/solidification-0

Support:
- metal casting is a major manufacturing application of solidification;
- solidification involves heat/transport, alloy thermodynamics, nucleation/growth, segregation, porosity, inclusions and fluid flow;
- final cast state depends on solidification physics, not geometry alone.

Episode use:
casting route physics / porosity / segregation context.

### W6C-S02 — American Foundry Society casting-defect analysis
Owner: AFS
Source:
https://www.afsinc.org/e-learning/casting-defect-analysis

Support:
gas porosity and shrinkage porosity are distinct casting-defect families with process-specific causes/control approaches.

Episode use:
casting defect mechanism context.

Guardrail:
no universal porosity acceptance level is inferred.

### W6C-S03 — Forging Industry Association Product Design Guide
Owner: Forging Industry Association
Source:
https://www.forging.org/Common/Uploaded%20files/Design%20Engineering%20Center/Product%20Design%20Guide%20for%20Forging.pdf

Support:
- forging process and developed grain flow can significantly affect material properties;
- material, forging process and heat treatment should be balanced together;
- forging design includes parting line, draft, machining allowance and inspection considerations.

Episode use:
forging route / grain-flow / material-state coupling.

Guardrail:
numeric forging design values remain guide/process/material specific.

### W6C-S04 — NIST Springback program
Owner: NIST
Source:
https://www.nist.gov/programs-projects/springback
Updated: 2025-03-26.

Support:
springback is elastic shape change after forming; prediction depends on material properties and complex strain history.

Episode use:
sheet/forming route dimensional behavior.

### W6C-S05 — NIST NCAL tension-compression / sheet forming
Owner: NIST
Source:
https://www.nist.gov/programs-projects/ncal-tension-compression-testing

Support:
sheet forming behavior and springback depend on material constitutive response/loading path; advanced alloys may not follow simple legacy rules.

Episode use:
material-state/process-history coupling in forming.

### W6C-S06 — ISO 230-2:2014 + Amd1:2016
Owner: ISO
Title: Test code for machine tools — Part 2: positioning accuracy/repeatability of NC axes
Current status checked:
2014 Edition 4 confirmed 2025; Amendment 1:2016 applies.
Official:
https://www.iso.org/standard/55295.html

Use:
machine-axis positioning capability context.

Boundary:
axis accuracy is not finished-part accuracy.

### W6C-S07 — ISO 230-12:2022
Owner: ISO
Title: Test code for machine tools — Part 12: Accuracy of finished test pieces
Edition: 1
Official:
https://www.iso.org/standard/76756.html

Public support:
finished test-piece geometric error can have multiple contributors; machine quasi-static errors are important but other effects such as dynamic contouring can also matter.

Episode use:
machine capability ≠ part/process capability.

### W6C-S08 — NIST residual stress / machining distortion
Owner: NIST
Source:
https://www.nist.gov/publications/experimental-investigation-residual-stress-and-its-impact-machining-hybrid

Support:
residual stresses in a manufactured metal state can cause unanticipated distortion during subsequent machining.

Episode use:
general mechanism example for process sequence/material-state effects.

Boundary:
study is hybrid AM/subtractive and is not generalized quantitatively to all wrought/cast parts.

### W6C-S09 — NIST springback / formed-part research
Additional sources:
https://www.nist.gov/publications/robustness-sheet-metal-springback-cup-test
https://www.nist.gov/publications/designing-uniaxial-tensioncompression-test-springback-analysis-high-strength-steel-0

Use:
formed-part springback and residual-stress/material response are real dimensional-control problems.

### W6C-S10 — NIST process/material-selection package
Dependency:
Wave 06A NIST source family.

Use:
route selection remains material/process/economics coupled.

## 3. EP13 engineering claims

### W6C-C01 — machining is one metal route, not the default production truth
Status: VERIFIED + V6 SYNTHESIS.
Support: Wave 06A + W6C source family.

### W6C-C02 — cast-part behavior depends on solidification, flow, segregation and defect mechanisms as well as geometry
Status: VERIFIED.
Sources: W6C-S01/S02.

### W6C-C03 — porosity is not one defect mechanism and its consequence depends on location/size/connectivity/function
Status: VERIFIED + V6 SYNTHESIS.
Sources: W6C-S01/S02.

### W6C-C04 — forging/forming can create directional material structure/grain-flow effects that matter to part behavior
Status: VERIFIED INDUSTRY GUIDANCE.
Source: W6C-S03.

### W6C-C05 — sheet-metal forming can exhibit springback tied to material response and strain history
Status: VERIFIED.
Sources: W6C-S04/S05/S09.

### W6C-C06 — machine-axis accuracy/repeatability is not equivalent to finished-part process capability
Status: VERIFIED PUBLIC SCOPE.
Sources: W6C-S06/S07.

### W6C-C07 — residual stress/material history can cause distortion during later machining
Status: VERIFIED MECHANISM.
Source: W6C-S08 + heat-treatment domain synthesis.

### W6C-C08 — exact alloy/temper/heat-treatment/incoming state belongs to the route definition
Status: VERIFIED PREMISE + V6 SYNTHESIS.
Sources: W6C-S03/S05 + heat-treatment domain.

### W6C-C09 — near-net + finish machining can be a valid route when precision is concentrated at functional interfaces
Status: V6 SYNTHESIS supported by W6C-S01/S03/S07 + Wave 06A.

### W6C-C10 — inspection/NDT burden belongs in route selection where casting/forming/material-state risks require it
Status: V6 SYNTHESIS.
No universal NDT method/acceptance level asserted.

### W6C-C11 — process sequence can invalidate earlier dimensional evidence
Status: DEPENDENCY — Wave 01 + heat-treatment/residual-stress mechanisms.

### W6C-C12 — supplier/source capability must be demonstrated for the actual alloy/state/geometry/process/inspection envelope
Status: DEPENDENCY — Waves 02/03.

## 4. Hard guardrails

1. no universal casting porosity acceptance level;
2. no universal forging grain-flow strength multiplier;
3. no universal machining allowance;
4. no generic bend radius/springback compensation;
5. no “same alloy name = same state” assumption;
6. no machine positioning spec used as finished-part tolerance proof;
7. no heat-treatment recipe or hardness value without exact alloy/application;
8. no claim casting/forging automatically beats machining at a fixed volume;
9. no universal NDT method/acceptance rule;
10. process-specific standards/allowables remain application scoped.

## 5. Current-status lock

- ISO 230-2:2014 Edition 4 + Amd1:2016 — current/confirmed.
- ISO 230-12:2022 Edition 1 — current.
- NIST Springback project active/current.
- NIST Solidification source updated/published 2026.

## 6. Episode gate

EP13 can proceed using current generic material/process evidence without process-family numeric thresholds.

Current generic-script P0 blockers: 0.
