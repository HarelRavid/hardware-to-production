# Wave 01 Internal Technical Review — A1 / A7 / A8

status: PASS TO SCRIPT OUTLINE WITH CONTROLLED GUARDRAILS
review_date: 2026-09-10
review_type: internal technical consistency + source-boundary review
human_independent_review: NOT CLAIMED
inputs:
- `W1_SHARED_SOURCE_REGISTER.md`
- `W1_A1_A7_A8_CLAIM_LOCK.md`
- A1/A7/A8 Production Blueprints
- A1/A7/A8 Research Pack claim sets
- P2.02 Configuration & Change Control
- frozen Knowledge Backbone V1 invariants

## 1. Review purpose

Test whether the three foundation episodes can advance from source lock into script outlining without:
- overstating NASA guidance;
- falsely invoking ISO requirements;
- creating contradictory definitions;
- teaching later quality/supplier material too early;
- confusing verification, validation, acceptance and configuration control;
- turning a lightweight startup workflow into aerospace-style bureaucracy.

This review is not represented as an external human professional signoff.

# 2. A1 technical review — Requirements

## Result
PASS WITH SCRIPT GUARDRAILS.

## Strengths
1. The episode correctly distinguishes product intent from an engineering requirement baseline.
2. Functional/performance/interface/environmental/safety-style requirement categories are source-supported at the engineering-guidance level.
3. The `Minimum Useful Requirements` concept is correctly presented as a lightweight internal tool, not a complete formal specification method.
4. `CONFIRMED / TARGET / ASSUMPTION / TBD` is useful editorial synthesis and does not conflict with the sources as long as it is not attributed to ISO/NASA.
5. The episode correctly treats requirement maturity as iterative rather than forcing a complete frozen specification before prototyping.

## Required wording guards
### A1-G01 — do not equate a requirement with a `shall` sentence universally
NASA's formal program guidance uses `shall` statements. The podcast should explain that a well-controlled requirement needs clear, testable meaning; it should not tell every startup that all early requirements must be written in NASA-style `shall` syntax.

### A1-G02 — regulatory watchlist is not compliance determination
The script may say that regulatory/safety/environmental constraints should be identified early because they may alter design choices.
It must not say that a generic checklist determines legal compliance.

### A1-G03 — CTQ remains preview only
Do not teach CTQ selection criteria in A1. Say that some requirements later become production-critical characteristics/controls; defer formal quality-chain treatment.

### A1-G04 — interface failure statement stays qualitative
Avoid claims such as `most hardware failures happen at interfaces` unless separately evidenced. Teach instead that interfaces create cross-discipline dependencies and should be explicit.

## Technical decision
A1 can advance to script outline.

---

# 3. A7 technical review — Verification

## Result
PASS WITH SCRIPT GUARDRAILS.

## Strengths
1. The episode correctly separates `test activity` from `verification evidence`.
2. The verification-chain fields align well with NASA's requirement/version/product/version/procedure/environment/equipment/result records.
3. Claim-specific representativeness is correctly inherited from A4 instead of being redefined.
4. The episode correctly avoids presenting DVT/PVT as universal standards-defined phases.
5. The distinction between exploratory learning and release/qualification evidence is pedagogically useful and safely labeled as synthesis.

## Required wording guards
### A7-G01 — verification vs validation
Use the distinction carefully:
- verification: evidence against specified requirements;
- validation: intended-use/stakeholder expectation question.
Do not use `validation` as a synonym for `more serious testing`.

### A7-G02 — acceptance criteria before data
For a real pass/fail verification decision, acceptance criteria should be defined before interpreting results.
However, exploratory studies may intentionally refine hypotheses/criteria. Do not imply every experiment must have a frozen pass/fail threshold.

### A7-G03 — measurement adequacy remains principle-level
A7 may say that the measurement method must be adequate for the conclusion. Do not introduce universal GR&R percentages, resolution ratios, Cp/Cpk criteria or other numeric quality thresholds here.

### A7-G04 — re-verification scope
Say:
`assess which evidence depends on what changed and reverify accordingly`.
Do not attribute that exact dependency algorithm to NASA or ISO.

### A7-G05 — one passing article
A single passing article can verify some deterministic/configuration-specific requirements, depending on the claim and method. Do not use an absolute statement that `one unit can never verify a requirement`.
The prohibition is against treating one pass as proof of process capability/population behavior without supporting evidence.

