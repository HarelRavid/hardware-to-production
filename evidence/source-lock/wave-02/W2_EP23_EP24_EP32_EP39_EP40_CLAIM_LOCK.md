# Wave 02 Claim Lock — EP23 / EP24 / EP32 / EP39 / EP40

status: CLAIM-LEVEL EVIDENCE LOCK COMPLETE FOR CURRENT GENERIC SCRIPT SCOPE
checked: 2026-09-19
shared_register: `../SOURCE_LOCK_WAVE_02_QUALITY_SUPPLIER_REGISTER.md`

## Status vocabulary

- `VERIFIED OPEN SOURCE` — directly supported by open authoritative/public source.
- `VERIFIED + V6 SYNTHESIS` — source supports the premise; wording/framework remains ours.
- `PUBLIC METHOD CONTEXT ONLY` — official industry-body page supports identity/high-level purpose, not protected details.
- `LICENSED MANUAL GATE` — exact method step/field/threshold/submission rule cannot be narrated authoritatively until current licensed text is reviewed.
- `CUSTOMER/SECTOR GATE` — obligation depends on customer/contract/jurisdiction/sector.
- `V6 LOCKED AS SYNTHESIS` — current generic script may use it as our engineering guidance without external attribution.

# EP23 — DFMEA, PFMEA, Control Plans and Quality Gates

## EP23-C01
Claim: product/design risk and manufacturing/process risk are related but distinct engineering perspectives.
Lock: `PUBLIC METHOD CONTEXT ONLY + V6 SYNTHESIS`.
Sources: W2-S01, W2-S02, W2-S03.
Rule: exact AIAG/VDA DFMEA/PFMEA structure remains `LICENSED MANUAL GATE`.

## EP23-C02
Claim: process-risk analysis is useful when failure modes/causes are connected to prevention/detection controls and production execution.
Lock: `VERIFIED + V6 SYNTHESIS`.
Sources: W2-S01, W2-S03.
Boundary: do not quote AIAG/VDA steps or forms without licensed text.

## EP23-C03
Claim: a Control Plan is a structured manufacturing-control artifact linked to product-quality/process planning.
Lock: `PUBLIC METHOD CONTEXT ONLY`.
Source: W2-S03.
Boundary: exact fields/phases/Safe Launch requirements remain `LICENSED MANUAL GATE`.

## EP23-C04
Claim: detection is not the same as preventing the mechanism that creates the defect.
Lock: `V6 LOCKED AS SYNTHESIS`.
No claim that AIAG mandates a universal prevention hierarchy.

## EP23-C05
Claim: measurement adequacy should be understood before inspection/test data support strong process conclusions.
Lock: `VERIFIED OPEN SOURCE`.
Sources: W2-S07, W2-S09.

## EP23-C06
Claim: control intensity should follow consequence/risk/process dependence rather than applying equal rigor to every characteristic.
Lock: `V6 LOCKED AS SYNTHESIS`.
No universal CTQ taxonomy claimed.

## EP23-C07
Claim: a quality gate needs an explicit reaction for affected process/product/WIP; a check with no response logic is weak control.
Lock: `V6 LOCKED AS SYNTHESIS`.
Source-informed by the quality-chain model; exact AIAG reaction-plan fields remain manual-gated.

## EP23-C08
Claim: RPN/Action Priority or any one scoring number must not replace engineering judgment.
Lock: `LICENSED MANUAL GATE + V6 GUARDRAIL`.
Rule: no exact RPN/AP method teaching until the current FMEA handbook is reviewed.

### EP23 gate
Current generic script can teach the Risk-to-Control Chain without reproducing proprietary Core Tool details.
Unresolved P0: exact AIAG/VDA method claims only.

---

# EP24 — Production Testing and Measurement-System Capability

## EP24-C01
Claim: the production measurement system includes more than the instrument; method, operator, fixture, conditions and time can affect results.
Lock: `VERIFIED OPEN SOURCE`.
Sources: W2-S07, W2-S08, W2-S09.

