# Source-Lock Wave 06G — Additive Manufacturing Shared Source Register

status: SHARED SOURCE REGISTER LOCKED
checked: 2026-09-19
scope: EP17 — Additive Manufacturing: When It Creates Value and When It Does Not
dependencies: Wave 06A process selection + Wave 02 measurement/quality + Wave 03 economics + Wave 01 configuration/change

## 1. Purpose

Lock the current public/authoritative source layer required to teach AM as a production process family with distinct value cases, process-state dependencies, post-processing and qualification burdens.

EP17 is not a catalogue of AM technologies and not an advocacy episode.

## 2. Current AM standards family

### W6G-S01 — ISO/ASTM 52900:2021
Title: Additive manufacturing — General principles — Fundamentals and vocabulary
Edition: 2
Official:
https://www.iso.org/standard/74514.html

Current status:
reviewed/confirmed 2025; remains current.

Public support:
AM builds physical 3D geometry by successive addition of material and defines common process-family terminology.

### W6G-S02 — ISO/ASTM 52920:2023
Title: Additive manufacturing — Qualification principles — Requirements for industrial additive manufacturing processes and production sites
Edition: 1
Official:
https://www.iso.org/standard/76911.html

Public support:
industrial AM production involves quality-relevant process characteristics/factors across additive-system operations and production-site activities.

Use:
production-AM evidence is broader than successful printing.

### W6G-S03 — ISO/ASTM TS 52930:2021
Title: Additive manufacturing — Qualification principles — IQ/OQ/PQ of PBF-LB equipment
Edition: 1
Official:
https://www.iso.org/standard/79527.html

Current status:
published, under review.

Public support:
PBF-LB machine qualification can involve installation, operation and performance qualification; feedstock and most post-processing remain separate scope.

Use:
machine qualification is not the entire production process qualification.

### W6G-S04 — ISO/ASTM 52924:2023
Title: Additive manufacturing of polymers — Qualification principles — Classification of part properties
Official:
https://www.iso.org/standard/76909.html

Public support:
polymer AM part quality/property expectations can be specified/classified in a traceable way.

Use:
process/material/application-specific property evidence.

### W6G-S05 — ISO/ASTM 52927:2024
Title: Additive manufacturing — General principles — Main characteristics and corresponding test methods
Current published family context:
https://www.iso.org/ics/25.030/x/

Use:
AM quality/property evidence is linked to defined characteristics/test methods.

### W6G-S06 — ISO/ASTM 52928:2024
Title: Additive manufacturing of metals — Feedstock materials — Powder life cycle management
Current published family context:
https://www.iso.org/ics/25.030/x/

Use:
metal-AM powder/feedstock state has lifecycle/traceability implications.

### W6G-S07 — ISO/ASTM 52929:2025
Title: Additive manufacturing of metals — Powder bed fusion — Presentation of material properties in material data sheets
Current published family context:
https://www.iso.org/ics/25.030/x/

Use:
material-property communication remains AM-process/context specific.

### W6G-S08 — ISO/ASTM 52926-1:2023
Title: Additive manufacturing of metals — Qualification principles — General qualification of operators
Official:
https://www.iso.org/standard/76827.html

Public support:
operator qualification can be relevant in industrial metal AM; industry-specific requirements may supersede generic guidance.

Use:
personnel/process qualification is a separate evidence layer.

## 3. NIST source family

### W6G-S09 — NIST Additive Manufacturing program/research family
Primary context:
NIST AM research/measurement-science work.

Use:
process monitoring, measurement, qualification and reproducibility remain active AM engineering challenges rather than solved by geometry alone.

### W6G-S10 — NIST Additive Manufacturing Cost Effectiveness
Source:
https://www.nist.gov/publications/costs-and-cost-effectiveness-additive-manufacturing

Use:
AM economics depend on utilization, material, process and system boundaries; AM is not universally lower cost.

### W6G-S11 — NIST AM supply-chain perspective
Source:
https://www.nist.gov/publications/costs-benefits-and-adoption-additive-manufacturing-supply-chain-perspective

Use:
part-level process cost can omit tooling, inventory, transport, consolidation and wider supply-chain effects.

## 4. EP17 engineering claims

### W6G-C01 — printable geometry is not the same as production viability
Status: VERIFIED PREMISE + V6 SYNTHESIS.
Sources: W6G-S02/S03 + Wave06A.

### W6G-C02 — AM creates value when process-specific benefits such as internal geometry, part consolidation, customization, low tooling or rapid iteration outweigh post-process/qualification/cost burdens
Status: V6 SYNTHESIS + W6G-S10/S11.

### W6G-C03 — orientation/support strategy can affect buildability, process state, geometry, surface and downstream work
Status: VERIFIED PREMISE + V6 SYNTHESIS.

### W6G-C04 — feedstock/material/build configuration is part of AM evidence
Status: VERIFIED.
Sources: W6G-S02/S06/S07.

### W6G-C05 — machine qualification is not equivalent to full part/process qualification
Status: VERIFIED PUBLIC SCOPE.
Source: W6G-S03.

### W6G-C06 — post-processing can be integral to the final production route
Status: VERIFIED PREMISE + V6 SYNTHESIS.
Examples: support removal, heat treatment/HIP where used, machining, surface finishing, cleaning, inspection.

### W6G-C07 — prototype print success does not automatically establish serial-production qualification
Status: VERIFIED PREMISE + DEPENDENCY.
Sources: W6G-S02/S03 + A4/Wave03.

### W6G-C08 — final properties/allowables are material/process/machine/post-process/application specific
Status: VERIFIED APPLICABILITY RULE.
Sources: W6G-S04/S05/S07.

### W6G-C09 — inspection burden can increase when geometry creates inaccessible/internal features
Status: V6 SYNTHESIS + Wave02.

### W6G-C10 — AM economics must compare final accepted process chain, not printer time alone
Status: VERIFIED PREMISE + V6 SYNTHESIS.
Sources: W6G-S10/S11 + Wave03.

### W6G-C11 — AM is not inherently the more mature or advanced manufacturing route
Status: V6 SYNTHESIS.

### W6G-C12 — process/material/machine/software/feedstock/post-process change can trigger evidence-impact reassessment
Status: DEPENDENCY — Wave01.

## 5. Hard guardrails

1. no universal AM process/property capability table;
2. no generic layer thickness/orientation/support rule;
3. no universal anisotropy/property penalty;
4. no generic porosity/defect acceptance threshold;
5. no process parameter window;
6. no material allowable transferred across machine/process/post-process;
7. no PBF-LB qualification rule generalized to all AM families;
8. no printer-time-only cost comparison;
9. no claim complexity is free;
10. no prototype print = production qualification shortcut;
11. no post-processing treated as optional if required for final claim;
12. no aerospace/medical qualification burden generalized unless applicable.

## 6. Current-status lock

Checked 2026-09-19:
- ISO/ASTM 52900:2021 current/confirmed 2025.
- ISO/ASTM 52920:2023 current.
- ISO/ASTM TS 52930:2021 published/under review.
- ISO/ASTM 52924:2023 current.
- ISO/ASTM 52927:2024 current.
- ISO/ASTM 52928:2024 current.
- ISO/ASTM 52929:2025 current.
- ISO/ASTM 52926-1:2023 current.

## 7. Episode gate

EP17 can proceed without material-specific AM allowables, machine parameters, defect limits or regulated-industry qualification rules.

Current generic-script P0 blockers: 0.
