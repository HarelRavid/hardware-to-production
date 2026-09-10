# Episode 56 Production Blueprint — Lessons from Automotive Manufacturing

status: PRODUCTION BLUEPRINT COMPLETE
season: Season 6 — Manufacturing Atlas: Decision Playbooks and Case Studies
primary_audience: hardware/NPI/manufacturing/quality/supplier teams outside and inside automotive
lifecycle: LVP → SVP, with DEV transfer guidance
maps_to: MASTER_WBS 10.4 + quality/supplier/evidence synthesis
source_basis: `EP56_CASE_EVIDENCE_PACK.md`
entry_point: YES WITH QUALITY-CHAIN RECAP
technical_depth: practitioner

## Listener transformation
Before: sees automotive quality as a stack of acronyms — APQP, PPAP, FMEA, SPC, MSA — and either copies the paperwork or rejects it as bureaucracy.
After: understands the connected evidence problem those methods address and can transfer the mechanism while preserving customer, certification, volume and industry-specific applicability.

## Narrative hook
A 2025 RAV4 recall potentially involved only four U.S. vehicles, yet the investigation could trace the risk through supplier tier, production period, welding line, jig interference, robot damage and shared tip-dressing equipment.

The opening question is:

> What kind of manufacturing system lets you reconstruct a four-vehicle problem that deeply?

## Teaching flow
1. RAV4 seat-bracket weld case: reconstruct shim → robot damage → shared tip dresser → second weld path → potentially affected population.
2. Extract genealogy beyond VIN/serial: supplier tier, line, tooling/equipment, time/effectivity and process state.
3. Introduce AIAG Core Tools only after the case, as connected methods around planning, risk, control, measurement, process behavior and production approval.
4. Chevrolet Bolt: two manufacturing defects in the same cell as an interaction condition, followed by supplier manufacturing/QA changes.
5. Connect INTERACTION CLAIM, supplier evidence envelope and change/requalification logic.
6. Explain PPAP/APQP carefully as automotive/customer-context methods, not universal manufacturing law.
7. Explain current IATF 16949 revision-status discipline: publication/current-status claims must be checked at script time.
8. Close with the rule: borrow the evidence chain, not the paperwork burden.

## Core framework — Automotive Practice Transfer Matrix
`Method → problem controlled → evidence object → customer/standard requirement? → volume assumption → supplier-network assumption → consequence/risk assumption → DEV need → LVP need → SVP/customer requirement → transferable core → non-transferable overhead`.

Internal synthesis only; it does not redefine AIAG methods.

## Case spine
### Case 1 — Toyota RAV4 seat-bracket weld recall
Owns: process genealogy, shared-equipment interaction, supplier-tier investigation and population scoping.
Guardrail: potentially involved vehicles are not equivalent to confirmed defective units; preserve Toyota/NHTSA report wording.

### Case 2 — Chevrolet Bolt battery
Owns: interacting supplier manufacturing defects and process/QA change after field evidence.
Guardrail: torn-anode/folded-separator root-cause wording is GM-attributed in the cited NHTSA-hosted communication.

### Method context — AIAG Core Tools / IATF
Owns: connected automotive quality/planning context and current-publication discipline.
Guardrail: exact PPAP/APQP/IATF requirements depend on current manuals, customer-specific requirements and scope.

## Listener tool — Quality Chain Transfer Check
For an automotive method ask:
`What failure/decision is this method controlling? → what evidence object does it create? → what upstream/downstream object must link to it? → is it required here or merely useful? → what lighter DEV/LVP implementation preserves the mechanism? → what changes at contractual SVP?`.

## DEV / LVP / SVP
DEV: use lightweight risk/control/measurement thinking without pretending to run a serial automotive approval system.
LVP: connect process risks, controls, measurement adequacy, supplier changes and genealogy; keep approval proportional to real risk/customer needs.
SVP: where customer/industry contracts require formal Core Tools/PPAP/IATF processes, apply the current exact requirements and preserve evidence of the demonstrated production envelope.

## Prototype shortcut / expiration
Shortcut: informal supplier/process approval based on samples and engineering familiarity.
Expires when: product release depends on repeatable supplier/process capability across lots, lines, equipment, tooling or changes that the sample evidence did not cover.

## Common mistakes
- treating an approved supplier name as permanent evidence;
- maintaining PFMEA/Control Plan/MSA/SPC as disconnected documents;
- assuming traceability means only product serial/VIN;
- inferring defect rate from a recall portal field without reading its definition;
- claiming a specific Core Tool would necessarily have prevented a case;
- copying automotive submission overhead into low-risk DEV/LVP without customer/risk justification.

## Source / script gates
Before script lock:
- verify current AIAG manual editions and any exact claims used;
- recheck IATF 16949 2nd Edition/publication transition status;
- source any customer-specific PPAP requirement if narrated;
- preserve GM attribution for Bolt root-cause language;
- preserve Toyota potentially-affected vs confirmed-defect wording.

## Season handoff
EP56 shows a mature industry's connected production-evidence machinery. EP57 moves to medical devices, where rework, packaging, field remediation and jurisdiction-specific QMS obligations make another principle visible: a corrective action creates a new evidence state rather than erasing the old one.
