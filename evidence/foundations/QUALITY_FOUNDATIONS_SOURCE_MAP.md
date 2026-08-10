# Quality Foundations — PFMEA, Control Plan, MSA, SPC & Capability — Evidence Source Map

status: BREADTH COMPLETE
campaign: A4
maps_to: MASTER_WBS 4.7, 4.8, 4.9, 6.1–6.4; PODCAST_MAP Episodes 23–24, 32
provenance: primary-source-first

## Purpose
Build the evidence backbone for the quality system that connects product/process risk to controls, measurement adequacy, statistical stability, capability and reaction.

## Authoritative source backbone

### AIAG / Automotive Core Tools
Evidence role:
- APQP, PFMEA, Control Plan, MSA, SPC and PPAP are intended as linked quality-planning/control tools in automotive contexts;
- AIAG training/material explicitly links Process Flow, PFMEA and Control Plan and teaches using APQP/FMEA information to construct Control Plans;
- current Control Plan material includes prototype, pre-launch/safe-launch and production contexts.

Key sources:
- AIAG & VDA Process FMEA: Understanding and Implementing with Control Plans
- AIAG Control Plan manual / Control Plan Understanding and Implementing
- AIAG Core Tools Support material showing explicit relational links among Process Flow, PFMEA and Control Plan

Applicability boundary: automotive Core Tools are not universal legal requirements for all hardware sectors. Podcast use should extract engineering logic and identify sector-specific obligations separately.

### NIST / SEMATECH statistical engineering
Evidence role:
- process control/stability is distinct from capability/conformance;
- control limits are derived from process behavior and are not engineering specification limits;
- capability analysis compares a stable process distribution with specification limits and requires data/model assumptions.

### NIST Gauge R&R / measurement-system references
Evidence role:
- production gauges can require characterization of repeatability, reproducibility, stability, bias, resolution, linearity, hysteresis, drift and configuration/operator effects;
- measurement adequacy is broader than calibration status.

### ASQ SPC references
Evidence role:
- control charts are diagnostic tools used to detect common/special-cause variation and support process-control decisions;
- reaction should be based on the nature of process variation rather than indiscriminate adjustment.

## Canonical quality chain
Requirement / CTQ -> failure mechanism / risk -> prevention/detection control -> measurement method -> measurement-system adequacy -> data collection -> stability assessment -> capability assessment -> reaction plan / quality gate -> learning into PFMEA/Control Plan.

This sequence is editorial synthesis, not a single standard requirement.

## PFMEA -> Control Plan logic
PFMEA identifies process failure modes, effects, causes and current/preventive/detection controls. The Control Plan operationalizes selected controls into production characteristics, control/measurement methods, sample/frequency and reaction expectations.

### C-QF-001 — PFMEA and Control Plan should be linked rather than treated as independent paperwork
status: STRONG FOR AUTOMOTIVE CORE-TOOLS CONTEXT / STRONG TRANSFERABLE LOGIC
Evidence basis: AIAG material explicitly teaches Process FMEA and Control Plan linkages and construction of Control Plans using APQP/FMEA outputs.
Podcast use: Episode 23.

### C-QF-002 — Risk analysis is useful only if important risks change design/process controls, validation or monitoring
status: STRONG SYNTHESIS
Boundary: scoring/ranking methods are methodology-specific; do not turn RPN or Action Priority into universal engineering truth.

## MSA boundary
A measurement system should be evaluated in relation to the decision it supports.

### C-QF-003 — Calibration alone does not prove a measurement system is adequate for a production decision
status: STRONG
Evidence basis: NIST Gauge R&R explicitly evaluates repeatability, reproducibility, stability, bias, resolution, linearity, hysteresis, drift and configuration effects.
Podcast use: Episode 24.

### C-QF-004 — Measurement-system adequacy should be understood before interpreting small process differences or capability indices
status: STRONG DIRECTION
Evidence basis: observed variation can include both process and measurement effects; direct quantitative acceptability thresholds depend on method/industry/decision.

## SPC and capability
### C-QF-005 — Control limits and specification limits answer different questions
status: STRONG
Control limits characterize expected process behavior under the charting model; specifications come from product/engineering requirements.
Podcast use: Episode 32.

