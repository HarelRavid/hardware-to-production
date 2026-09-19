# Source-Lock Wave 06B — Polymers / Forming / Elastomers Shared Source Register

status: SHARED SOURCE REGISTER LOCKED
checked: 2026-09-19
scope: EP12 — Polymer Parts: Injection Molding and the Alternatives
dependencies: Wave 06A process selection + Wave 03 economics + Wave 02 measurement/quality

## 1. Purpose

Lock the generic engineering premises required to teach polymer manufacturing route selection without turning material- or supplier-specific DFM rules into universal laws.

EP12 uses injection molding as the anchor process and compares alternate polymer-forming/bridge routes at a high level.

## 2. Current standards / authoritative source register

### W6B-S01 — ISO 20457:2026
Owner: ISO
Title: Plastics moulded parts — Tolerances and acceptance conditions
Edition: 2
Published: 2026-08
Official record:
https://www.iso.org/standard/20457.html
OBP:
https://www.iso.org/obp/ui#iso:std:iso:20457:ed-2:v1:en

Current-status finding:
ISO 20457:2026 replaced ISO 20457:2018 on 2026-08-06.

Public support:
- plastic moulded-part dimensional/geometric tolerances require a plastics-specific framework;
- dimensional/form/location variation can be driven by material behaviour, moulding shrinkage, processing conditions, geometry, warpage and non-uniform cooling;
- applies to non-porous moulded thermoplastics, thermoplastic elastomers and thermosets using stated moulding processes.

Episode use:
moulded plastic ≠ machined-metal tolerance assumptions; tolerance/geometry/process coupling.

Guardrail:
surface imperfections such as sink marks and joint lines are explicitly outside this standard's scope; use separate technical sources for those mechanisms.

### W6B-S02 — ISO 294-1:2017
Owner: ISO
Title: Plastics — Injection moulding of test specimens of thermoplastic materials — Part 1
Edition: 2
Current status: confirmed/current.
Official source:
https://www.iso.org/standard/67036.html

Public support:
- reproducible injection-moulding reference specimens require controlled/consistent moulding conditions;
- mould design is an important factor;
- exact conditions vary by material.

Episode use:
process conditions and mould design materially influence produced state.

Guardrail:
test-specimen preparation standard is not a universal production-part DFM specification.

### W6B-S03 — ISO 294-4:2018
Owner: ISO
Title: Plastics — Injection moulding of test specimens of thermoplastic materials — Part 4: Determination of moulding shrinkage
Edition: 3
Current status: confirmed 2024/current.
Official source:
https://www.iso.org/standard/70413.html

Public support:
- injection-moulding shrinkage can differ parallel and normal to melt-flow direction;
- post-moulding effects can include humidity uptake;
- shrinkage is material/process-state dependent.

Episode use:
shrinkage is not one universal isotropic scalar.

### W6B-S04 — ISO 62:2008
Owner: ISO
Title: Plastics — Determination of water absorption
Edition: 3
Current status: confirmed/current.
Official source:
https://www.iso.org/standard/41672.html

Public support:
controlled methods for moisture/water absorption of plastics.

Episode use:
material moisture/conditioning can matter to dimensional/property state for susceptible materials.

Guardrail:
does not imply every polymer is strongly moisture sensitive or prescribe production drying settings.

### W6B-S05 — BASF grade-specific injection-moulding data example
Owner: BASF
Example:
Ultramid B3WG7 (PA6-GF35)
https://plastics-rubber.basf.com/global/en/performance_polymers/products/ultramid/30055646

Public support:
- grade-specific moulding shrinkage values differ parallel vs normal to flow;
- properties can differ dry vs conditioned;
- processing/property data belongs to exact grade/state.

Episode use:
concrete proof that “plastic” or even “PA6” is insufficient material definition.

Guardrail:
BASF values are specific to the cited compound/test conditions and are not generalized.

### W6B-S06 — BASF polyamide/PPA moisture and dimensional-state examples
Owner: BASF
Sources:
https://plastics-rubber.basf.com/emea/en/performance_polymers/fpgs/polyphthalamides
https://plastics-rubber.basf.com/emea/en/performance_polymers/products/ultramid_advanced_t1000

Support:
different polyamide/PPA chemistries/grades show different water uptake and dimensional/property behaviour.

Episode use:
grade/state/conditioning matter.

### W6B-S07 — Autodesk Moldflow warpage technical guidance
Owner: Autodesk
Sources:
https://help.autodesk.com/cloudhelp/2024/ENU/MoldflowInsight-CLC-Results/files/Warp-analysis-results/MoldflowInsight_CLC_Results_Warp_analysis_results_Material_orientation_results_html.html
https://help.autodesk.com/cloudhelp/2026/ENU/MoldflowInsight-CLC-Analyses/files/analysis-sequences/Warp-analysis/MoldflowInsight_CLC_Analyses_analysis_sequences_Warp_analysis_Isolate_cause_of_warpage_html.html

Technical support:
warpage can be driven by differential cooling, differential shrinkage, orientation effects and geometry/corner effects; material/filler orientation can change shrinkage direction.

Episode use:
warpage is a coupled material/process/geometry result, not simply “wrong CAD.”

### W6B-S08 — Autodesk Moldflow sink-mark technical guidance
Owner: Autodesk
Source:
https://help.autodesk.com/cloudhelp/2023/ENU/MoldflowInsight-CLC-Troubleshoot/files/Troubleshooting-molding-problems/LM_SINK_MARKS_AND_VOIDS.html

Support:
sink/void risk is related to localized thick sections, volumetric shrinkage, packing/gate freeze and thermal/process conditions.

