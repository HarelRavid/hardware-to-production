# P2.03 — Canonical Quality Chain Pack

Status: NEAR PODCAST READY

## Purpose
Provide one canonical teaching chain for early hardware teams moving from prototype builds into controlled production:

**Requirement / CTQ → Failure mechanism → PFMEA → Prevention & Detection Controls → Measurement Adequacy → Process Stability → Capability → Reaction → Learning / Update**

This is a synthesis framework. AIAG treats FMEA, Control Plan, MSA and SPC as interconnected Core Tools; NIST provides the statistical foundations used here for measurement and capability interpretation.

## 1. Sentinel Node worked chain

### CTQ
Connector seating depth target: 5.00 mm; specification 4.80–5.20 mm.

### Failure mechanism
Incomplete or inconsistent seating can damage connector pins or create intermittent electrical behavior during final test and field use.

### PFMEA question
Do not begin with an inspection column. Begin with: what can fail, what is the effect, what can cause it, and what prevention/detection controls exist?

Candidate causes include fixture geometry, operator technique, connector tolerance, insertion-force variation, contamination and component damage.

### Control Plan translation
For significant risks, define the controlled characteristic/process parameter, method, frequency or event trigger, measurement/test system, record, owner and reaction.

A Control Plan is therefore an operational response to known process/product risks, not a substitute for the risk analysis.

## 2. Measurement gate
Before interpreting production data, ask whether the measurement system is fit for the intended decision. Calibration alone does not establish repeatability, reproducibility, stability, bias, resolution or other relevant measurement-system behavior.

Listener question: **If two trained operators measure the same part, will the decision remain the same?**

## 3. Stability gate
Specification limits answer whether a product result conforms to an engineering requirement. Control limits describe expected process behavior based on process data. They are not interchangeable.

Therefore an observation may remain inside specification while still providing evidence of a process shift or special cause.

## 4. Capability gate
Capability is assessed only after the measurement and stability questions are credible. For a normal two-sided model:

Cp = (USL − LSL) / 6σ

Cpk = min[(USL − μ)/(3σ), (μ − LSL)/(3σ)]

Sentinel illustration:
- μ = 5.00 mm, σ = 0.040 mm → Cp ≈ 1.67, Cpk ≈ 1.67.
- μ shifts to 5.10 mm with the same σ → Cp remains ≈ 1.67 while Cpk falls to ≈ 0.83.

Teaching point: **potential spread capability and actual centering are different questions.**

NIST notes that capability-index estimates generally need a sufficiently large sample; about 50 independent observations is a common rule of thumb in its handbook, subject to the method's assumptions. Do not convert a 20–30 unit LVP build into false long-term precision.

## 5. LVP evidence discipline
With small builds, report what was actually observed:
- configuration and build conditions;
- units attempted and completed;
- observed conformance by CTQ;
- FPY and rework events;
- defect modes and where detected;
- operator/fixture/tooling dependence;
- ordered measurements where useful;
- changes made during the build;
- unresolved risks.

Do not silently transform these observations into long-term defect rates, mature Cpk claims or sustained-production forecasts.

### LVP Evidence Ladder
0. Anecdote
1. Controlled observation
2. Repeatability evidence
3. Statistical process evidence
4. Sustained production evidence

A pilot build may legitimately advance the team from 0→1 or 1→2 without reaching 3 or 4.

## 6. Reaction architecture
A reaction plan should distinguish at least three signal types.

### A. Product nonconformance
Contain affected product; identify scope; disposition under controlled authority; investigate cause; verify correction; update risk/control documents when learning changes the known process risk.

### B. Statistical process signal while product remains in specification
Do not automatically scrap conforming product. Preserve sequence and context, investigate the special-cause signal, determine affected scope, restore control and document the learning.

### C. Downstream failure pointing upstream
Final-test failure is evidence about the manufacturing system, not merely a final-test event. Trace it back to the likely operation, measurement, material, fixture or handling mechanism; then strengthen prevention/detection at the appropriate point.

## 7. Closed-loop rule
The quality system is incomplete if the chain stops at detection.

**Failure / signal → containment → investigation → corrective learning → PFMEA update → Control Plan update → work instruction/tooling/training/measurement update → effectiveness verification**

This prevents PFMEA and Control Plan from becoming static launch paperwork.

## 8. Listener decision tool — QUALITY CHAIN 8
Before claiming a process is production-ready, answer:
1. What requirement/CTQ are we protecting?
2. What failure mechanism threatens it?
3. What prevents the cause?
4. What detects escape or drift?
5. Can we trust the measurement/test system for this decision?
6. Is the process stable enough to characterize?
7. Is there enough representative data to make the capability claim we are making?
8. What exact reaction occurs when the signal appears, and how does the learning return to the controls?

Any unanswered question is not automatically a launch blocker; it is an explicit evidence gap that must be risk-assessed.

## 9. Podcast guardrails
- Inside spec ≠ process in statistical control.
- In control ≠ capable against specification.
- High Cp ≠ centered process.
- Calibration ≠ adequate measurement system.
- 100% inspection ≠ zero escape risk.
- A small LVP dataset ≠ mature serial capability.
- PFMEA without changed controls is weak risk-management evidence.
- A reaction plan without feedback into risk/control documents loses organizational learning.

## 10. Evidence maturity
This pack is NEAR PODCAST READY. Remaining work before episode lock:
- technical review of formulas/example arithmetic;
- source-note packaging with exact citations/claims;
- editorial mapping to the relevant episodes;
- optional downloadable worksheet formatting.

## Primary evidence anchors
- AIAG Quality Core Tools: FMEA, Control Plan, MSA and SPC are presented as interconnected quality tools.
- NIST/SEMATECH e-Handbook: process capability definitions, assumptions and sample-size caution.
- NIST/SEMATECH measurement-process guidance: measurement-system characterization beyond calibration.

## Provenance note
The QUALITY CHAIN 8, LVP Evidence Ladder, Sentinel Node scenario and reaction architecture are editorial/engineering synthesis frameworks created for this project. They must not be presented as verbatim AIAG or NIST requirements.