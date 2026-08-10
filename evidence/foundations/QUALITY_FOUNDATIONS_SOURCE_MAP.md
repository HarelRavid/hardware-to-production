# Quality Foundations — PFMEA, Control Plan, MSA, SPC & Capability — Evidence Source Map

status: IN PROGRESS — SPC/CAPABILITY/METROLOGY BACKBONE CAPTURED
campaign: A4
maps_to: MASTER_WBS 4.7, 4.8, 4.9, 6.1–6.4; PODCAST_MAP Episodes 23–24, 32
provenance: primary-source-first

## Purpose
Build the evidence backbone for the quality system that connects product/process risk to controls, measurement adequacy, statistical stability and capability.

## Source backbone

### AIAG / Automotive Core Tools
Evidence role:
- APQP relationship to DFMEA/PFMEA, Control Plan, MSA, SPC and PPAP;
- risk-to-control linkage;
- measurement-system and capability expectations in automotive contexts.
Applicability: contractual/industry-specific requirements must not be generalized as universal manufacturing law.
Status: primary mapping still to be deepened.

### ISO 9001 and sector QMS overlays
Evidence role:
- quality planning, control of nonconforming outputs, monitoring/measurement and documented evidence boundaries.
Applicability: management-system requirements are not substitutes for technical process-capability methods.
Status: clause-level mapping reserved for Pass 2.

### NIST/SEMATECH e-Handbook — Process Monitoring and Control
Evidence role:
- explicitly separates process control/stability from process capability;
- capability compares the natural variation of a stable/in-control process with engineering specification limits;
- Cp/Cpk/Cpm require stated assumptions and sufficient data;
- NIST notes common capability-index estimates generally need a sufficiently large independent sample and commonly assume normality for the standard formulas;
- an in-control process can still be unacceptable relative to specifications, which is treated as a distinct problem from an out-of-control process.

Editorial consequence: control limits and specification limits must never be taught as interchangeable concepts.

### NIST/SEMATECH e-Handbook — Measurement Process Characterization
Evidence role:
- measurement is itself a process with bias, short-term variability, long-term variability and uncertainty;
- measurement-process quality requires characterization/control when metrology error matters;
- production-process conclusions can be distorted when measurement error is material.

### NIST — Metrology and Process Control: Dealing with Measurement Uncertainty
Evidence role:
- measurements used to adjust manufacturing processes carry uncertainty;
- uncertainty creates decision risk: good product can be rejected and faulty product can pass;
- measurement uncertainty must be related to tolerance and decision consequence rather than ignored.

### NIST — Measurement Uncertainty
Evidence role:
- measurement results require a defined measurand/reference and carry uncertainty;
- supports the broader principle that measured data is evidence with quality/uncertainty, not perfect truth.

### NIST — Model-Based Manufacturing Capability Definition
Evidence role:
- manufacturing capability is dynamic and decision/context dependent;
- measured/predicted capability should inform lifecycle and manufacturing decisions.
Applicability: this project is broader manufacturing-systems research, not a replacement for Cp/Cpk definitions.

### ISO/IEC 17025 and metrology references
Evidence role:
- calibration/testing competence and traceability boundaries;
- measurement uncertainty and evidence quality where applicable.
Applicability: laboratory accreditation requirements do not automatically apply to every shop-floor measurement activity.
Status: applicability mapping remains open.

## Core conceptual chain
Risk / failure mechanism -> CTQ / requirement -> prevention/control method -> measurement/test method -> measurement adequacy -> process monitoring -> stability assessment -> capability assessment -> reaction plan / quality gate -> NCR/CAPA learning.

The chain is intentionally directional: capability statistics should not be the starting point if the CTQ, measurement method or process state is not understood.

## Claim register

### C-QF-001 — PFMEA and Control Plan should be linked rather than treated as independent paperwork
status: STRONG DIRECTION / PRIMARY MAPPING OPEN
Evidence target: AIAG Core Tools / APQP-Control Plan-FMEA relationships.

### C-QF-002 — Inspection does not substitute for a capable/stable process
status: STRONG ENGINEERING DIRECTION
Evidence basis: NIST distinguishes process monitoring/control, capability and acceptance sampling as different activities. Deeper direct corroboration remains Pass 2.

### C-QF-003 — Measurement-system adequacy must be understood before interpreting process capability or making measurement-driven process decisions
status: STRONG
Evidence basis: NIST measurement-process characterization and metrology/process-control uncertainty work.
Boundary: the required MSA method depends on measurement technology, decision and industry; Gauge R&R is not the only valid measurement-system analysis.

