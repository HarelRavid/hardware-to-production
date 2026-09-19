# Wave 02 Internal Technical Review — EP23 / EP24 / EP32 / EP39 / EP40

status: PASS TO SCRIPT OUTLINE WITH CONTROLLED MANUAL/APPLICABILITY GATES
review_date: 2026-09-19
review_type: internal technical consistency + source-boundary review
human_independent_review: NOT CLAIMED

inputs:
- WAVE_02_MANIFEST.md
- SOURCE_LOCK_WAVE_02_QUALITY_SUPPLIER_REGISTER.md
- W2_EP23_EP24_EP32_EP39_EP40_CLAIM_LOCK.md
- P2.03 Quality Chain artifacts
- P2.06 Supplier Industrialization artifacts
- canonical Production Blueprints
- Wave 01 configuration/change source lock
- frozen Knowledge Backbone V1 invariants

## 1. Review purpose

Test whether the selected episodes can advance to script outlining without:
- reproducing protected Core Tool content;
- presenting automotive/aerospace methods as universal requirements;
- teaching misleading statistical shortcuts;
- confusing conformance, stability and capability;
- confusing first article, production approval and sustained capability;
- turning supplier scoring into a substitute for technical hard stops.

# 2. EP23 — Risk to Control

Result: PASS WITH SCRIPT GUARDRAILS.

Strengths:
1. The episode owns a clear engineering question: how risk becomes prevention/detection/reaction in production.
2. It correctly avoids making FMEA scoring the engineering objective.
3. It hands measurement adequacy to EP24 and sustained process statistics to EP32.
4. The Risk-to-Control Chain is useful synthesis and does not require proprietary forms.

Required guards:

### EP23-G01 — DFMEA/PFMEA terms
It is safe to state that design-focused and process-focused FMEA methods address different perspectives.
Do not teach the exact AIAG/VDA seven-step method, Action Priority logic, RPN treatment or form structure without licensed review.

### EP23-G02 — Control Plan
Say that AIAG's current standalone Control Plan is linked to APQP/product-quality planning and manufacturing-control definition.
Do not narrate exact mandatory fields/phases or Safe Launch requirements as universal.

### EP23-G03 — prevention/detection
Teach the engineering distinction without implying that every detected risk must be physically prevented.

### EP23-G04 — quality gates
A gate is only meaningful if ownership/reaction/affected-product logic is clear.
Keep exact sampling/frequency rules context-specific.

Decision: advance to script outline.

# 3. EP24 — Measurement System Capability

Result: PASS.

Strengths:
1. NIST provides strong open support for repeatability, reproducibility, stability and measurement-process characterization.
2. The episode correctly separates instrument calibration from full decision adequacy.
3. It avoids universal GR&R thresholds.
4. It preserves retest/rework history and configuration dependency from Wave 01.

Required guards:

### EP24-G01 — calibration wording
Do not say calibration is unimportant. Say it is necessary in many contexts but does not alone characterize all measurement-system behavior relevant to a production decision.

### EP24-G02 — repeatability/reproducibility
Use NIST terminology carefully. Reproducibility requires stating which conditions changed.

### EP24-G03 — golden/reference units
A reference/golden unit may be a controlled check artifact, but it is not automatically a calibration standard or traceability chain.

### EP24-G04 — guard bands/false accept-reject
Keep conceptual unless a metrology/decision-rule source is separately locked.

### EP24-G05 — GR&R
No universal percentage thresholds.

Decision: advance to script outline.

# 4. EP32 — SPC and Capability

Result: PASS WITH STATISTICAL GUARDRAILS.

Strengths:
1. NIST directly supports stability-before-capability reasoning and Cp/Cpk formulas.
2. The Sentinel arithmetic is correct.
3. The episode distinguishes specification limits from control limits.
4. It does not use Cpk as a universal process-health score.

Required guards:

### EP32-G01 — normality/sample assumptions
Capability indices require assumptions. NIST notes normality assumptions for common Cp/Cpk interpretation and sample-size considerations.
Do not imply the formulas are universally valid for any data distribution or sampling scheme.

### EP32-G02 — control chart rules
Do not teach a universal set of Western Electric/AIAG/VDA signal rules without locking the chosen method.
The episode can teach the concept of detecting departures from established process behavior.

### EP32-G03 — illustrative UCL/LCL
The Sentinel `5.00 ± 3×0.03` limits are illustrative teaching values, not a universal chart-construction recipe.

### EP32-G04 — thresholds
Do not say `Cpk 1.33 = capable` generically.
Any customer/sector threshold must be sourced and scoped.

