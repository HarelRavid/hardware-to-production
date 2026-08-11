# Pass 2.02 — Configuration & Change Control

status: ACTIVE — EVIDENCE BACKBONE + WORKED EXAMPLE STARTED
created_on: 2026-08-11
maps_to: Opening Arc; Episodes 3–5, 20–31, 35, 39, 60
companion: P2_01_WORKED_EXAMPLE_SENTINEL_NODE.md; P2_01_DEV_LVP_SVP_READINESS_MATRIX.md

## Purpose
Teach a hardware team how to answer, at any point in development or production:
1. What exactly is the approved product definition?
2. What exactly did we build?
3. What changed, why, who approved it and when did it become effective?
4. Which units/lots/builds contain the change?
5. Which prior verification/qualification evidence remains valid after the change?

The goal is not enterprise bureaucracy. It is preservation of engineering truth as hardware, software, suppliers and manufacturing processes evolve.

## Evidence backbone
### NASA Systems Engineering Handbook — Configuration Management
NASA describes configuration management across the product life cycle as a discipline for visibility and control of functional and physical characteristics and changes. It identifies five core elements:
- configuration planning/management;
- configuration identification;
- configuration change management;
- configuration status accounting (CSA);
- configuration verification/audit.

NASA further describes a baseline as an agreed product description at a point in time that becomes the known configuration against which subsequent changes are addressed.

Applicability boundary: NASA program governance is not prescribed as startup process. The transferable concepts are identification, baseline, controlled change, status/history and verification.

### Configuration identification is prerequisite infrastructure
A configuration item must be identifiable before its changes and history can be controlled. Product definition may include hardware, software/firmware, drawings, BOMs, requirements, process/test definitions and other controlled artifacts where their identity affects product truth.

### Change control is more than approval
A useful change lifecycle is:
**Need/problem → proposed change → impact assessment → decision/approval → implementation plan → effectivity/cut-in → verification/requalification → closure/status accounting.**

NASA describes change management as systematic proposal, justification and evaluation followed by incorporation of approved changes and verification of implementation.

### Status accounting preserves current and historical truth
NASA CSA guidance calls for current and historical configuration documentation and status of proposed changes, deviations and waivers. For hardware-to-production this supports the practical requirement to reconstruct what definition applied to a particular build and what changes were pending or implemented.

## Core distinctions
### Definition vs as-built
**Definition** = what should be built under an approved configuration.
**As-built** = what was actually installed/assembled/programmed/tested on a particular unit or lot.

They may diverge because of deviation, rework, alternate components, firmware loading, supplier substitution or implementation error. A controlled system must not silently overwrite this distinction.

### Revision vs effectivity
**Revision** answers: what definition/version exists?
**Effectivity** answers: where/when/for which serials/lots/orders does that revision apply?

Publishing revision C does not prove every unit after the publication timestamp contains revision C.

### Engineering change vs deviation/waiver
An engineering change modifies the controlled baseline/definition.
A deviation/waiver permits a bounded departure from a requirement or definition under explicit authorization and scope; it should not silently become the new baseline.

Terminology varies by company/industry. Preserve the semantic distinction even when local names differ.

### Product change vs process change
A product-definition change and a manufacturing-process change are different objects but may invalidate the same evidence. Examples:
- sensor supplier change without drawing change;
- solder profile change;
- molding tool repair affecting geometry;
- calibration algorithm update;
- work-instruction torque change.

The impact assessment must therefore cross product, process, supplier, test, quality, service and compliance boundaries as applicable.

## Sentinel Node worked example — configuration stack
For each serialized Sentinel Node, preserve enough identity to reconstruct at least:
- finished-good part number + revision;
- PCB assembly revision;
- PCB bare-board revision where material;
- sensor manufacturer/part/source status and lot where needed;
- enclosure revision and manufacturing route/tool revision where material;
- gasket/seal specification revision/lot where needed;
- firmware release/build identifier;
- calibration/test software version;
- routing/work-instruction revision for critical operations;
- deviations/rework affecting the unit;
- final test/calibration record;
- manufacturing date/lot/serial genealogy.

This is not a universal mandatory field list. Capture the minimum identity needed to preserve requirement, failure, quality, service and change decisions for the product risk/context.

## Worked change — alternate vibration sensor
### Trigger
Primary vibration sensor has a supply shortage during ramp.
Purchasing finds an alternate with similar headline range and package.

### Bad implementation
1. Buyer substitutes alternate part in ERP.
2. Assembly fits physically.
3. One unit passes a bench functional check.
4. Production continues.

Why this is dangerous: the substitution may affect sensitivity, frequency response, noise, temperature behavior, firmware coefficients, calibration, test limits, PCB loading, EMC, reliability or regulatory evidence.

### Controlled implementation
#### 1. Identify the proposed change
- old sensor/source;
- proposed alternate;
- affected product configurations;
- reason: shortage/resilience/cost/etc.;
- requested implementation timing.

#### 2. Impact assessment
Ask which requirements/evidence may be affected:
- sensing accuracy/bandwidth;
- environmental performance;
- firmware/driver behavior;
- calibration model;
- production test coverage/limits;
- mechanical fit and assembly process;
- electrical power/interface;
- reliability/lifetime;
- supplier/process qualification;
- compliance/certification where applicable;
- service/spares/interchangeability.