### C-QF-004 — Control limits and specification limits answer different questions
status: STRONG
Evidence basis: NIST control-chart limits derive from process behavior/historical variability; engineering specification limits define acceptable product requirements and are used separately in capability analysis.

### C-QF-005 — A process can be statistically stable yet incapable of meeting specifications
status: STRONG
Evidence basis: NIST explicitly treats the condition 'in control but unacceptable' separately and defines capability as comparison of a stable process to specification limits.

### C-QF-006 — Capability indices are meaningful only under stated assumptions and data conditions
status: STRONG
Evidence basis: NIST capability guidance states standard Cp/Cpk/Cpm estimates require sufficient independent data and standard formulas assume a distribution model such as normality.
Editorial rule: never present a Cp/Cpk value without process state, data basis and relevant assumptions.

### C-QF-007 — Quality controls should be selected from failure/risk mechanisms and CTQs rather than generic inspection habit
status: STRONG SYNTHESIS
Evidence target: PFMEA/Control Plan methodologies and process-specific examples.

### C-QF-008 — Measurement uncertainty can create both false reject and false accept risk
status: STRONG
Evidence basis: NIST metrology/process-control research.

### C-QF-009 — Statistical control is not the same as product conformance
status: STRONG
Evidence basis: NIST separation of process-control and capability/acceptance questions.

### C-QF-010 — A capability statistic calculated from a materially inadequate measurement system can misrepresent the underlying manufacturing process
status: STRONG SYNTHESIS
Evidence basis: NIST measurement error/uncertainty + capability framework. Pass 2 should add worked examples.

## Podcast teaching sequence
1. Start with the requirement/CTQ and failure consequence.
2. Ask what process condition or failure mechanism must be prevented/detected.
3. Define how the characteristic is measured and whether the measurement is adequate for the decision.
4. Separate specification limits from process-derived control limits.
5. Establish whether repeated-process data is stable enough for capability reasoning.
6. Only then calculate/interpret capability where appropriate.
7. Define reaction plan when process or product evidence violates the relevant boundary.

## DEV / LVP / SVP lens
### DEV
Use lightweight risk tracking, characterize measurement limitations, and learn defect mechanisms. Do not fake statistical confidence from tiny or nonrepresentative samples. Verification evidence may be engineering-test oriented rather than SPC oriented.

### LVP
Introduce structured PFMEA/control planning, controlled inspection/test, basic MSA where decisions depend on measurement, defect/FPY tracking and early SPC where repeated data supports it. Low volume may constrain classical capability studies; document the evidence limitation rather than manufacturing a confident index.

### SVP
Use qualified measurement systems, stable sampling/data definitions, capability/SPC appropriate to the process, reaction plans, traceable quality gates and closed-loop NCR/CAPA. Sector/customer requirements may impose additional methods and thresholds.

## Myth register
- 'Inside spec means the process is in control' — REJECT.
- 'Inside control limits means the product meets spec' — REJECT.
- 'Cp/Cpk tells you everything about process quality' — REJECT.
- 'A calibrated gauge is automatically adequate for every manufacturing decision' — REJECT as universal claim; calibration/traceability and decision adequacy are different questions.
- '100% inspection guarantees quality' — OPEN for deeper evidence; reject as simplistic decision rule, but define contexts where 100% screening is justified.
- 'Gauge R&R is the only MSA method' — REJECT as universal claim.

## Breadth gaps to close
1. primary-source mapping of PFMEA -> Control Plan relationship;
2. AIAG/other authoritative MSA terminology and applicability;
3. sampling/inspection boundary and when 100% inspection is/not useful;
4. reaction-plan linkage to SPC/control plans;
5. myths/case studies for Episodes 23, 24 and 32;
6. sector applicability differences: general manufacturing vs automotive/medical/aerospace.

## Pass-2 targets
- worked PFMEA -> control-plan example;
- Gauge R&R / measurement-system example with applicability;
- control-chart example showing common vs special cause;
- capability example with assumptions and measurement caveat;
- case where inspection passed while process remained unstable;
- low-volume example where capability evidence is limited by sample size;
- sector-specific applicability comparison.

## Readiness
Source map: IN PROGRESS — SPC/CAPABILITY/METROLOGY BACKBONE CAPTURED
Critical claims identified: YES
Primary-source backbone: PARTIAL / STRONG FOR STATISTICAL-METROLOGY SIDE
PFMEA/Control Plan primary mapping: OPEN
Applicability conflicts visible: YES
Podcast Ready: NO