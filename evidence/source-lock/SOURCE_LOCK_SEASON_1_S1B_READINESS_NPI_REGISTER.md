# Season 1 S1-B — Industrialization / Readiness Shared Source Register

status: SHARED SOURCE REGISTER LOCKED
checked: 2026-09-19
scope: EP01 / EP02 / EP03 / EP04 / EP05
governed_by: podcast/season-1/SEASON_1_CLAUDE_HANDOFF_DELIVERY_BOARD.md
dependencies: Product Readiness source map + Waves 01–03

## 1. Purpose

Lock the external premises needed to explain the transition from a working prototype to controlled industrialization without presenting any one readiness model, phase vocabulary or industry method as universal.

S1-B owns:
- prototype success vs manufacturing evidence;
- multidimensional build maturity;
- NPI/industrialization ownership;
- product readiness vs manufacturing readiness;
- lifecycle/gate translation.

## 2. NASA technology/readiness source family

### S1B-S01 — NASA Technology Readiness Levels
Official:
https://www.nasa.gov/directorates/somd/space-communications-navigation-program/technology-readiness-levels/

Public support:
- TRL is a technology-maturity scale;
- proof of concept and fully functional prototype appear at different maturity levels;
- technology maturity does not by itself describe manufacturing readiness.

Episode use:
EP01/EP02 contextual example only.

Guardrail:
TRL is not the podcast's product/manufacturing readiness model.

### S1B-S02 — NASA NPR 7123.1D Appendix E — TRL
Official:
https://nodis3.gsfc.nasa.gov/displayDir.cfm?Internal_ID=N_PR_7123_001D_&page_name=AppendixE

Current status checked:
- NPR 7123.1D Updated with Change 2;
- effective 2023-07-05;
- expiration 2028-07-05;
- mandatory for NASA employees inside NASA scope.

Use:
current NASA TRL procedural context and explicit applicability.

### S1B-S03 — NASA NPR 7123.1D Appendix G — Production Readiness Review
Official:
https://nodis3.gsfc.nasa.gov/displayDir.cfm?Internal_ID=N_PR_7123_001D_&page_name=AppendixG

Support:
production readiness considers production plans/documentation, process controls, resources, tooling/test equipment, people/suppliers, quality and unresolved production issues.

Episode use:
EP01/EP03/EP04/EP05.

Guardrail:
NASA PRR is an aerospace/NASA review framework, not a universal commercial gate.

### S1B-S04 — NASA manufacturing-readiness contextual source
NASA technical memorandum:
https://ntrs.nasa.gov/api/citations/20220018403/downloads/TM-20220018403.pdf

Support:
manufacturing readiness can progress separately from technology readiness and includes process, tooling, production-relevant environment, sources, cost and production capability.

Use:
EP01/EP02/EP04 contextual corroboration.

Guardrail:
MRL terminology is not adopted as the podcast's universal maturity scale.

## 3. NIST NPI / production-system source family

### S1B-S05 — NIST production-line / NPI work
NIST publication page:
https://www.nist.gov/publications/challenges-setting-manufacturing-plant-during-pandemic
Underlying paper:
https://tsapps.nist.gov/publication/get_pdf.cfm?pub_id=932687

Support:
- setting up/updating a factory or production line is part of broader NPI work;
- activities include production targets, equipment/manpower capacity, capital procurement, manufacturing methods/technology and verification of production/inspection equipment/processes.

Episode use:
EP01/EP03/EP04.

Guardrail:
pandemic context is case context; the production-system activities are the transferable engineering premise.

## 4. Automotive launch-context source family

### S1B-S06 — AIAG APQP 3rd Edition public scope
Official:
https://www.aiag.org/training-and-resources/manuals/details/APQP-3

Current status:
3rd Edition, published March 2024.

Public support:
new-product launch planning includes sourcing, change management, program metrics, risk mitigation, gated management and traceability.

Use:
cross-industry corroboration that launch readiness spans product/process/supplier/change evidence.

Guardrail:
automotive APQP requirements are not universal hardware requirements.

### S1B-S07 — AIAG PPAP-4 public scope
Official:
https://www.aiag.org/training-and-resources/manuals/details/PPAP-4

Public support:
production-part approval addresses whether engineering requirements can be consistently met using actual production processes at production rates.

Use:
EP01/EP04 contextual example of production-process evidence distinct from one good prototype/sample.

Guardrail:
submission levels/elements/customer requirements remain automotive/customer specific and are not taught here.

## 5. Shared S1-B claims

### S1B-C01 — functional/technology maturity and manufacturing readiness are related but distinct
Status: VERIFIED.
Sources: S1B-S01/S02/S03/S04.

### S1B-C02 — a working prototype does not by itself establish repeatable production capability
Status: VERIFIED PREMISE + V6 SYNTHESIS.
Sources: S1B-S03/S04/S05/S07.

### S1B-C03 — production readiness is multidimensional
Status: VERIFIED PREMISE + V6 SYNTHESIS.
Sources: S1B-S03/S04/S05/S06.

### S1B-C04 — production-system development is a parallel engineering workstream, not merely a late manufacturing handoff
Status: VERIFIED.
Source: S1B-S05 + S1B-S06.

### S1B-C05 — product verification evidence and production/process evidence answer different questions
Status: VERIFIED PREMISE + V6 SYNTHESIS.
Sources: NASA product/readiness source family + S1B-S07.

### S1B-C06 — phase labels such as POC/MVP/EVT/DVT/PVT do not by themselves define evidence
Status: VERIFIED AS APPLICABILITY GUARDRAIL + V6 SYNTHESIS.
Support:
NASA uses its own TRL/PRR constructs; AIAG uses different launch constructs; company phase definitions vary.

### S1B-C07 — useful gates should be defined by evidence/decision rather than name alone
Status: V6 SYNTHESIS supported by S1B-S03/S05/S06.

### S1B-C08 — one build/sample does not prove sustained supplier/process capability
Status: VERIFIED PREMISE.
Source: S1B-S07 + Wave 02 supplier/capability lock.

### S1B-C09 — rate/yield/rework/economics belong to manufacturing readiness when they affect the intended production claim
Status: DEPENDENCY — Wave 03.

### S1B-C10 — readiness must remain tied to a defined product/process/configuration/applicability envelope
Status: DEPENDENCY — frozen global invariants / Wave 01.

## 6. Hard guardrails

1. no claim NASA TRL or MRL is a universal hardware-company lifecycle;
2. no claim EVT/DVT/PVT have one universal definition;
3. no fixed unit count proves maturity;
4. no single readiness percentage;
5. no assumption all readiness dimensions mature together;
6. no automotive APQP/PPAP requirement generalized outside applicability;
7. no NASA PRR process transplanted as startup bureaucracy;
8. no “NPI starts at design handoff” rule;
9. no supplier sample = production capability shortcut;
10. quantitative rate/yield/cost examples must reuse checked Wave 03 assumptions or remain illustrative.

## 7. Episode mapping

EP01:
S1B-S03/S04/S05/S07 + Waves 01–03.

EP02:
S1B-S01/S02/S04 + A4 representativeness.

EP03:
S1B-S03/S05/S06 + ownership/change dependencies.

EP04:
S1B-S01/S03/S04/S05/S06/S07.

EP05:
source family used only to show vocabulary/framework diversity; Phase Evidence Card is internal synthesis.

## 8. Current generic blockers

No intended EP01–05 script requires protected APQP/PPAP detail, one universal lifecycle definition or an unverified numeric readiness threshold.

Current generic-script P0 blockers: 0.