## Technical decision
A7 can advance to script outline.

---

# 4. A8 technical review — Configuration

## Result
PASS WITH SCRIPT GUARDRAILS.

## Strengths
1. The episode correctly teaches reconstructability before tooling/software sophistication.
2. The `Definition / As-built-as-programmed / Evidence` separation is a strong canonical synthesis and aligns with the source family's need to preserve product/configuration and verification state.
3. The episode correctly includes firmware, calibration, supplier/material and test-procedure identity when they affect the claim.
4. `Rework adds history` remains technically sound as a traceability principle and is not falsely attributed to a standard.
5. Change impact and effectivity are introduced in a way that supports later NPI/supplier/field lessons.

## Required wording guards
### A8-G01 — configuration management is broader than revision control
Do not collapse CM into file naming/version control. Preserve the distinction among identification, change, status/history and verification.

### A8-G02 — as-built detail is risk-dependent
Do not imply every unit needs every possible lot/tool/process parameter recorded. The minimum genealogy must be chosen based on which attributes affect quality, safety, reliability, service, investigation or release evidence.

### A8-G03 — effectivity terminology
The concept `where/when/which units receive a change` is valid. Until a later formal source lock, keep our `revision vs effectivity` explanation as internal/practitioner terminology rather than an ISO definition claim.

### A8-G04 — rework history
Do not imply every minor touch-up requires an enterprise NCR. Preserve the principle: consequential deviation/rework that can affect the engineering conclusion needs visible history appropriate to the context.

### A8-G05 — supplier equivalence
Do not state that every supplier/lot change requires requalification. Say it requires impact assessment when the source/process/material identity affects a supported claim or controlled requirement.

## Technical decision
A8 can advance to script outline.

---

# 5. Cross-episode boundary review

## A1 vs A7
A1 owns `what must be true / how could we eventually know?`
A7 owns `how to plan and preserve verification evidence`.
PASS — no merge required.

## A7 vs A8
A7 owns evidence intent/execution/use.
A8 owns identity/history/change state that keeps evidence interpretable over time.
PASS — mutually reinforcing, not duplicative.

## A1 vs A8
A1 may introduce controlled requirement changes.
A8 owns detailed configuration/change implementation.
PASS.

## A7/A8 vs P2.03 quality
A7 may preview measurement adequacy.
A8 may preview CTQ/supplier/process dependencies.
Neither should teach MSA/SPC/capability or supplier approval rules.
PASS with guards.

## A8 vs P2.06 supplier change
A8 owns generic configuration impact.
P2.06 owns supplier qualification/reapproval/change obligations and industry-specific methods.
PASS.

# 6. Global-invariant check

1. Claim/evidence/applicability envelope preserved — PASS.
2. Impact-based change invalidation preserved — PASS.
3. Definition / execution / evidence distinction preserved — PASS.
4. Rework history preserved — PASS.
5. Measurement adequacy before capability conclusions — PASS.
6. No rate/OEE misuse introduced — N/A.
7. Approval remains bounded — PASS.
8. No false universal standard applicability — PASS.

# 7. Standards wording audit

Allowed at current script stage:
- `NASA systems-engineering guidance describes...`
- `ISO/IEC/IEEE 29148:2018 is the current published requirements-engineering standard as of this source check...`
- `ISO 10007:2017 is the current published ISO guidance standard for configuration management as of this source check...`

Not allowed without full-text lock:
- `ISO 29148 requires startups to...`
- `ISO 10007 requires every engineering change to...`
- any clause-specific `shall` statement from ISO 29148/10007.

# 8. Review result

Architecture change required: NO.
Claim deletion required: NO.
Claim rewording required before script: YES — controlled wording guards above.
New source family required before script outline: NO.
New source family required before final PODCAST READY: only if the script deliberately introduces a named-standard normative claim outside the locked scope.

Decision:

**WAVE 01 INTERNAL TECHNICAL REVIEW: PASS TO SCRIPT OUTLINE**

Recommended next production action:
Create A1 script architecture first, validate the script/source-note workflow on the series entry episode, then apply the same controlled pattern to A7 and A8 before opening Source-Lock Wave 02.
