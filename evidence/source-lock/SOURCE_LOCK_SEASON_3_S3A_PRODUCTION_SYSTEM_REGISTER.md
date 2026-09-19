# Season 3 S3-A — Production System Engineering Shared Source Register

status: SHARED SOURCE REGISTER LOCKED
checked: 2026-09-19
scope: EP20 / EP21 / EP22 / EP25
governed_by: podcast/season-3/SEASON_3_CLAUDE_HANDOFF_DELIVERY_BOARD.md
dependencies: Waves 01/02/03 + Season 1 DFX + ISA-95 context

## 1. Purpose

Lock the generic engineering premises required to translate a released product definition into an executable production system without treating any ERP/MES convention, work-instruction template, fixture rule, training scheme or factory-layout heuristic as universal.

S3-A owns:
- manufacturing definition / routing;
- tooling/fixtures/equipment;
- standard work / operator qualification;
- layout / material flow / WIP / ergonomics.

## 2. Process planning / routing source family

### S3A-S01 — NIST Conceptual Process Planning
Official:
https://www.nist.gov/publications/conceptual-process-planning-definition-and-functional-decomposition

Support:
process planning identifies manufacturing activities and is part of early manufacturability/cost reasoning.

Use:
EP20/EP21.

### S3A-S02 — NIST Categorical Models for Process Planning
Official:
https://www.nist.gov/publications/categorical-models-process-planning

Support:
process plans structure:
- tasks;
- resources;
- relationships/constraints;
and guide operational decisions.

Use:
EP20.

### S3A-S03 — NIST Information Modeling on Conceptual Process Planning
Official:
https://www.nist.gov/publications/information-modeling-conceptual-process-planning-integrated-conceptual-design

Support:
process planning includes:
- process selection;
- resource selection;
- cost/time estimation;
- information sharing.

Use:
EP20/EP21.

### S3A-S04 — ISA-95 Part 3 public scope
Owner: ISA
Official:
https://www.isa.org/standards-and-publications/isa-standards/isa-95-standard

Current public status:
ANSI/ISA-95.00.03-2013 remains the listed Part 3 publication.

Public support:
manufacturing operations management activity models and exchanged information can be represented explicitly.

Use:
EP20 as semantic/contextual corroboration.

Guardrail:
ISA-95 does not mandate one EBOM/MBOM/routing data model or one ERP/MES implementation.

## 3. Production readiness / tooling / procedures / people source family

### S3A-S05 — NASA NPR 7123.1D Appendix G — PRR
Official:
https://nodis3.gsfc.nasa.gov/displayDir.cfm?Internal_ID=N_PR_7123_001D_&page_name=AppendixG

Current applicability:
NASA-specific procedural requirement context.

Public support:
PRR examines:
- design documentation;
- production plans;
- process controls/procedures;
- facilities/tools;
- special tools/test equipment;
- qualified production/support staff;
- suppliers;
- manufacturing readiness.

Use:
EP20/EP21/EP22.

Guardrail:
NASA PRR is not imposed as a commercial-startup gate.

### S3A-S06 — NIST Training Within Industry (TWI)
Official:
https://www.nist.gov/mep/training-within-industry-twi

Public support:
- Job Instruction standardizes how jobs are taught;
- structured instruction is intended to help workers perform jobs correctly and consistently.

Use:
EP22.

Guardrail:
TWI is a methodology/context, not a universal legal qualification scheme.

## 4. Flow / WIP / material-handling source family

### S3A-S07 — NIST TN 1890 — Inventory and Flow Time in US Manufacturing
Official:
https://www.nist.gov/publications/inventory-and-flow-time-us-manufacturing-industry

Support:
manufacturing waste/flow analysis includes:
- transportation;
- rework/defects;
- motion;
- inventory;
- waiting;
and flow time/WIP are meaningful system variables.

Use:
EP25.

### S3A-S08 — NIST supply-chain flow-time work
Official:
https://www.nist.gov/publications/examination-national-supply-chain-flow-time

Support:
flow time and bottlenecks can be analyzed across manufacturing systems.

Use:
EP25 context.