### EP32-G05 — stable vs conforming
A stable process can produce nonconforming output.
An unstable process can temporarily produce all conforming output.
Preserve both directions.

Decision: advance to script outline.

# 5. EP39 — RFQ / First Production Approval

Result: PASS WITH INDUSTRY-METHOD GUARDRAILS.

Strengths:
1. The episode's main value is technical completeness/ambiguity reduction in supplier transfer.
2. It correctly treats FAI and PPAP as different evidence packages.
3. It can teach first-production approval generically without prescribing a universal package.
4. Wave 01 supplies configuration/effectivity discipline.

Required guards:

### EP39-G01 — FAI scope
Use IAQG 9102 as aviation/space/defense FAI context and note it can be adopted elsewhere.
Do not imply AS9100 universally requires 9102 or that every hardware supplier must perform aerospace FAI.

### EP39-G02 — PPAP scope
Use AIAG's public PPAP description only at high level.
Do not teach submission levels, required elements or resubmission triggers without licensed/current/customer-specific source.

### EP39-G03 — first article vs capability
A conforming first article is evidence about a defined configuration/process result.
It is not by itself proof of sustained process capability or rate.

### EP39-G04 — certificates
A certificate is useful only if its relationship to the actual requirement/product/process is defined; avoid blanket statements that certificates are weak/useless.

Decision: advance to script outline.

# 6. EP40 — Supplier Quality / Dual Sourcing / Resilience

Result: PASS WITH CONTRACT/APPLICABILITY GUARDRAILS.

Strengths:
1. NIST MEP supports supplier evaluation, TCO, metrics/scorecards and supplier development.
2. The episode correctly treats alternate-source readiness as an evidence problem, not a vendor-count problem.
3. It preserves supplier/process change as a configuration/evidence transition.
4. It does not elevate one supplier score above hard safety/quality stops.

Required guards:

### EP40-G01 — scorecards
Supplier metrics support management; do not imply a specific weighting formula is authoritative.

### EP40-G02 — incoming inspection
Do not say incoming inspection is always inferior or unnecessary. Say it is one control and does not automatically replace evidence about source-process capability when that matters.

### EP40-G03 — change notification
Exact supplier change-notification obligations are contractual/customer/sector specific.
Generic script: consequential changes should trigger defined notification/impact review according to the applicable agreement/system.

### EP40-G04 — dual sourcing
Two qualified sources may legitimately use different processes/material routes if both satisfy the needed claims. Do not require identical process architecture; require controlled equivalence/independent evidence where relevant.

### EP40-G05 — resilience
Resilience includes more than geography or having a second supplier: tooling, material, sub-tier, capacity, data and requalification lead time may be common-mode dependencies.

Decision: advance to script outline.

# 7. Cross-episode boundary review

EP23 vs EP24:
- EP23 owns what needs control.
- EP24 owns whether measurement/test can support the control decision.
PASS.

EP24 vs EP32:
- EP24 owns measurement-system trust.
- EP32 owns time-ordered process behavior and capability interpretation.
PASS.

EP23 vs EP32:
- EP23 may introduce reaction logic.
- EP32 owns statistical signals/capability.
PASS.

EP39 vs EP40:
- EP39 owns technical RFQ and initial/first-production approval.
- EP40 owns sustained supplier performance/change/resilience.
PASS.

EP39/40 vs EP56 automotive:
- EP56 applies automotive examples.
- EP39/40 own generic supplier evidence architecture.
PASS.

# 8. Global invariant check

Claim/evidence/applicability envelope — PASS.
Change invalidation is impact-based — PASS.
Definition/as-built/evidence distinction — PASS.
Rework history preserved — PASS.
Measurement adequacy before capability — PASS.
Approval bounded by demonstrated envelope — PASS.
Hard stops not overridden by weighted score — PASS.

No backbone change required.

# 9. Script-entry decision

EP23: `PASS TO SCRIPT OUTLINE — LICENSED FMEA/CP DETAILS EXCLUDED`.
EP24: `PASS TO SCRIPT OUTLINE`.
EP32: `PASS TO SCRIPT OUTLINE — STATISTICAL METHOD/THRESHOLD GUARDS`.
EP39: `PASS TO SCRIPT OUTLINE — FAI/PPAP DETAILS SCOPED`.
EP40: `PASS TO SCRIPT OUTLINE — CUSTOMER/CONTRACT RULES SCOPED`.

**WAVE 02 INTERNAL TECHNICAL REVIEW: PASS**
