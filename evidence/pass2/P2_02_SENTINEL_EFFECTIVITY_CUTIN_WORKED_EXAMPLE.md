# Pass 2.02 — Sentinel Node Effectivity / Cut-In Worked Example

status: ACTIVE — WORKED EXAMPLE
created_on: 2026-08-11
maps_to: Opening A8; Episodes 4–5, 25, 29–31, 39–40, 60
companion: P2_02_CONFIGURATION_CHANGE_CONTROL.md; P2_01_WORKED_EXAMPLE_SENTINEL_NODE.md

## Purpose
Show how one seemingly simple component substitution propagates across engineering definition, firmware, production, WIP, deviations, test evidence and genealogy. The example is fictional but structured around real configuration-management principles.

## Scenario
Sentinel Node uses vibration sensor `VS-A`, supplier `S1`, in released product configuration Rev B.

During ramp, supplier S1 announces a long lead-time disruption. Purchasing proposes alternate sensor `VS-B` from supplier `S2`.

VS-B is mechanically compatible at the package level and has similar nominal sensing range, but differs in:
- sensitivity tolerance;
- digital filtering behavior;
- startup timing;
- calibration coefficients;
- recommended PCB decoupling/layout details;
- firmware device ID/register map;
- supplier/process pedigree.

Therefore the change is not treated as a purchasing-only substitution.

## Baseline before change
Released product definition:
- Product: Sentinel Node
- Product revision: Rev B
- PCB assembly: PCA-100 Rev B
- vibration sensor: VS-A / S1
- firmware: FW 1.8.2
- enclosure: ENC-210 Rev C
- final test procedure: FTP-020 Rev 5
- calibration procedure: CAL-012 Rev 3
- work instruction: WI-ASSY-014 Rev 4

Known effectivity:
- Rev B configuration effective from serial SN-0101
- normal production currently at SN-0260
- WIP includes SN-0261 to SN-0280 at different assembly states

## Change request
Change ID: ECO-027
Reason: supply interruption / alternate-source qualification
Requested change: permit VS-B/S2 as an approved production sensor where qualification conditions are met.

## Impact assessment
### Requirements impact
Check whether VS-B still satisfies:
- measurement range;
- accuracy/sensitivity requirement;
- frequency response;
- startup/availability timing;
- temperature/environment limits;
- diagnostic behavior.

### Mechanical impact
Package is nominally compatible, but mounting stress and orientation assumptions are reviewed.

### Electrical/PCB impact
Review:
- pinout;
- supply current;
- decoupling;
- signal integrity;
- layout constraints;
- EMC implications.

### Firmware impact
VS-B requires a driver branch and configuration table change.

Proposed firmware: FW 1.9.0.

### Calibration/test impact
CAL-012 Rev 3 assumes VS-A coefficient behavior.
FTP-020 Rev 5 verifies one register/diagnostic response unique to VS-A.

Both require revision or conditional logic.

### Supplier/process impact
S2 has not yet been production-qualified for this product.
Need incoming identity/lot controls and defined approval evidence.

### Reliability/environment evidence impact
Prior vibration accuracy/environment tests used VS-A.
Determine which tests can transfer analytically and which require regression/reverification with VS-B.

## Evidence decision
Evidence is split into four classes.

### Transfers with no new test
Evidence where changed sensor is not relevant to the supported claim, for example enclosure dimensional inspection.

### Transfers with engineering analysis
Evidence where equivalence can be justified through specification/design review and risk assessment.

### Requires targeted regression/reverification
Examples:
- sensor accuracy across temperature;
- startup timing;
- diagnostic/fault handling;
- calibration repeatability;
- firmware compatibility.

### Requires broader requalification if triggered
If PCB/layout, EMC behavior, thermal load or other system interactions change materially, broader qualification may be required.

The correct class is determined by the requirement and the assumptions behind the original evidence, not by how visually similar the components are.

## Released change package
After qualification:
- PCA-100 Rev C permits VS-B layout/component option where applicable
- FW 1.9.0 supports VS-A and VS-B with explicit sensor identity
- FTP-020 Rev 6 records detected sensor type and firmware
- CAL-012 Rev 4 contains sensor-specific calibration logic
- WI-ASSY-014 Rev 5 adds sensor identity verification
- approved-vendor/material list updated
- ECO-027 approved with effectivity and WIP disposition

## Effectivity plan
The team chooses serial-based normal effectivity:
- VS-B normal production authorization starts at SN-0291
- SN-0291 onward must use the Rev C configuration set unless a controlled deviation says otherwise

This does NOT mean every unit physically built after the release date automatically follows Rev C.