## 5. Ergonomics source family

### S3A-S09 — NIOSH Ergonomics / Risk Factors
Official:
https://www.cdc.gov/niosh/ergonomics/ergo-programs/risk-factors.html

Public support:
physical risk factors include:
- awkward posture;
- force;
- lifting/carrying;
- repetition;
- static posture;
- vibration.

Use:
EP25.

### S3A-S10 — Revised NIOSH Lifting Equation
Official:
https://www.cdc.gov/niosh/ergonomics/about/rnle.html

Public support:
manual-lifting risk depends on task geometry, load, frequency, duration and coupling.

Use:
EP25 as an example of why ergonomics is task-specific.

Guardrail:
EP25 does not teach RNLE calculations or universal lift limits.

## 6. Shared engineering claims

### S3A-C01 — released product definition is not yet an executable production system
Status: VERIFIED PREMISE + V6 SYNTHESIS.
Sources: S3A-S01/S02/S03/S05.

### S3A-C02 — process/routing definition includes tasks, sequence, resources and constraints
Status: VERIFIED.
Sources: S3A-S02/S03.

### S3A-C03 — EBOM/MBOM/routing distinctions are implementation models, not universal one-to-one taxonomies
Status: V6 SYNTHESIS + ISA-95 guardrail.

### S3A-C04 — alternate/rework routes require controlled identity/history/effectivity when they affect product evidence
Status: DEPENDENCY — Wave01.

### S3A-C05 — tooling/fixtures/equipment are production-enabling engineering objects, not merely shop aids
Status: VERIFIED PREMISE + V6 SYNTHESIS.
Source: S3A-S05.

### S3A-C06 — fixture/tool validity can change through wear, calibration/verification state, maintenance and product/process revision
Status: V6 SYNTHESIS + Waves01/02/04.

### S3A-C07 — work instructions and standard work are execution definitions, but training attendance alone does not prove competent execution
Status: VERIFIED PREMISE + V6 SYNTHESIS.
Sources: S3A-S05/S06.

### S3A-C08 — hidden expert knowledge should be converted into explicit process definition or architecture/control where consequential
Status: V6 SYNTHESIS + Season1 A5/A6/EP07.

### S3A-C09 — layout should be designed around routing, material/operator flow, WIP, inspection and abnormal paths rather than equipment placement alone
Status: VERIFIED PREMISE + V6 SYNTHESIS.
Sources: S3A-S07/S08/S09.

### S3A-C10 — WIP can expose or absorb variation but is not itself system capacity
Status: DEPENDENCY — Wave03 + S3A-S07.

### S3A-C11 — ergonomics can affect safety, fatigue, consistency and practical process execution
Status: VERIFIED PREMISE + V6 SYNTHESIS.
Sources: S3A-S09/S10.

### S3A-C12 — layout/tooling/work-instruction changes can invalidate affected production evidence and require impact review
Status: DEPENDENCY — Wave01 global invariant.

## 7. Hard guardrails

1. no universal EBOM/MBOM schema;
2. no mandatory ERP/MES/PLM ownership assignment;
3. no universal routing object model;
4. no generic fixture tolerance ratio or fixture-life rule;
5. no universal tooling calibration interval;
6. no universal training-hour/certification requirement;
7. no claim reading a WI equals qualification;
8. no universal aisle width / WIP quantity / staffing ratio;
9. no universal lifting threshold derived from RNLE without task analysis;
10. no assumption all WIP is waste or all buffers are bad;
11. no NASA PRR process imposed outside NASA applicability;
12. no machinery-safety/EHS legal requirement without jurisdiction/application source.

## 8. Episode mapping

EP20:
S3A-S01/S02/S03/S04 + Wave01.

EP21:
S3A-S03/S05 + Waves01/02/04.

EP22:
S3A-S05/S06 + Season1 EP07 + Wave01.

EP25:
S3A-S07/S08/S09/S10 + Wave03.

## 9. Episode gate

EP20/21/22/25 can proceed to claim locks and technical review without universal software schemas, fixture rules, training requirements or layout dimensions.

Current generic-script P0 blockers: 0.
