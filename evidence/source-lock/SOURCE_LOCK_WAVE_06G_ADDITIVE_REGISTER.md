# Source-Lock Wave 06G — Additive Manufacturing Shared Source Register

status: SHARED SOURCE REGISTER LOCKED
checked: 2026-09-25
scope: EP17 — Additive Manufacturing: When It Creates Value and When It Does Not
dependencies: Wave 06A process selection + Wave 02 measurement/quality + Wave 03 economics + Wave 01 configuration/change

## 1. Purpose

Lock the generic evidence required to teach additive manufacturing as a production-route decision rather than a technology showcase.

EP17 must answer:
- when AM creates unique product/business value;
- what process-state/evidence burden comes with it;
- when a conventional or hybrid route is better.

No universal AM property, parameter window, break-even volume or qualification rule is taught.

## 2. Core AM terminology / industrialization source family

### W6G-S01 — ISO/ASTM 52900:2021
Title: Additive manufacturing — General principles — Fundamentals and vocabulary
Official:
https://www.iso.org/standard/74514.html

Current status:
Edition 2; confirmed 2025; current.

Public support:
AM is a family of additive shaping technologies with standardized terminology/process categories.

Use:
process-family vocabulary only.

### W6G-S02 — ISO/ASTM 52920:2023
Title: Additive manufacturing — Qualification principles — Requirements for industrial additive manufacturing processes and production sites
Official:
https://www.iso.org/standard/76911.html

Current status:
Edition 1; current.

Public support:
industrial AM production includes quality-relevant processes, characteristics and production-site activities independent of one material/process family.

Use:
AM production readiness is broader than “the printer can make the shape.”

Guardrail:
not asserted as mandatory for every AM application.

### W6G-S03 — ISO/ASTM TS 52930:2021
Title: Additive manufacturing — Qualification principles — IQ/OQ/PQ of PBF-LB equipment
Official:
https://www.iso.org/standard/79527.html

Current status:
Edition 1; current Technical Specification.

Public support:
equipment installation, operation and performance qualification are distinct machine/system evidence layers.

Use:
machine qualification example.

Guardrail:
PBF-LB-specific; not generalized to every AM family.

## 3. NIST AM qualification / measurement source family

### W6G-S04 — NIST Additive Manufacturing Part Qualification
Official:
https://www.nist.gov/programs-projects/additive-manufacturing-part-qualification

Public support:
AM qualification is challenged by:
- complex/internal geometries;
- surface topography;
- internal defects;
- anisotropic properties;
- residual stresses;
- post-process effects;
- dimensional/NDE measurement difficulty.

Use:
production qualification and inspection burden.

### W6G-S05 — NIST Qualification for AM Materials, Processes and Parts
Official:
https://www.nist.gov/programs-projects/qualification-additive-manufacturing-materials-processes-and-parts

Public support:
qualification may be statistical/equivalence/model based depending on context; process variables materially affect qualification burden.

Use:
qualification is application/process dependent.

Guardrail:
critical aerospace/defense/medical examples remain scoped examples.

### W6G-S06 — NIST Measurement Science for Additive Manufacturing
Official:
https://www.nist.gov/programs-projects/measurement-science-additive-manufacturing-program

Public support:
AM process control, post-process metrology, NDE and data-management/qualification are active production concerns.

### W6G-S07 — NIST Additive Manufacturing Standards
Official:
https://www.nist.gov/additive-manufacturing/standards

Updated: 2026-08-06.

Public support:
AM industrialization depends on evolving standards and benchmarks across materials/processes/test/quality.

## 4. Current ISO/ASTM catalogue context

### W6G-S08 — ISO TC261 current AM catalogue
Official:
https://www.iso.org/committee/629086/x/catalogue/

Current public examples:
- ISO/ASTM 52919:2025
- ISO/ASTM 52927:2024
- ISO/ASTM 52928:2024
- ISO/ASTM 52929:2025
- ISO/ASTM 52920:2023
- ISO/ASTM 52924:2023
- ISO/ASTM 52925:2022
- ISO/ASTM 52926 series: 2023

Use:
demonstrates that AM qualification/material/operator standards are process/application specific rather than one generic AM rulebook.

Guardrail:
EP17 does not teach these standards’ protected details.

### W6G-S08A — ISO/ASTM 52927:2024
Title: Additive manufacturing — General principles — Main characteristics and corresponding test methods
Status: current/published.
Use: AM characteristics/test methods are process/evidence specific.

