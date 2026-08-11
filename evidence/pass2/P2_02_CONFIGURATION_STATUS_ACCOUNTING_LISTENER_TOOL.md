# Pass 2.02 — Configuration Status Accounting & Listener Decision Tool

status: NEAR PODCAST READY SUPPORT TOOL
created_on: 2026-08-11
companion: P2_02_CONFIGURATION_CHANGE_CONTROL.md; P2_02_SENTINEL_EFFECTIVITY_CUTIN_WORKED_EXAMPLE.md

## Purpose
Turn configuration management from document-control language into a practical production question:

> For any unit, lot, build, or release, can we prove what definition applied, what was actually built, what exceptions existed, what evidence supported acceptance, and what changed afterward?

This tool is Hardware-to-Production synthesis grounded in NASA configuration-management functions, especially configuration identification, change control, configuration status accounting, and verification/audit.

## 1. The five questions a useful CSA system must answer
1. **What is the currently released definition?**
2. **What was the released definition at a historical point/effectivity boundary?**
3. **What was actually built for this serial/lot/work order?**
4. **Which changes, deviations, waivers, discrepancies, or rework affected it?**
5. **What evidence proves that the implemented configuration was accepted?**

If the organization can answer only question 1, it has document control, not sufficient production configuration visibility.

## 2. Compact production configuration object model

### Product Definition
- product/configuration identifier
- revision/baseline
- BOM/drawings/specifications
- PCB/ECAD revision where applicable
- firmware/software release
- approved materials/suppliers
- process/work-instruction versions
- inspection/test/calibration definitions

### Change Object — ECR/ECO/ECN equivalent
- unique change ID
- reason/problem/opportunity
- affected configuration items
- requirement/CTQ impact
- risk and evidence impact
- approvals
- released changes
- effectivity rule
- WIP/inventory disposition
- implementation verification
- closure state

Names differ by company. The important concept is controlled lifecycle and traceable decision state, not the acronym.

### Temporary Exception — Deviation/Waiver equivalent
- unique ID
- requirement/baseline exception
- affected serials/lots/work orders
- rationale and risk acceptance
- compensating controls/tests
- approver
- start/end or explicit expiry
- closure/disposition

Do not universalize sector-specific terminology: organizations may distinguish deviation and waiver differently. NASA guidance itself notes variation in usage while requiring controlled status and traceability.

### Effectivity Object
- change/configuration ID
- effectivity type: serial / lot / work order / date / other controlled boundary
- first affected unit or range
- inventory/WIP rule
- transition-lot rule
- supersession/expiry if applicable

### As-Built / Genealogy Record
- unit/lot identity
- product revision/baseline
- critical component identities/lots as required
- firmware/software version or build identity
- process/test/calibration versions where needed
- deviations/waivers
- rework/repair history
- acceptance result

## 3. Hardware + firmware co-configuration rule
A hardware product with firmware should not be represented as if hardware revision alone defines the product state.

For every accepted unit, define and retain the allowed/actual combination of:
- hardware revision;
- firmware/software revision/build;
- calibration/configuration data version when product behavior depends on it;
- relevant programmable-device image where applicable.

### Sentinel example
Rev C hardware may support both VS-A and VS-B, but the allowed combinations are controlled:

| Hardware | Sensor | Firmware | Status |
|---|---|---|---|
| Rev B | VS-A | 1.8.2 | released legacy |
| Rev B | VS-B | 1.8.2 | prohibited / unsupported |
| Rev C | VS-A | 1.9.0 | released if qualification covers it |
| Rev C | VS-B | 1.9.0 | released normal production |
| transition unit | VS-B | 1.9.0-rc2 | only under DEV-011 scope |

The lesson is not the exact table. The lesson is that product identity may be a valid combination of configuration items, not one revision label.

## 4. Configuration Status Accounting example — Sentinel Node