#### 3. Decide required evidence
Possible result:
- dimensional/electrical review;
- engineering samples;
- bench comparison;
- environmental regression subset;
- firmware/calibration update;
- production-test update;
- supplier qualification evidence;
- pilot lot before broad release.

Do not default to full requalification or to no requalification. Scope evidence to the assumptions affected by the change.

#### 4. Approve definition
If accepted, release controlled BOM/drawing/firmware/test changes with linked rationale and evidence.

#### 5. Define effectivity
Examples:
- serial number 2501 onward;
- manufacturing order X onward;
- after depletion of old lot;
- dual-approved sources under defined applicability;
- temporary deviation for specified quantity/date while permanent change remains under evaluation.

#### 6. Implement and verify cut-in
Confirm that the shop-floor/CM/ERP/MES/test definitions actually changed and that first affected builds match the intended configuration.

#### 7. Preserve genealogy
For any field failure, quality excursion or later evidence question, identify which units contain old vs alternate sensor and which firmware/calibration/test versions were paired with them.

## Change impact matrix
| Change | Potentially affected evidence |
|---|---|
| PCB layout revision | EMC, thermal, functional, assembly/test, reliability |
| firmware algorithm | functional/performance, calibration, safety behavior, test compatibility |
| sensor supplier/part | performance, calibration, reliability, supplier qualification, test limits |
| CNC → molded enclosure | geometry/tolerance, sealing, material/environmental, assembly, tooling/process capability |
| gasket material | sealing, chemical/environmental aging, compression/process controls |
| solder/process profile | joint reliability, defects, inspection/control plan, special-process evidence as applicable |
| test fixture/software | measurement/test adequacy, historical comparability, false accept/reject risk |
| work-instruction torque | assembly integrity, sealing, reliability, operator/control-plan evidence |

## Evidence invalidation test
For every meaningful change ask:
1. What prior claim/evidence are we relying on?
2. What configuration/process/environment assumptions made it valid?
3. Which assumptions does this change touch?
4. Is existing evidence still directly applicable?
5. If not, what analysis/regression/reverification/requalification is proportionate?
6. How will affected units/lots be identified?

## Minimum startup change record
A lightweight but useful change record can contain:
- change ID/title;
- problem/reason;
- affected items/current revisions;
- proposed definition;
- impact/risk assessment;
- evidence required;
- decision/approvers;
- released revisions;
- effectivity/cut-in rule;
- verification of implementation;
- affected serial/lot/build range;
- linked deviations/NCRs/tests where applicable;
- closure status.

The sophistication of the tool can scale from a controlled spreadsheet/repository to PLM/MES/QMS integration. The information relationships matter more than buying a particular platform too early.

## DEV / LVP / SVP lens
### DEV
Minimum goal: know what configuration produced each important engineering result. Git commits, BOM snapshots, build notes and explicit prototype identities may be enough for low-risk early work.

### LVP
Configuration becomes production infrastructure. Controlled BOM/drawings/firmware/work instructions, change authority, deviations, effectivity and as-built reconstruction should be operational.

### SVP
Configuration/change control must scale across suppliers, lots/serials, sites, software, process changes, service/field feedback and sustained production without losing historical truth.

## Claims
### P2-C-CM-001 — A successful test result is weak evidence if the tested configuration cannot be reconstructed
status: STRONG SYNTHESIS
basis: NASA configuration identification/status accounting + readiness/evidence-transfer logic.

### P2-C-CM-002 — Release revision and production effectivity are different concepts
status: STRONG SYNTHESIS
needs deeper industry-standard corroboration for formal effectivity terminology before Podcast Ready.

### P2-C-CM-003 — An approved change is not complete until implementation and applicable verification are confirmed
status: STRONG EVIDENCE
basis: NASA change-management sequence includes incorporation and verification.

### P2-C-CM-004 — Supplier/component substitution can require re-evaluation even if form/fit appears unchanged
status: STRONG SYNTHESIS
requires domain-specific examples/standards for episode examples.

### P2-C-CM-005 — Deviation/waiver should remain distinguishable from a baseline engineering change
status: STRONG EVIDENCE / terminology-context dependent
basis: NASA distinguishes engineering change from waiver; local industry terminology varies.

## Myths to challenge
- “The BOM in ERP tells us exactly what every unit contains.”
- “Revision C was released Monday, so everything built Tuesday is Rev C.”
- “Same package and specification headline means drop-in equivalent.”
- “If a change was approved, change control is finished.”
- “A deviation is basically a temporary revision.”
- “Firmware is separate from hardware configuration.”

## Next depth work
1. Add authoritative EIA-649 / industry CM corroboration where publicly accessible.
2. Build effectivity/cut-in worked table for Sentinel Node serials/lots.
3. Build a change-impact/reverification decision tree.
4. Connect supplier change rules from A6.
5. Connect process/test change evidence from A4/A5/A7.
6. Convert to podcast listener tool and Research Pack.

## Readiness
CM evidence backbone: CAPTURED
Sentinel worked change: CAPTURED
Effectivity worked example: NEXT
Reverification decision tree: NEXT
Podcast readiness: IN PROGRESS