### W6G-S08B — ISO/ASTM 52928:2024
Title: Additive manufacturing of metals — Feedstock materials — Powder life cycle management
Status: current/published.
Use: feedstock state/reuse/history are controlled production-evidence objects.

### W6G-S08C — ISO/ASTM 52929:2025
Title: Additive manufacturing of metals — Powder bed fusion — Presentation of material properties in material data sheets
Status: current/published.
Use: material-property statements remain process/material context dependent.

## 5. Economics source family

### W6G-S09 — NIST AM cost effectiveness
Dependency:
Wave 06A / NIST SP 1176 and supply-chain AM economics.

Use:
AM economics depend on utilization, tooling avoidance, complexity, post-processing, inspection and system boundary.

## 6. EP17 engineering claims

### W6G-C01 — “printable” does not equal production viable, inspectable, qualified or economical
Status: VERIFIED PREMISE + V6 SYNTHESIS.
Sources: W6G-S02/S04/S06.

### W6G-C02 — AM can create unique value through complexity, internal features, consolidation, customization, low tooling or iteration speed, but those benefits are application dependent
Status: VERIFIED PREMISE + V6 SYNTHESIS.
Sources: W6G-S04/S09.

### W6G-C03 — build orientation/support/toolpath/build strategy can change geometry, surface, material state, post-processing and evidence
Status: VERIFIED PREMISE + V6 SYNTHESIS.
Sources: W6G-S04/S06.

### W6G-C04 — anisotropy, residual stress, porosity/internal defects and surface condition can affect AM part qualification
Status: VERIFIED.
Source: W6G-S04.

### W6G-C05 — post-processing can materially change final AM part state and must remain inside the process/evidence chain
Status: VERIFIED.
Sources: W6G-S04/S06.

### W6G-C06 — complex/internal geometry can create metrology/NDE/cleaning/access burdens that must be considered during process selection
Status: VERIFIED.
Sources: W6G-S04/S06.

### W6G-C07 — AM machine qualification, process qualification and part/application qualification are distinct questions
Status: VERIFIED PREMISE + V6 SYNTHESIS.
Sources: W6G-S02/S03/S05.

### W6G-C08 — prototype print success does not establish production process/material/part qualification
Status: VERIFIED PREMISE.
Sources: W6G-S02/S04/S05.

### W6G-C09 — feedstock lot/state, machine/build configuration, orientation, supports, post-process and inspection should remain traceably linked where they affect the product claim
Status: V6 SYNTHESIS + Wave01/Wave05.

### W6G-C10 — AM should be compared against conventional/hybrid alternatives using final accepted-part economics and evidence burden
Status: DEPENDENCY — Wave06A/Wave03.

### W6G-C11 — no universal AM break-even volume exists
Status: VERIFIED ECONOMIC GUARDRAIL + V6 SYNTHESIS.
Source: W6G-S09.

### W6G-C12 — in-process monitoring does not automatically replace post-process verification/qualification unless the relationship to product quality is validated
Status: VERIFIED PREMISE + V6 SYNTHESIS.
Sources: W6G-S04/S06.

## 7. Hard guardrails

1. no AM hype / no “complexity is free”;
2. no universal AM break-even volume;
3. no universal anisotropy/porosity/surface/tolerance value;
4. no machine/material label = qualified state shortcut;
5. no in-process monitoring = acceptance shortcut;
6. no inspection method treated as universal for internal AM defects;
7. no feedstock reuse rule without exact process/material source;
8. no heat-treatment/HIP recipe generalized;
9. no PBF-LB qualification rule generalized to other AM processes;
10. no medical/aerospace/defense qualification burden generalized;
11. no printer time compared directly with accepted final part cost;
12. no prototype-print evidence silently upgraded to serial-production evidence.

## 8. Current-status lock

Checked 2026-09-19:
- ISO/ASTM 52900:2021 current/confirmed 2025.
- ISO/ASTM 52920:2023 current.
- ISO/ASTM TS 52930:2021 current.
- ISO/TC 261 catalogue includes newer process/material/operator qualification standards through 2025.
- NIST AM Standards page updated 2026-08-06.

## 9. Episode gate

EP17 can proceed to claim lock/technical review without material/process-specific property allowables or qualification criteria.

Current generic-script P0 blockers: 0.