## WIP disposition table
| Serial range | State when ECO approved | Sensor physically installed | Planned disposition | Final configuration record |
|---|---|---|---|---|
| SN-0261–0268 | final assembly/test | VS-A | finish as Rev B | Rev B / FW 1.8.2 |
| SN-0269–0274 | PCB assembled | VS-A | finish as Rev B | Rev B / FW 1.8.2 |
| SN-0275–0280 | kit staged, sensor not installed | VS-A kits reserved | finish as Rev B unless shortage forces deviation | Rev B unless deviation recorded |
| SN-0281–0290 | not started | mixed material availability | transition validation lot under ECO | explicit transition configuration per unit |
| SN-0291+ | normal production after cut-in | VS-B authorized | build to Rev C baseline | Rev C / FW 1.9.0, sensor identity recorded |

## Temporary deviation example
A customer urgently needs five units while qualification is nearly complete.

Deviation: DEV-011
Scope: SN-0284–0288 only
Permits: VS-B + FW 1.9.0-rc2 under enhanced test and engineering review
Expiration: automatically closes after SN-0288; cannot be reused for later serials
Required genealogy:
- sensor supplier/lot;
- firmware build hash/version;
- deviation ID;
- calibration data;
- enhanced test result;
- approving authority.

These five units are NOT silently treated as standard Rev C production evidence unless the qualification plan explicitly accepts them for that purpose.

## Definition versus as-built example
For SN-0286:

Nominal baseline at production date might already show Rev C as current.
Actual as-built record must instead show:
- transition/deviation configuration;
- VS-B supplier/lot;
- PCB revision actually used;
- FW 1.9.0-rc2;
- DEV-011;
- CAL/FTP versions;
- rework if any;
- final acceptance result.

This is why “current BOM” cannot reconstruct historical truth.

## Change-impact / reverification decision tree
For every proposed change:

1. **What changed?**
   - requirement / part / material / supplier / process / tooling / software / test / site / sub-tier?
2. **What requirements or CTQs can it affect?**
3. **What prior evidence supports those requirements today?**
4. **What assumptions made that evidence valid?**
5. **Did the change alter any of those assumptions?**
   - No → evidence may transfer; document rationale.
   - Yes, bounded → targeted analysis/regression/reverification.
   - Yes, material/system-level → requalification scope assessment.
6. **What released objects must change?**
   - BOM/drawing/PCB/firmware/work instruction/control plan/test/calibration/supplier approval/etc.
7. **What is the effectivity rule?**
   - serial / lot / work order / date + controlled inventory/WIP rule.
8. **What happens to WIP and existing stock?**
9. **How will as-built genealogy prove what each unit received?**
10. **What closes the change?**
   - evidence complete, released documents, cut-in verified, affected WIP dispositioned, audit trail complete.

## Listener checklist — before approving any production change
- Change reason is explicit.
- Affected requirements/CTQs identified.
- Prior evidence impact assessed.
- New verification/requalification scope defined.
- All affected product/process/test/software documents identified.
- Supplier/sub-tier impact assessed.
- WIP and inventory disposition defined.
- Effectivity boundary is unambiguous.
- Temporary deviations have explicit scope/expiry.
- As-built genealogy can distinguish old/new/transition units.
- First cut-in units are verified.
- Change closure confirms implementation, not only document approval.

## Claims illustrated
### P2-C-CM-001 — Revision release and physical effectivity are separate events
status: STRONG SYNTHESIS grounded in CM/change-accounting principles.

### P2-C-CM-002 — A production change can invalidate only part of the prior evidence; re-verification scope should follow affected requirements and assumptions
status: STRONG ENGINEERING SYNTHESIS.

### P2-C-CM-003 — Definition data and as-built genealogy answer different questions
status: STRONG.

### P2-C-CM-004 — Temporary deviation requires controlled scope and expiry; otherwise it becomes an uncontrolled alternate configuration
status: STRONG ENGINEERING DIRECTION.

## Podcast use
This example can support:
- Opening A8 configuration management;
- Episode 4 design maturity;
- Episode 5 production readiness;
- engineering-change episodes;
- supplier-change episodes;
- ramp/change-cut-in discussion;
- Manufacturing Atlas genealogy/effectivity arc;
- Episode 60 full decision story.

## Next P2.02 work
1. connect the worked example to formal CM terminology/source evidence;
2. create a compact ECR/ECO/deviation/effectivity object model;
3. add firmware/hardware co-configuration rule;
4. technical-review the change-impact tree against sector-specific change frameworks without universalizing them;
5. create show-note-ready one-page change checklist.