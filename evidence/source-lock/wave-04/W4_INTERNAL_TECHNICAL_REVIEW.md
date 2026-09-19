# Wave 04 Internal Technical Review — EP41 / EP42 / EP43 / EP44 / EP45 / EP46

status: PASS TO SCRIPT OUTLINE WITH CONTROLLED SAFETY/STANDARD GATES
review_date: 2026-09-19
review_type: internal technical consistency + source-boundary + quantitative review
human_independent_review: NOT CLAIMED

inputs:
- SOURCE_LOCK_WAVE_04_AUTOMATION_SAFETY_OEE_REGISTER.md
- W4_EP41_EP42_EP43_EP44_EP45_EP46_CLAIM_LOCK.md
- P2.07 worked examples / release gate / OEE loss tree
- EP41–46 Production Blueprints
- Waves 01–03 source-lock packages
- frozen Knowledge Backbone V1 invariants

## 1. Review purpose

Test whether the automation arc can advance to scripts without:
- presenting automation as a maturity badge;
- turning robot/cobot labels into safety conclusions;
- universalizing machinery standards or legal obligations;
- treating FAT/SAT as full production qualification;
- confusing OEE with root cause or system capacity;
- duplicating Wave 02 automated-measurement fundamentals;
- duplicating Wave 03 economics/capacity ownership;
- implying predictive maintenance is always superior;
- assuming replicated cells are automatically equivalent.

# 2. EP41 — When Not to Automate

Result: PASS WITH SCRIPT GUARDRAILS.

Strengths:
1. Correctly starts from manufacturing problem/mechanism.
2. Reuses process stability, measurement and constraint evidence from earlier waves.
3. Preserves manual/fixture/semi-auto alternatives.
4. Includes safety/recovery/maintenance as readiness inputs.

Guards:
### EP41-G01 — unstable process language
Do not say automation always worsens unstable processes. Say automation can encode/amplify unresolved mechanisms and reduce flexibility/recovery if the process is not understood.

### EP41-G02 — operator judgment
Do not romanticize manual work. Tacit operator adjustment can be valuable evidence that variation is not yet modeled; it can also be a source of variation.

### EP41-G03 — robot repeatability
Repeatability alone is not process capability, but it can be a useful system characteristic when the rest of the process/measurement architecture is sound.

### EP41-G04 — safety
Do not make exact safety standard/legal claims here. Keep to the readiness hard stop: unresolved hazard/recovery architecture blocks automation release.

Decision: PASS TO OUTLINE.

# 3. EP42 — Automation Business Case

Result: PASS WITH ECONOMICS-REUSE GUARDRAILS.

Strengths:
1. Correctly reuses Wave 03 rather than rebuilding economics.
2. Includes do-nothing/staged alternatives.
3. Keeps demand/yield/uptime/change assumptions visible.
4. Treats maintenance/support/integration as lifecycle costs.

Guards:
### EP42-G01 — finance thresholds
No universal hurdle rate, payback or NPV acceptance criterion.

### EP42-G02 — labor savings
Do not assume labor removed from one operation becomes cash savings unless staffing/operating model changes accordingly.

### EP42-G03 — quality benefit
Quality improvement must be evidenced, not assumed from automation.

### EP42-G04 — residual value
Do not assume equipment is redeployable or has residual value without project evidence.

### EP42-G05 — staged CAPEX
Present as option-value strategy under uncertainty, not universally superior investment behavior.

Decision: PASS TO OUTLINE.

# 4. EP43 — Semi-Automation, Robotics and Machine Vision

Result: PASS WITH SAFETY/TECHNOLOGY GUARDRAILS.

Strengths:
1. Function-level decomposition avoids manual-vs-robot false binary.
2. NIST robotics sources support integration/performance/application dependence.
3. ISO 10218 split between robot and application/cell strongly supports the safety boundary.
4. Task-based HRC source supports collaborative-operation context.

Guards:
### EP43-G01 — cobot
Do not say collaborative robot features make an application safe. Application/task risk assessment remains required where applicable.

### EP43-G02 — ISO 10218
Public scope can be stated. Exact safeguards/requirements remain licensed/applicability gated.

### EP43-G03 — vision
Do not teach universal vision false-pass/fail limits or validation sample sizes.

### EP43-G04 — human vs machine
Avoid claims that humans are always better at variability or robots always better at precision. Frame allocation by demonstrated task characteristics.

### EP43-G05 — repeatability vs accuracy
Preserve distinction; neither alone proves product/process capability.

Decision: PASS TO OUTLINE.

# 5. EP44 — Automated Inspection and End-of-Line Test

Result: PASS WITH MEASUREMENT DEPENDENCY GUARDRAILS.

Strengths:
1. Correctly treats automated test as measurement/decision system.
2. Reuses Wave 02 instead of introducing new MSA thresholds.
3. Configuration/effectivity of software/limits is explicit.
4. Retest history/genealogy remain intact.

Guards:
### EP44-G01 — 100% test
100% coverage can reduce escapes for covered detectable failure modes but never implies zero escape probability.

### EP44-G02 — false accept/reject
Keep conceptual unless decision-theory/guard-band statistics are separately sourced.

### EP44-G03 — automated test yield
Do not equate test pass rate with process FPY if the test system itself has faults/false rejects/retest loops.

