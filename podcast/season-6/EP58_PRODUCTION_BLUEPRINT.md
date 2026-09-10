# Episode 58 Production Blueprint — Lessons from Aerospace Manufacturing

status: PRODUCTION BLUEPRINT COMPLETE
season: Season 6 — Manufacturing Atlas: Decision Playbooks and Case Studies
primary_audience: hardware/NPI/quality/reliability/supplier teams learning from aerospace evidence discipline
lifecycle: LVP → SVP → FIELD / long-life operation
maps_to: MASTER_WBS 10.6 + configuration/supplier/reliability synthesis
source_basis: `EP58_CASE_EVIDENCE_PACK.md`
entry_point: YES WITH CONFIGURATION + EVIDENCE-ENVELOPE RECAP
technical_depth: advanced practitioner

## Listener transformation
Before: treats aerospace discipline as exhaustive documentation, FAI and certification that either should be copied wholesale or dismissed as excessive.
After: understands what the evidence burden is trying to protect — exact configuration, supplier/process state, rework closure, inspection capability and lifecycle reliability — and can transfer those mechanisms proportionately without claiming aerospace methods are universal.

## Narrative hook
The Boeing 787 battery had acceptance and first-article evidence, and supplier audits existed. Yet the later NTSB investigation found manufacturing features and inspection/control gaps that those approvals had not been designed to expose.

The opening question is:

> What does an approval actually prove — and what can remain completely outside its field of view?

## Teaching flow
1. 787 battery: approval/audit evidence existed; NTSB later identified winding perturbations, FOD/control concerns and CT-inspection limitations.
2. Establish evidence-envelope rule: conformance/FAI/audit proves only what the verification system actually covers.
3. Distinguish first-article verification from ongoing process understanding/capability and from lifetime reliability evidence.
4. Alaska 737-9 door plug: rework/removal created an incomplete configuration state; missing documentation prevented the expected closure/QA path.
5. Reinforce canonical rule: rework = new configuration state requiring ownership, record and re-verification.
6. Introduce IAQG 9102 as an actual aerospace FAI method with its explicit applicability caveat; do not equate it automatically with AS9100 obligations.
7. PW4077 fan blade: as-manufactured geometry/contamination can become a fatigue-life variable years later; lifecycle inspection interpretation becomes another evidence layer.
8. Close with three transferable aerospace habits: configuration identity, mechanism-aware verification and disciplined evidence after change/rework.

## Core framework — Aerospace Evidence Transfer Check
`Aerospace practice → exact claim protected → configuration/process dependency → supplier/flowdown dependency → verification method/capability → change/rework trigger → lifecycle consequence → contractual/regulatory context → transferable mechanism → assurance burden that should NOT be copied automatically`.

Internal synthesis only.

## Case spine
### Case 1 — Boeing 787 APU battery / GS Yuasa
Owns: bounded approval evidence, supplier/subtier process understanding and inspection capability.
Guardrail: do not reduce the incident to one manufacturing feature or claim FAI/audits were absent; the lesson is that they did not cover every consequential mechanism.

### Case 2 — Alaska Airlines 737-9 door plug
Owns: rework state, documentation-triggered verification and release closure.
Guardrail: avoid operator-blame framing and avoid generalizing NTSB aviation recommendations directly into non-aviation requirements.

### Case 3 — PW4077 fan blade
Owns: manufacturing-created state → long-term reliability → inspection interpretation.
Guardrail: preserve NTSB/P&W attribution and keep numerical stress/life estimates case-specific.

### Method context — IAQG 9102 FAI
Owns: configuration-specific first-article verification concept.
Guardrail: 9102 may be contractual/self-imposed and is not automatically required merely because another aerospace standard is used.

## Listener tool — Approval Boundary Sheet
For any FAI/audit/qualification/certificate ask:
`What exact configuration was reviewed? → which characteristics/process steps were observed? → what inspection capability was assumed? → what latent mechanisms were outside scope? → what supplier/subtier evidence was relied upon? → what change invalidates the approval? → what ongoing evidence is needed after first article?`.

## DEV / LVP / SVP / FIELD
DEV: do not imitate aerospace documentation volume; do preserve configuration, test purpose and critical process assumptions.
LVP: first production/change evidence should prove the defined article/process while process risks and measurement capability are developed explicitly.
SVP: supplier/subtier control, rework closure, ongoing process evidence and change effectivity become scalable systems; approval cannot become a permanent badge.
FIELD: manufacturing state can affect long-life reliability, so field inspection/maintenance evidence may need to reconnect to original process/configuration populations.

## Prototype shortcut / expiration
Shortcut: first-article/sample conformance may be enough to decide whether to continue development.
Expires when: the claim becomes “this process/supplier/configuration can repeatedly produce and sustain the required result” without representative ongoing evidence.

## Common mistakes
- equating FAI with process capability;
- equating completed audit with mechanism understanding;
- assuming low reject rate means a process is safe when the inspection cannot see the relevant feature;
- treating rework as invisible once assembly is closed;
- copying aerospace paperwork burden into low-risk hardware without consequence/contract justification;
- overclaiming causal mechanisms from factual investigation reports.

## Source / script gates
Before script lock:
- preserve exact NTSB locators for 787/737-9/PW4077 findings;
- source any formal 9102 requirement/edition statement from current IAQG material;
- independently verify any numerical PW4077 estimate if narrated and retain P&W attribution;
- conduct aerospace applicability review for FAI/supplier/special-process language;
- maintain distinction among conformance, process capability and reliability evidence.

## Season handoff
EP58 shows how evidence must survive configuration, rework and long life. EP59 takes the same logic into industrial equipment, where machines may remain installed for decades while controllers, software, spares, safety expectations and retrofit configurations change around them.