## EP24-C02
Claim: repeatability and reproducibility answer different measurement questions.
Lock: `VERIFIED OPEN SOURCE`.
Source: W2-S08.

## EP24-C03
Claim: calibration status alone does not establish total measurement-system adequacy for a production decision.
Lock: `VERIFIED OPEN SOURCE + V6 SYNTHESIS`.
Sources: W2-S07, W2-S09.

## EP24-C04
Claim: measurement adequacy is decision-dependent; a method adequate for coarse screening may be inadequate for a tighter discrimination/capability conclusion.
Lock: `VERIFIED + V6 SYNTHESIS`.
Sources: W2-S07, W2-S09.

## EP24-C05
Claim: measurement/test changes that can alter the decision need controlled effectivity and renewed adequacy assessment where affected.
Lock: `V6 + P2.02 DEPENDENCY`.
Wave 01 configuration/change lock supplies the generic premise.

## EP24-C06
Claim: no universal GR&R percentage threshold applies to every measurement decision.
Lock: `SCRIPT GUARDRAIL`.
AIAG-specific thresholds/interpretation remain `LICENSED MANUAL GATE`.

## EP24-C07
Claim: retest/rework history should not be erased by a final PASS.
Lock: `V6 GLOBAL INVARIANT`.

### EP24 gate
P0 generic measurement claims: 0 unresolved.
Any AIAG MSA-specific design/threshold claim remains gated.

---

# EP32 — Process Capability, SPC and Knowing Whether Production Is Stable

## EP32-C01
Claim: specification limits and statistical control limits answer different questions.
Lock: `VERIFIED OPEN SOURCE`.
Sources: W2-S10 plus NIST/SEMATECH process-monitoring/capability guidance.

## EP32-C02
Claim: a process can be statistically stable yet not capable relative to specifications.
Lock: `VERIFIED OPEN SOURCE`.
Source: W2-S10.

## EP32-C03
Claim: temporary conformance to specification does not by itself prove statistical stability.
Lock: `VERIFIED + V6 SYNTHESIS`.
NIST process-control/capability framework supports the distinction.

## EP32-C04
Claim: capability interpretation assumes a credible representation of process behavior and depends on model/data assumptions.
Lock: `VERIFIED OPEN SOURCE`.
Source: W2-S10.

## EP32-C05
Claim: Cp and Cpk answer related but different questions; Cpk accounts for off-centering relative to specification limits.
Lock: `VERIFIED OPEN SOURCE`.
Source: NIST process-capability page in W2-S10.
Formula lock:
- Cp = (USL-LSL)/(6s)
- Cpk = min[(USL-xbar)/(3s), (xbar-LSL)/(3s)]

## EP32-C06
Claim: no universal Cpk threshold should be taught without customer/sector/context applicability.
Lock: `SCRIPT GUARDRAIL`.

## EP32-C07
Claim: measurement adequacy precedes strong capability interpretation.
Lock: `VERIFIED OPEN SOURCE`.
Sources: W2-S07, W2-S09, W2-S10.

## EP32-C08
Claim: the 2026 AIAG/VDA SPC manual is current automotive method context, not the generic authority for all hardware manufacturing.
Lock: `PUBLIC METHOD CONTEXT ONLY`.
Source: W2-S04.

### EP32 numerical lock
Sentinel worked example independently checked:
- centered mean 5.00 mm, sigma 0.04 mm, LSL 4.80, USL 5.20 → Cp=Cpk≈1.67.
- shifted mean 5.10 mm with same sigma/limits → Cp≈1.67, Cpk≈0.83.
Status: `ARITHMETIC VERIFIED — ILLUSTRATIVE DATA`.

---

# EP39 — RFQ Technical Package and Approving First Production

## EP39-C01
Claim: a technically useful RFQ must communicate enough configuration/requirement/process/evidence context that suppliers are quoting the same problem.
Lock: `V6 LOCKED AS SYNTHESIS`.
NIST supplier-evaluation/TCO guidance supports broader supplier-selection context; exact RFQ content is our listener framework.