Episode use:
thick features/ribs/bosses and packing/cooling design interact.

Guardrail:
no numeric rib/wall ratio from Moldflow guidance is used as a universal rule.

### W6B-S09 — Autodesk Moldflow weld/meld-line technical guidance
Owner: Autodesk
Source:
https://help.autodesk.com/cloudhelp/2025/ENU/MoldflowInsight-CLC-Results/files/Fill-or-flow-results/MoldflowInsight_CLC_Results_Fill_or_flow_results_Weld_and_meld_lines_result_html.html

Support:
weld/meld lines occur where separated flow fronts meet; structural/cosmetic consequence depends on material/fillers, temperature, pressure and location.

Episode use:
gating/flow path can create product-relevant local features.

Guardrail:
no universal weld-line strength penalty is claimed.

### W6B-S10 — Covestro gate-design technical paper
Owner: Covestro
Source:
https://solutions.covestro.com/-/media/covestro/solution-center/whitepapers/gate-design-for-high-quality-surface-finish.pdf

Support:
gate design, wall thickness/flow length and packing can affect filling/surface quality and sink behaviour.

Episode use:
tool/gate architecture is part of product/process design.

### W6B-S11 — DuPont public polymer/mould-design training
Owner: DuPont
Source:
https://www.dupont.com/mobility/webinars.html

Public scope:
covers plastic design, mould design, runners/gates/vents/cooling/ejection/shrinkage and injection-moulding process fundamentals.

Episode use:
industry-primary corroboration of tooling/process coupling.

### W6B-S12 — Wave 06A / Wave 03 bridge-route economics
Dependencies:
- W6A process-selection lock;
- Wave 03 economics.

Use:
bridge manufacturing / tooling/NRE / design-change flexibility / accepted-good-output economics.

## 3. EP12 engineering claims

### W6B-C01 — a polymer part is defined by exact material grade/state and process, not “plastic” alone
Status: VERIFIED + V6 SYNTHESIS.
Sources: W6B-S03/S04/S05/S06.

### W6B-C02 — injection moulding creates a process-specific state through filling, packing, cooling and ejection/tool interaction
Status: VERIFIED PREMISE + V6 SYNTHESIS.
Sources: W6B-S02/S07/S08/S09/S11.

### W6B-C03 — moulded dimensional behaviour should not be assumed equivalent to machined prototype dimensions
Status: VERIFIED.
Source: W6B-S01 + Wave 01 representativeness.

### W6B-C04 — shrinkage is directional/material/process dependent and should not be treated as one universal scalar
Status: VERIFIED.
Sources: W6B-S03/S05/S07.

### W6B-C05 — warpage can arise from differential cooling, differential shrinkage and orientation effects
Status: VERIFIED TECHNICAL GUIDANCE.
Source: W6B-S07.

### W6B-C06 — sink/void risk is related to local section geometry plus packing/cooling/material behaviour
Status: VERIFIED TECHNICAL GUIDANCE.
Source: W6B-S08.

### W6B-C07 — weld/meld lines are process-flow features whose consequence is location/material/process dependent
Status: VERIFIED TECHNICAL GUIDANCE.
Source: W6B-S09.

### W6B-C08 — gate/tooling/ejection/cooling decisions are part of the product/process architecture
Status: VERIFIED PREMISE + V6 SYNTHESIS.
Sources: W6B-S02/S10/S11.

### W6B-C09 — moisture/conditioning can materially affect some polymer grades; exact behaviour is material specific
Status: VERIFIED.
Sources: W6B-S04/S05/S06.

### W6B-C10 — alternate polymer routes should be compared by natural geometry/forming mechanism/tooling/secondary operations/economics rather than one maturity ranking
Status: V6 SYNTHESIS.
Dependencies: polymer-forming domain map + Wave 06A.

### W6B-C11 — bridge routes can be valid when they answer the needed product claim and their missing production mechanisms are explicit
Status: DEPENDENCY — Wave 06A + Wave 01.

### W6B-C12 — no generic draft/wall/shrinkage/tolerance/process-window value applies across all polymers/tools/parts
Status: VERIFIED GOVERNANCE RULE.
Support: W6B-S01/S02/S03/S05.

## 4. Process-family map for EP12

High-level listener map only:
- injection moulding;
- extrusion;
- blow moulding;
- thermoforming;
- rotational moulding;
- compression/transfer/reactive moulding;
- machining/additive/soft-tool bridge routes.

These categories are descriptive/synthesis for route comparison.
EP12 does not publish unsourced process-family capability tables.

## 5. Hard guardrails

1. no universal wall-thickness rule;
2. no universal draft angle;
3. no universal rib/boss thickness percentage;
4. no universal shrink factor;
5. no universal moulding tolerance beyond the exact applicable standard/material/process;
6. no universal drying temperature/time or moisture target;
7. no claim all polyamides or all plastics behave alike;
8. no “injection moulding wins above X volume” threshold;
9. no assumption CNC prototype sealing/dimensions automatically transfer to moulded production;
10. no supplier/material data generalized beyond cited grade/process conditions;
11. no simulation result treated as qualification evidence by itself;
12. exact material/process/customer requirements remain application-specific.

## 6. Current-status lock

- ISO 20457:2026 Edition 2 — current, replaced 2018 edition.
- ISO 294-1:2017 Edition 2 — current/confirmed.
- ISO 294-4:2018 Edition 3 — current/confirmed.
- ISO 62:2008 Edition 3 — current/confirmed.

## 7. Episode gate

EP12 can proceed without clause-level proprietary standard content or universal DFM numbers.

Current generic-script P0 blockers: 0.