### C-QF-006 — Stable does not mean capable
status: STRONG
A process can be statistically stable and still fail to meet specifications adequately.

### C-QF-007 — In-spec observations do not prove statistical control
status: STRONG
An unstable process may temporarily produce conforming product while special-cause variation remains present.

### C-QF-008 — Capability indices require assumptions, suitable data and meaningful measurement
status: STRONG
Do not present Cp/Cpk as universal truth from tiny, nonrepresentative or unstable datasets.

## Sampling, 100% inspection and reaction plans
### Inspection boundary
Inspection strategy depends on defect mechanism, detectability, measurement capability, cost, risk, process stability and whether inspection itself can introduce error/damage.

### C-QF-009 — 100% inspection is not automatically equivalent to 100% defect containment
status: STRONG ENGINEERING DIRECTION / quantitative Pass-2 depth open
Reason: measurement systems have false-accept/false-reject risk and coverage limitations; operator/equipment effects may remain.

### C-QF-010 — Sampling is a decision/risk tool, not a substitute for process control
status: STRONG SYNTHESIS
Sampling can support lot acceptance or monitoring, but it does not create a stable/capable process.

### Reaction-plan principle
A control or monitoring method is incomplete without a defined response to abnormal conditions.

Reaction plan should define as applicable:
- trigger/signal;
- immediate containment/hold boundary;
- response owner;
- stop/escalate/adjust rules;
- disposition of potentially affected product;
- verification after correction;
- PFMEA/Control Plan/update feedback when learning changes risk/control assumptions.

### C-QF-011 — Reaction plans should distinguish special-cause investigation from routine process adjustment
status: STRONG DIRECTION
Evidence basis: SPC sources distinguish common and special causes; indiscriminate adjustment can add variation.

## DEV / LVP / SVP lens
### DEV
Use lightweight risk tracking and characterize measurement limitations. Focus on learning failure mechanisms and avoid fake statistical confidence from tiny/nonrepresentative samples.

### LVP
Introduce structured PFMEA/control planning, controlled inspection/test, fit-for-purpose MSA, defect/FPY tracking and basic SPC where repeated data supports it. Use explicit containment/reaction even if the process remains manual.

### SVP
Use qualified measurement systems, stable data definitions, SPC/capability appropriate to the process, reaction plans, traceable quality gates and closed-loop NCR/CAPA. Sector-specific Core Tools requirements may apply.

## Myth register
- "Inside spec means the process is in control" — FALSE.
- "Inside control limits means the product is good" — FALSE.
- "A calibrated gauge is an adequate measurement system" — FALSE.
- "Cp/Cpk tells the whole story" — FALSE.
- "100% inspection means zero escapes" — FALSE AS UNIVERSAL CLAIM.
- "PFMEA is complete when the spreadsheet is approved" — FALSE AS ENGINEERING PRACTICE; value depends on controls/learning linkage.
- "Sampling fixes an unstable process" — FALSE.
- "Gauge R&R is the only valid MSA method" — FALSE AS UNIVERSAL CLAIM.

## Breadth result
Source families represented:
- PFMEA/Control Plan linkage — YES
- MSA/Gauge R&R — YES
- SPC/common-special cause — YES
- stability versus capability — YES
- sampling/100% inspection boundary — DEFINED with Pass-2 quantitative depth open
- reaction-plan logic — YES
- applicability conflicts — YES

## Pass-2 targets
- worked PFMEA -> Control Plan example;
- Gauge R&R / measurement-system example;
- control-chart example showing common versus special cause and a reaction decision;
- capability example with explicit assumptions and measurement caveat;
- quantitative false-accept/false-reject / guard-banding example;
- sampling-plan example with acceptance-risk interpretation;
- case where 100% inspection still allowed escapes;
- sector applicability comparison: general manufacturing vs automotive/medical/aerospace.

## Readiness
Source map: BREADTH COMPLETE
Critical claims identified: YES
Primary-source backbone: YES
Applicability conflicts visible: YES
Quantitative depth: OPEN for Pass 2
Podcast Ready: NO