# Season 4 S4-A Internal Technical Review — EP33 / EP34 / EP35 / EP36

status: PASS TO FINAL SCRIPT OUTLINE
review_date: 2026-09-19
review_type: internal technical / applicability / source-currentness review
human_independent_review: NOT CLAIMED

inputs:
- SOURCE_LOCK_SEASON_4_S4A_QUALITY_RELIABILITY_TRACEABILITY_COMPLIANCE_REGISTER.md
- S4A_EP33–EP36 claim locks
- EP33–EP36 Production Blueprints
- Waves 01/02/05
- Season 1 EP10
- Season 3 quality/ramp packages

## 1. EP33 — Nonconformance / MRB / CAPA

Result: PASS.

Core ownership:
Detection → containment → affected population → disposition → cause → corrective action → effectiveness.

Required guards:
1. do not define universal MRB authority;
2. do not say every defect requires CAPA;
3. do not treat rework/retest as corrective action;
4. do not prescribe one root-cause tool;
5. preserve original failure/rework history;
6. effectiveness must be population/evidence based.

Claude dialogue opportunity:
Speaker B should ask:
“If the unit is fixed and passes, why isn’t the problem closed?”

## 2. EP34 — Reliability Validation / Field Evidence

Result: PASS.

Core ownership:
reliability claim + production variation + field exposure + population evidence.

Required guards:
1. no universal MTBF/life target;
2. no universal sample size/confidence threshold;
3. accelerated testing remains failure-mechanism/model dependent;
4. field anecdotes require configuration/exposure segmentation;
5. zero failures ≠ proof;
6. burn-in/screening only with mechanism/economic rationale.

Claude dialogue opportunity:
qualification passed, then one supplier lot fails only in hot/humid market.

## 3. EP35 — Genealogy / Traceability / Affected Population

Result: PASS.

Core ownership:
physical product genealogy and affected-population reconstruction.

Required guards:
1. serial number ≠ full genealogy;
2. no universal retention period;
3. no maximal-data-by-default mindset;
4. current master data does not reconstruct historical truth;
5. rework/deviation history remains visible;
6. one centralized database is not required.

Boundary with Season 5:
EP35 owns what physical production history must be reconstructable.
Season 5 EP48 owns the digital architecture for implementing linked genealogy.

## 4. EP36 — Standards / Applicability / Compliance

Result: PASS WITH CURRENT-EDITION CORRECTION.

Critical current correction:
- ISO 9001:2026 is now current; ISO 9001:2015 is withdrawn.
- ISO 9000:2026 is now current; ISO 9000:2015 is withdrawn.

Required guards:
1. standard ≠ law;
2. certification ≠ universal product compliance;
3. regulation/customer/contract/standard/guidance authority classes remain distinct;
4. no protected clause teaching from public metadata;
5. FDA QMSR is U.S. medical-device scope only;
6. no legal advice;
7. current edition/status must be checked at final script freeze if materially named.

Claude dialogue opportunity:
team says “we’re ISO compliant”; B asks “which ISO, which edition, which market, which requirement, and what evidence?”

## 5. Cross-episode boundary

EP33:
failure handling and corrective learning.

EP34:
reliability over time/exposure/populations.

EP35:
genealogy needed to identify affected populations.

EP36:
authority/applicability of external/internal requirements.

EP32 remains owner of SPC/process capability.
EP39/40 remain supplier approval/ongoing supplier quality.

Result:
PASS — no structural overlap repair needed.

## 6. Standards/source currentness

Verified 2026-09-19:
- ISO 9000:2026 current.
- ISO 9001:2026 current.
- ISO 10007:2017 current, revision project underway.
- NIST IR 8536 final 2026-09-09.
- NIST reliability handbook remains current reference source.
- FDA QMSR effective 2026-02-02.

## 7. Decision

EP33: PASS TO FINAL SCRIPT OUTLINE.
EP34: PASS TO FINAL SCRIPT OUTLINE.
EP35: PASS TO FINAL SCRIPT OUTLINE.
EP36: PASS TO FINAL SCRIPT OUTLINE.

**SEASON 4 S4-A TECHNICAL REVIEW: PASS**
