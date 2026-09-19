# Wave 03 Internal Technical Review — EP26 / EP27 / EP28 / EP29 / EP30 / EP31

status: PASS TO SCRIPT OUTLINE WITH CONTROLLED CUSTOMER/FINANCE GATES
review_date: 2026-09-19
review_type: internal technical consistency + source-boundary + quantitative review
human_independent_review: NOT CLAIMED

inputs:
- SOURCE_LOCK_WAVE_03_RAMP_ECONOMICS_REGISTER.md
- W3_EP26_EP27_EP28_EP29_EP30_EP31_CLAIM_LOCK.md
- P2.04 capacity/ramp artifacts
- P2.05 economics artifacts
- EP26–31 Production Blueprints
- Wave 01 configuration/change lock
- Wave 02 quality/supplier lock
- frozen Knowledge Backbone V1 invariants

## 1. Review purpose

Test whether the six ramp-family episodes can advance to script outlining without:
- turning NASA PRR into a universal production gate;
- pretending PVT/Run-at-Rate have one universal definition;
- confusing batch completion, rate and sustainable capacity;
- teaching takt/cycle/throughput/capacity as synonyms;
- hiding rework inside final yield;
- overstating queue/WIP formulas;
- turning financial examples into universal investment thresholds;
- duplicating supplier/change material already owned by Waves 01–02.

# 2. EP26 — Pilot Build Planning

Result: PASS WITH SCRIPT GUARDRAILS.

Strengths:
1. Correctly treats pilot as a designed evidence event.
2. Quantity is subordinate to learning/decision objective.
3. Configuration/effectivity and intervention visibility are integrated.
4. Exit decision includes carryover gaps instead of binary pass/fail mythology.

Guards:
### EP26-G01 — pilot quantity
Never imply 25, 30, 100 or another count is generically sufficient. Quantity depends on the claims and risks being investigated.

### EP26-G02 — stop rules
Teach stop/containment logic as risk-based planning. Do not invent universal defect-count stop criteria.

### EP26-G03 — NASA
NASA PRR may support production-readiness categories but does not define the podcast's Pilot Build Plan.

### EP26-G04 — shipped pilot units
Do not imply pilot units can never ship. The issue is whether shipment interferes with learning/containment and whether released status is explicit.

Decision: PASS TO OUTLINE.

# 3. EP27 — Production Validation

Result: PASS WITH REPRESENTATIVENESS GUARDRAILS.

Strengths:
1. Separates product verification from production-system evidence.
2. Treats intervention/workarounds as limitations on the claim.
3. Keeps rate evidence bounded to what was actually exercised.
4. Supports constrained-release/repeat/proceed decisions without inventing universal gates.

Guards:
### EP27-G01 — validation terminology
Do not imply the phrase “production validation” has one standards-defined meaning across sectors.

### EP27-G02 — configuration freeze
Prefer “bound/control the configuration being evaluated” rather than absolute design freeze; controlled changes may occur if effectivity and evidence remain clear.

### EP27-G03 — engineering intervention
Intervention does not automatically invalidate the build. It changes the evidence: record what required rescue and what normal production can/cannot yet do.

### EP27-G04 — rate extrapolation
Do not extrapolate sustainable capacity from a short ideal run.

Decision: PASS TO OUTLINE.

# 4. EP28 — Yield / Rework / Scrap

Result: PASS WITH TERMINOLOGY GUARDRAILS.

Strengths:
1. Separates first-pass success from eventual recovery.
2. Keeps rework history visible.
3. Links rework to capacity/economic burden.
4. Focuses on recurrence/effectiveness rather than cosmetic final yield.

Guards:
### EP28-G01 — FPY vs final yield
Define episode terminology explicitly because organizations use yield terms differently. Avoid claiming one naming convention is universal.

### EP28-G02 — RTY
Do not introduce rolled throughput yield formulas unless the episode genuinely needs them and a source/formula package is locked.

### EP28-G03 — rework vs repair
Local/company definitions may differ. Teach the semantic difference needed for the example, not a universal legal taxonomy.

### EP28-G04 — learning curve
Do not state a generic percentage learning rate. Improvement must be tied to observed process/design changes.

Decision: PASS TO OUTLINE.

# 5. EP29 — Capacity / Bottlenecks / Takt

Result: PASS WITH QUANTITATIVE GUARDRAILS.

Strengths:
1. Takt and cycle time are correctly separated.
2. Accepted throughput remains the system boundary metric.
3. WIP/queue growth is used as a flow-balance signal, not a goal.
4. Rework burden at the constraint is explicit.
5. All current arithmetic has been independently checked.

Guards:
### EP29-G01 — takt denominator
State the time basis explicitly. Planned production time choices differ by organization; the example's 420 minutes is illustrative.

### EP29-G02 — bottleneck
The longest nominal cycle can be a candidate constraint, not automatically the full system constraint under variability, shared labor, failures and mix.

### EP29-G03 — Little's Law
Use only for stable/appropriate average-flow relationships. Do not imply it predicts transient queue dynamics by itself.