## EP39-C02
Claim: first-production evidence should be representative of the source/process/configuration being approved.
Lock: `VERIFIED + V6 SYNTHESIS`.
Sources: W2-S05, W2-S12.

## EP39-C03
Claim: FAI and PPAP are not synonyms.
Lock: `VERIFIED CROSS-SOURCE SYNTHESIS`.
Sources: W2-S05, W2-S12.
Boundary:
- 9102 FAI = aerospace/contract applicability;
- PPAP = automotive/customer-specific applicability.

## EP39-C04
Claim: a conforming first article does not by itself establish sustained process capability at required rate.
Lock: `VERIFIED CROSS-SOURCE SYNTHESIS`.
Sources: W2-S10, W2-S12.

## EP39-C05
Claim: exact PPAP submission levels, evidence package contents and resubmission triggers are not universal.
Lock: `LICENSED MANUAL GATE + CUSTOMER/SECTOR GATE`.

## EP39-C06
Claim: approval authority and open deviations should remain explicit rather than being hidden inside supplier correspondence.
Lock: `V6 LOCKED AS SYNTHESIS`.

### EP39 gate
Generic first-production-approval episode can proceed.
Detailed PPAP/9102 requirement narration remains gated to exact source/applicability.

---

# EP40 — Supplier Quality, Dual Sourcing and Resilience

## EP40-C01
Claim: supplier performance should be monitored across meaningful dimensions such as quality, delivery, responsiveness and development/continuity concerns rather than reduced to quote price.
Lock: `VERIFIED + V6 SYNTHESIS`.
Source: W2-S11.

## EP40-C02
Claim: supplier metrics/scorecards can support performance management.
Lock: `VERIFIED OPEN SOURCE`.
Source: W2-S11.

## EP40-C03
Claim: an approved supplier name is not permanent evidence independent of site/process/material/tooling/sub-tier/configuration state.
Lock: `V6 GLOBAL INVARIANT + METHOD CONTEXT`.
Sources: W2-S05, W2-S12, Wave 01 P2.02.

## EP40-C04
Claim: a supplier/process/material/site/sub-tier change can require impact assessment and new evidence where it touches the demonstrated approval envelope.
Lock: `VERIFIED PREMISE + V6 SYNTHESIS`.
Exact notification/reapproval obligation: `CUSTOMER/SECTOR GATE`.

## EP40-C05
Claim: two supplier names do not equal two qualified production sources.
Lock: `V6 LOCKED AS SYNTHESIS`.
Alternate-source readiness must be evaluated against current configuration/process/evidence.

## EP40-C06
Claim: incoming inspection is not a universal substitute for source-process control.
Lock: `V6 LOCKED AS SYNTHESIS`.
Any sector-specific incoming-acceptance rule is separately gated.

## EP40-C07
Claim: total cost of ownership and supplier segmentation are legitimate supplier-management considerations.
Lock: `VERIFIED OPEN SOURCE`.
Source: W2-S11.

## EP40-C08
Claim: a blended supplier score must not override a safety/regulatory/critical-quality hard stop.
Lock: `V6 GLOBAL HARD-STOP SYNTHESIS`.

### EP40 gate
Generic supplier-quality/resilience narrative can proceed.
Exact contractual flow-down/change-notification/dual-source requalification rules remain gated.

---

# Cross-wave dependencies

Wave 01 supplies:
- configuration/effectivity/change-impact discipline;
- evidence tied to exact configuration;
- targeted re-verification logic.

Wave 02 owns:
- risk/control/measurement/stability/capability chain;
- supplier first-production approval evidence;
- sustained supplier quality/resilience.

Do not duplicate Wave 01 configuration theory in EP39/EP40.

# Decision

**WAVE 02 CLAIM LOCK: PASS FOR INTERNAL TECHNICAL REVIEW**

Remaining unresolved items are explicit licensed-manual/customer-specific gates, not hidden generic-script blockers.