### EP44-G04 — golden unit
Retain Wave 02 rule: controlled check artifact, not automatically calibration standard.

### EP44-G05 — calibration intervals
No universal interval.

Decision: PASS TO OUTLINE.

# 6. EP45 — Qualification, OEE and Maintenance

Result: PASS WITH CURRENT-STANDARD AND OEE GUARDRAILS.

Strengths:
1. IEC 62381:2024 current scope supports FAT/FIT/SAT/SIT boundary.
2. NIST provides open OEE formula and maintenance context.
3. OEE loss decomposition is strong and arithmetic checked.
4. Recovery/first-good-piece/configuration logic preserves global invariants.

Guards:
### EP45-G01 — FAT/SAT
Do not imply IEC 62381 is universal outside its process-industry scope or that every automation project requires the exact standard.

### EP45-G02 — OEE definitions
Define planned production time, ideal cycle/effectiveness basis and good-output rule before comparison.

### EP45-G03 — OEE benchmark
No 85% “world class” rule.

### EP45-G04 — OEE vs capacity
Local OEE is not system-capacity proof.

### EP45-G05 — maintenance strategy
Predictive, preventive, condition-based and corrective strategies depend on failure modes/economics. Do not declare one universally superior.

### EP45-G06 — recovery
Restart is not full recovery until safe/configuration/quality/genealogy/release state is trustworthy for the claim.

### EP45-G07 — safety standards
Mention standards as applicability map only; no PL/SIL design instruction without qualified safety source/reviewer.

Decision: PASS TO OUTLINE.

# 7. EP46 — Scaling Without Automating Defects

Result: PASS WITH REPLICATION GUARDRAILS.

Strengths:
1. Reuses Wave 02/03 maturity evidence rather than inventing scale criteria.
2. Replication Equivalence Check is useful and source-compatible.
3. Moving-constraint loop preserved.
4. Equipment qualification and recovery are integrated before scale.

Guards:
### EP46-G01 — cloning
Do not imply identical equipment guarantees identical process output.

### EP46-G02 — equivalence
Replication evidence should be characteristic/claim dependent; not every component difference needs full requalification.

### EP46-G03 — scale stop
“Stop expansion” is a risk/evidence decision, not a universal numerical gate.

### EP46-G04 — local automation
Adding a parallel cell can improve throughput if it addresses the actual constraint; do not turn “automation at nonconstraint” into a blanket anti-parallelization rule.

Decision: PASS TO OUTLINE.

# 8. Safety standards current-status review

Current public status captured:
- ISO 12100:2010 current; revision active.
- ISO 13849-1:2023 current.
- ISO 13849-2:2012 current; revision active.
- IEC 62061:2021+A1:2024+A2:2026 current consolidated.
- ISO 10218-1/-2:2025 current.
- IEC 60204-1:2016+A1:2021 current public consolidated family.
- IEC 62381:2024 current.
- ISO 22400-2:2014+Amd1:2017 current published; revision active.

Review decision:
Public scope/current-status use is safe.
Clause-level normative content remains gated.

# 9. Quantitative review

Main Sentinel OEE:
Availability 378/420 = 0.9 — PASS.
Performance (45×470)/22,680 = 0.93253968 — PASS.
Quality 451/470 = 0.95957447 — PASS.
OEE = 0.80535714 ≈80.54% — PASS.

Equal-OEE cells:
0.82×0.99×0.99 = 0.803682 — PASS.
0.99×0.99×0.82 = 0.803682 — PASS.

No numerical safety threshold or OEE benchmark introduced.

# 10. Cross-episode boundary review

EP41 vs EP42:
readiness vs economics — PASS.

EP42 vs EP29:
automation investment vs physical capacity — PASS.

EP43 vs EP41:
function boundary/technology selection vs readiness — PASS.

EP44 vs EP24:
automation application of measurement system vs generic production measurement — PASS.

EP45 vs EP29:
equipment-loss/OEE/maintenance vs system capacity — PASS.

EP45 vs EP52:
physical automation recovery vs OT/data/security recovery — PASS.

EP46 vs EP41/45:
integrated replication gate vs individual automation readiness/qualification — PASS.

# 11. Global invariant check

OEE as loss lens not capacity/root cause — PASS.
Accepted throughput governs system-rate claim — PASS.
Measurement adequacy before automated release conclusions — PASS.
Definition/as-built/evidence separation — PASS.
Change invalidation impact-based — PASS.
Recovery includes configuration/quality/genealogy trust — PASS.
Approval bounded by demonstrated envelope — PASS.

No backbone change required.

# 12. Script-entry decision

EP41: PASS TO SCRIPT OUTLINE.
EP42: PASS TO SCRIPT OUTLINE.
EP43: PASS TO SCRIPT OUTLINE — SAFETY CLAUSE GATES RETAINED.
EP44: PASS TO SCRIPT OUTLINE — WAVE 02 MEASUREMENT DEPENDENCY RETAINED.
EP45: PASS TO SCRIPT OUTLINE — OEE/SAFETY GUARDS EMBEDDED.
EP46: PASS TO SCRIPT OUTLINE.

WAVE 04 INTERNAL TECHNICAL REVIEW: PASS.