### EP29-G04 — queue-growth arithmetic
The 2.43 units/hour result is a deliberately simplified arrival-minus-service illustration before rework/stochastic variability. Label it exactly that way.

### EP29-G05 — run duration
No universal run-at-rate duration.

### EP29-G06 — capacity vs demand
A line can have capacity above demand and still have delivery problems from scheduling/material/quality; do not equate capacity margin with total operational health.

Decision: PASS TO OUTLINE.

# 6. EP30 — Supplier Readiness / CM Management

Result: PASS WITH DEPENDENCY DISCIPLINE.

Strengths:
1. Reuses Wave 02 instead of reinventing FAI/PPAP/supplier approval.
2. Adds ramp-specific capacity and ownership questions.
3. Correctly separates quoted/theoretical capacity from demonstrated supplier system capacity.

Guards:
### EP30-G01 — supplier capacity
Do not accept machine nameplate capacity as source capacity without material/staffing/yield/downtime/mix assumptions.

### EP30-G02 — CM ownership
Contract manufacturer responsibility matrices are organization/contract specific. The episode can require explicit ownership without prescribing a universal RACI.

### EP30-G03 — qualification standards
No universal ISO 9001/IATF/AS9100/PPAP requirement.

### EP30-G04 — incoming inspection
Preserve Wave 02 nuance: useful control, not automatic substitute for source-process evidence.

Decision: PASS TO OUTLINE.

# 7. EP31 — Engineering Changes During Ramp

Result: PASS WITH CHANGE-BOUNDARY GUARDRAILS.

Strengths:
1. Correctly treats change as a production transition, not a document-only event.
2. WIP/inventory/supplier/test/tooling impacts are explicit.
3. Re-verification remains dependency-based.
4. Post-cut-in effectiveness ties change to ramp evidence.

Guards:
### EP31-G01 — ECO/ECN
Use as common practitioner labels, not universal standardized workflows.

### EP31-G02 — effectivity
Date can be valid when it uniquely controls implementation; do not claim date-based effectivity is always inadequate. The lesson is to select a boundary that reconstructs the population.

### EP31-G03 — emergency change
Emergency deviations may be necessary. The issue is explicit scope/expiry/closure, not “never change quickly.”

### EP31-G04 — customer/regulatory notification
Remain application specific.

Decision: PASS TO OUTLINE.

# 8. P2.05 Economics review

Result: PASS AS SHARED DEPENDENCY.

Technical findings:
- break-even arithmetic: PASS.
- simple payback arithmetic: PASS.
- support allocation arithmetic: PASS.
- yield-conversion arithmetic: PASS.
- five-year launched-unit arithmetic: PASS.
- NPV formula concept: PASS against NIST source family.

Guards:
### ECON-G01 — 10% rate
Illustrative only; not a recommended hurdle/discount rate.

### ECON-G02 — simple payback
Useful screening metric; not full investment analysis.

### ECON-G03 — capacity feasibility first
Do not compare five-year economics as if an alternative can serve demand beyond its stated practical capacity without an added capacity step.

### ECON-G04 — taxes/depreciation/working capital
The teaching model intentionally omits some real accounting/cash-flow details; explicitly say real decisions require project-specific finance treatment.

### ECON-G05 — uncertainty
Sensitivity analysis exposes importance of assumptions; it does not make unsupported assumptions accurate.

# 9. Cross-episode boundary review

EP26 vs EP27:
EP26 owns experiment planning; EP27 owns integrated readiness evidence. PASS.

EP27 vs EP29:
EP27 asks what rate evidence belongs in validation; EP29 owns the detailed flow/capacity math. PASS.

EP28 vs EP32:
EP28 owns production learning from failure/rework; EP32 owns statistical process stability/capability. PASS.

EP29 vs EP42:
EP29 owns capacity evidence; later automation business-case episode owns investment decision. P2.05 can be previewed but not re-teach EP42. PASS.

EP30 vs EP39/40:
EP30 owns supplier readiness specifically during ramp/CM execution; EP39/40 own approval and sustained supplier-quality architecture. PASS.

EP31 vs A8/P2.02:
EP31 applies existing change-control logic under ramp/WIP/supplier conditions. PASS.

# 10. Global invariant check

Accepted sustainable throughput > peak speed: PASS.
Measurement adequacy before capability: inherited/PASS.
Rework adds history: PASS.
Approval bounded by demonstrated envelope: PASS.
Change invalidation impact-based: PASS.
Definition/as-built/evidence separation: PASS.
Moving constraint loop preserved: PASS.

No backbone change required.

# 11. Script-entry decision

EP26: PASS TO SCRIPT OUTLINE.
EP27: PASS TO SCRIPT OUTLINE.
EP28: PASS TO SCRIPT OUTLINE.
EP29: PASS TO SCRIPT OUTLINE — quantitative guards embedded.
EP30: PASS TO SCRIPT OUTLINE — Wave 02 dependencies retained.
EP31: PASS TO SCRIPT OUTLINE — Wave 01 dependencies retained.

WAVE 03 INTERNAL TECHNICAL REVIEW: PASS.