For SN-0286 the status-accounting view should reconstruct:
- nominal/current product baseline at query time;
- baseline/effectivity applicable when the unit was built;
- PCB revision actually installed;
- VS-B supplier and lot;
- FW 1.9.0-rc2;
- DEV-011 authorization;
- CAL/FTP versions used;
- enhanced verification results;
- any rework;
- final disposition/acceptance;
- whether later ECO closure converted, retained, or excluded this transition evidence.

This is stronger than asking, “What is the current BOM?”

## 5. Listener decision tool — Is this change controlled enough?

### Gate A — Identify
- Can I name exactly what changed?
- Which configuration items are affected?
- Is the old state reconstructable?

If no: stop. The change is not sufficiently identified.

### Gate B — Impact
- Which requirements, CTQs, interfaces, safety/reliability assumptions, manufacturing controls, supplier controls, software behaviors, tests, or service procedures can change?
- Which existing evidence depended on the old state?

If unknown: perform impact assessment before release.

### Gate C — Evidence
Classify prior evidence:
1. unaffected — transfers;
2. transfers with documented engineering rationale;
3. targeted regression/reverification required;
4. broader qualification assessment required.

Never choose the class solely because parts look interchangeable.

### Gate D — Release
- Have all affected definitions been revised/released coherently?
- Are hardware, firmware, process, inspection, calibration, supplier and service objects synchronized where applicable?

If not: do not create a split-brain production definition.

### Gate E — Effectivity
- What exact serial/lot/work-order boundary applies?
- What happens to WIP?
- What happens to existing stock?
- Are transition units explicitly controlled?

A release date alone is usually insufficient for mixed/WIP production.

### Gate F — Genealogy
For an affected unit, can we later prove what was actually installed/run/tested?

If no: the organization cannot reliably investigate field failures or prove historical configuration.

### Gate G — Verify implementation
- Were first cut-in units checked?
- Was production actually using the intended released package?
- Were deviations closed/expired correctly?
- Were discrepancies resolved?

Document approval is not implementation verification.

## 6. Change closure definition
A change is not considered operationally closed merely because the ECO status says APPROVED.

A robust closure check asks whether:
- required evidence is complete;
- affected documents/data are released;
- effectivity is implemented;
- WIP/inventory is dispositioned;
- first affected production is verified;
- genealogy captures the new state;
- temporary exceptions are closed or explicitly retained;
- open discrepancies are resolved or accepted;
- downstream/service impact is communicated where required.

## 7. Podcast myths to break
- “The latest BOM tells me what every unit contains.” — False.
- “Rev C was released Monday, so Tuesday production is Rev C.” — Not necessarily.
- “Same footprint means equivalent component.” — False as a general rule.
- “Approved ECO means implemented change.” — False.
- “Firmware is separate from manufacturing configuration.” — Often dangerously false for behavior-defining products.
- “A deviation is just permission to build it differently.” — Incomplete; scope, risk, evidence, effectivity, genealogy and expiry matter.

## 8. Evidence/applicability notes
NASA systems-engineering guidance defines configuration management across the product life cycle and identifies five functions including status accounting and verification/audit. NASA describes CSA as recording/reporting configuration data and calls for current and historical configuration documentation, identifiers, status of changes/deviations/waivers, and discrepancy/audit status.

The exact ECR/ECO/ECN workflow, database schema, serial-effectivity convention, and deviation terminology in this file are not claimed as NASA-mandated forms. They are Hardware-to-Production implementation patterns derived from the underlying CM objectives.

## 9. P2.02 readiness gate
P2.02 can move to NEAR PODCAST READY when:
- formal CM terminology/source evidence is packaged;
- Sentinel cut-in example is complete;
- CSA/listener tool is complete;
- hardware/firmware co-configuration is represented;
- sector-specific terminology is marked as non-universal;
- final technical/editorial review remains as the principal open gate.

Current assessment after this tool: **NEAR PODCAST READY**.