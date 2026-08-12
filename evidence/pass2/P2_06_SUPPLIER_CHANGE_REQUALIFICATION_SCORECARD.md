# P2.06 — Supplier Change, Requalification & Engineering-Risk Scorecard

Status: DEPTH ACTIVE
Provenance: mixed verified-source synthesis + worked example

## Purpose
A supplier that was approved yesterday is not automatically approved for every future process, material, sub-tier, tool, site, cavity, inspection method, software or rate change. This pack defines a practical notification-to-requalification workflow and a scorecard that prevents delivery and price metrics from hiding engineering risk.

## Canonical rule
Supplier approval is valid inside the demonstrated and approved process/configuration envelope. A meaningful change requires impact assessment before evidence is reused.

## Supplier Change Notification workflow
1. Supplier identifies proposed change before implementation.
2. Classify change: product/material; process; tooling/cavity; site; sub-tier; equipment; inspection/test; packaging; software/recipe; capacity/rate; ownership/QMS where relevant.
3. Identify affected requirements and CTQs.
4. Identify prior evidence being relied upon: FAI, PPAP/PPA-like package, qualification, capability, MSA, validation, environmental/reliability tests, packaging tests, rate evidence.
5. Ask which assumptions behind that evidence changed.
6. Assign requalification scope proportionate to risk.
7. Approve, reject or conditionally approve the proposed change before production cut-in where contract/QMS requires prior approval.
8. Define effectivity: date, lot, serial, PO/work order, tool/cavity or other traceable boundary.
9. Disposition WIP and inventory made before/during transition.
10. Verify first production after cut-in and update supplier status accounting.

## Requalification Decision Tree
### Gate A — Did the approved envelope change?
If no: document rationale and continue monitoring.
If yes or uncertain: proceed.

### Gate B — Can the change affect fit, form, function, reliability, safety, compliance, manufacturability, CTQ distribution, traceability or capacity?
If yes: engineering/quality impact review required.

### Gate C — What evidence is potentially invalidated?
Map each affected claim to the evidence that supported it. Do not automatically repeat every test; do not automatically reuse every old result.

### Gate D — Select evidence response
Possible responses include document review, dimensional FAI, material verification, MSA confirmation, short capability study, process validation, functional regression, environmental/reliability retest, packaging/logistics validation, production-rate run, sub-tier audit, or full/partial production approval resubmission.

### Gate E — Define cut-in and containment
Record effectivity and any temporary incoming inspection, source inspection, tightened sampling, segregation, first-lot hold or enhanced traceability.

### Gate F — Verify effectiveness
Confirm post-change quality and process behavior before removing containment.

## Sentinel Node worked example — hidden sub-tier change
Supplier Alpha molds the production-intent enclosure. Six months after approval, Alpha changes the gasket-material sub-tier to improve lead time. Nominal material family and drawing dimensions appear unchanged, so Purchasing initially treats the change as commercial.

Engineering impact review identifies possible effects on compression set, sealing performance, chemical/environmental resistance and assembly compression window. The old enclosure dimensional FAI remains useful for unchanged geometry, but it does not by itself prove the new gasket source preserves sealing/reliability behavior.

Required response in the example:
- supplier change record before cut-in;
- material/certificate review and identity verification;
- comparison of critical material properties;
- targeted sealing/environmental reverification based on affected assumptions;
- defined lot effectivity;
- temporary enhanced incoming/functional controls;
- genealogy linking finished Sentinel serials to gasket lot/source;
- effectiveness review after representative production exposure.

The lesson is not that every sub-tier change requires full qualification. The lesson is that requalification scope follows affected claims and invalidated assumptions.

## Six-month Supplier Alpha scorecard
Illustrative values only.

| Month | OTD | Incoming PPM | Escape events | FPY at supplier | SCN discipline | Traceability | Engineering risk |
|---|---:|---:|---:|---:|---|---|---|
| M1 | 98% | 900 | 0 | 94% | Green | Amber | Amber |
| M2 | 100% | 500 | 0 | 96% | Green | Green | Green |
| M3 | 99% | 350 | 0 | 97% | Green | Green | Green |
| M4 | 100% | 300 | 1 | 97% | Red — unapproved sub-tier change discovered | Amber | Red |
| M5 | 99% | 250 | 0 | 98% | Amber — corrective controls active | Green | Amber |
| M6 | 100% | 180 | 0 | 98% | Green | Green | Green |

This deliberately shows why a supplier can look excellent on OTD and aggregate defect metrics while still becoming RED engineering risk. An unauthorized change can invalidate qualification assumptions even before a large PPM signal appears.

## Supplier scorecard architecture
Do not collapse everything into one weighted number without retaining hard-stop dimensions.

### Delivery & commercial
- OTD / schedule adherence
- lead-time stability
- expedite frequency
- price/TCO trend

### Quality
- incoming defects/PPM where appropriate
- supplier FPY
- customer/line escapes
- repeat defects
- corrective-action closure and effectiveness

### Process evidence
- CTQ stability/capability where statistically justified
- measurement-system adequacy
- tool/cavity/process-window control
- production-rate evidence

### Change discipline
- notification before change
- approval compliance
- effectivity clarity
- sub-tier change control
- deviation discipline

### Traceability
- material/lot/tool/cavity linkage appropriate to risk
- ability to contain affected population
- record completeness

### Resilience
- capacity headroom
- alternate tooling/site/source readiness
- recovery time
- single points of failure

## Hard-stop logic
A supplier should not remain Green solely because a weighted average is high when any critical condition is Red. Example hard stops:
- unauthorized product/process/sub-tier change affecting approved evidence;
- inability to identify affected lots after a critical escape;
- known measurement system incapable of supporting acceptance decisions;
- repeated critical escapes without effective containment/corrective action;
- demonstrated inability to meet required production rate for a critical part.

## Listener tool — CHANGE 9
Before accepting a supplier change, ask:
1. What changed?
2. Why is it changing?
3. Which requirement/CTQ can it affect?
4. Which old evidence are we relying on?
5. Which assumptions behind that evidence changed?
6. What minimum reverification closes the risk?
7. Where exactly is the cut-in/effectivity boundary?
8. Can we trace and contain the affected population?
9. What evidence will let us remove temporary containment?

## Evidence guardrails
- PPAP/PPA/FAI terminology and mandatory triggers are industry/customer specific; this framework does not claim universal applicability.
- Supplier scorecard thresholds are company/product/risk specific. The illustrative numbers above are not normative acceptance limits.
- A supplier change does not automatically require full requalification. Scope should follow impact, risk and the evidence assumptions affected.
- Good delivery and low aggregate defect rates do not prove configuration/change discipline.

## Source anchors
- NIST MEP supply-chain guidance supports supplier evaluation, supplier development, risk assessment and use of supplier metrics/scorecards.
- NIST MEP supplier-selection guidance emphasizes quality-system documentation, inspection evidence, rejection handling and lot control/traceability, not merely receipt of a good sample.
- AIAG PPAP is an automotive production-approval framework; use it only where contract/customer/industry applicability exists. Its concepts are useful as an example of production-intent evidence and controlled change, not as a universal mandate.

## Podcast-ready messages
1. A supplier is not a part number; it is a production system.
2. Approval is bounded by the process/configuration envelope that generated the evidence.
3. Supplier change control is configuration management across an organizational boundary.
4. The correct question after a supplier change is not “Do we repeat qualification?” but “Which claims lost support?”
5. OTD can be green while engineering risk is red.
6. Traceability matters most when you need to define the affected population quickly.
