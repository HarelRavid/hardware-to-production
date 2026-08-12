# Pass 2.03 — PFMEA → Control Plan → MSA → SPC → Capability Worked Example

status: ACTIVE — PRIMARY QUALITY CHAIN CAPTURED
created_on: 2026-08-12
maps_to: Episodes 23–24, 32; Opening Arc quality/readiness discussions
companion: P2_01_WORKED_EXAMPLE_SENTINEL_NODE.md; QUALITY_FOUNDATIONS_SOURCE_MAP.md

## Purpose
Turn the quality-core-tool stack into one connected manufacturing decision chain using the fictional Sentinel Node. The goal is not to teach automotive paperwork by rote. The goal is to show how a production risk becomes a controlled characteristic, a trustworthy measurement, a monitored process and finally a defensible capability statement.

## Evidence boundary
Authoritative backbone:
- AIAG presents FMEA, Control Plan, MSA and SPC as interconnected Quality Core Tools.
- AIAG Control Plan training explicitly uses information from APQP/FMEA to construct Control Plans.
- NIST Gauge R&R guidance treats the measurement process as a source of repeatability, reproducibility, stability, bias, resolution, linearity, hysteresis and drift effects.
- NIST process-capability guidance compares an in-control/stable process with specification limits.

Hardware-to-Production synthesis:
PFMEA → Control Plan → Measurement adequacy → SPC/stability → Capability → Reaction/learning loop is an editorial/engineering chain, not a claim that every industry mandates these exact documents or sequence.

## Sentinel Node scenario — connector seating damage
During LVP, Sentinel Node experiences approximately 15% final-test failure. Investigation finds that some operators partially side-load the industrial connector during enclosure assembly. The connector can appear seated but individual pins may be displaced or damaged.

Customer/product consequence can include intermittent communication or field failure.

### Step 1 — PFMEA-style risk reasoning
Process step: install/seat connector during final enclosure assembly.

Potential failure mode:
- connector not fully seated;
- pin displaced/damaged;
- excessive insertion load or angular misalignment.

Potential effects:
- intermittent communication;
- failed final test;
- latent field failure.

Potential causes:
- alignment variation;
- fixture freedom;
- operator technique;
- connector dimensional variation;
- excessive insertion force;
- poor visibility of seating condition.

Existing controls before improvement:
- operator visual check;
- final functional test.

Risk insight:
The final functional test detects some failures late but does not prevent connector damage and may not expose every intermittent condition. The risk analysis therefore must drive upstream prevention/detection controls.

## Step 2 — Control Plan translation
The team creates controls around the risk rather than merely adding more final inspection.

| Process point | Characteristic/control objective | Method | Frequency | Reaction concept |
|---|---|---|---|---|
| incoming connector | identity/critical dimensional condition | approved source + defined incoming verification | risk-based/lot-based | quarantine suspect lot |
| assembly fixture | connector alignment | fixture verification | setup/changeover | stop and correct fixture |
| insertion | seating/insertion signature | controlled fixture/force-displacement or bounded process parameter | each unit where implemented | reject/inspect abnormal signature |
| post-assembly | seating confirmation | defined visual/attribute or dimensional criterion | defined frequency / each unit based on risk | contain affected units |
| final test | communication/function | controlled functional test | each unit | contain; trigger upstream investigation |

The exact methods/frequencies are example design choices, not universal AIAG requirements.

## Step 3 — Measurement question before capability
Assume the team chooses connector seating depth as a measurable CTQ.

Engineering requirement for the worked example:
- target seating depth: 5.00 mm
- LSL: 4.80 mm
- USL: 5.20 mm

The team initially measures depth using a handheld depth gauge.

Before treating measured variation as process variation, ask:
- is resolution adequate relative to tolerance/process variation?
- is repeatability acceptable?
- do operators reproduce results?
- does fixture/contact geometry create bias?
- is the method stable over time?
- does the method behave consistently across the measurement range/configurations?

This follows the NIST measurement-process framing: the gauge and measurement method contribute their own variation and error.

## Step 4 — Deliberately misleading capability example
Suppose 50 production measurements from a seemingly stable run produce:
- observed mean = 5.00 mm
- observed standard deviation = 0.040 mm
- LSL = 4.80 mm
- USL = 5.20 mm

Nominal Cp = (USL-LSL)/(6s) = 0.40/(0.24) = 1.67.
Because the mean is centered, nominal Cpk is also approximately 1.67.

A team looking only at the spreadsheet may declare the process excellent.

But now an MSA investigation shows that the handheld measurement contributes substantial variation and operator-dependent contact error. The observed distribution is therefore not a clean representation of the assembly process alone.

Important teaching point:
A capability index calculated from untrustworthy measurement data is numerically precise but epistemically weak. MSA does not merely decorate the capability study; it determines whether the data can support the conclusion.

## Step 5 — Improved measurement system
The team introduces a locating fixture and controlled measurement contact, improves the method definition and repeats measurement-system characterization.

After measurement improvement, the team can distinguish actual process variation from measurement variation more credibly.

The result may move either direction:
- apparent process variation may shrink because measurement noise was removed;
- or the new method may expose real process shifts previously hidden by noisy measurements.

Therefore a better gauge does not guarantee a better Cpk. It gives a more defensible picture of reality.

## Step 6 — SPC/stability before capability conclusion
Capability is not used as a substitute for stability analysis.

The production team establishes an appropriate control-chart/rational-subgroup strategy for the seating-depth process and investigates special-cause signals.

Key distinction:
- specification limits answer whether product/process output satisfies engineering acceptance boundaries;
- control limits describe expected process behavior under the statistical model/charting method.

A point inside specification can still be evidence of a process shift.
A stable process can still be incapable of meeting specification.

## Step 7 — Reaction loop
If the control system signals abnormal behavior:
1. contain potentially affected product according to defined boundary;
2. identify the process/change point;
3. check fixture, material lot, operator/method, equipment and measurement system;
4. correct special cause where found;
5. verify recovery;
6. disposition affected product;
7. update PFMEA/Control Plan/work instruction/maintenance or measurement controls if the learning changes the known risk/control model.

The loop is intentionally circular:
Risk analysis → controls → measurements → process evidence → reaction → new knowledge → updated risk/control model.

## Listener decision tool — Do not calculate Cpk yet
Before accepting a capability number, ask:
1. What requirement/CTQ are we assessing?
2. Are specification limits engineering/customer requirements rather than limits inferred from current process data?
3. Is the measurement system adequate for the decision?
4. Is the process stable enough for the capability model being used?
5. Are data representative of the production configuration, operators, equipment, materials and conditions being claimed?
6. Are distribution/model assumptions understood?
7. Is sample size/time span adequate for the claim?
8. Are multiple machines/cavities/lines/lots being incorrectly pooled?
9. Does Cpk answer the business/risk question, or are yield, tails, defects or attribute failures more relevant?
10. What reaction occurs if the process drifts after the study?

## Claims captured
### P2-C-Q-001 — PFMEA and Control Plan should be connected
status: STRONG for AIAG-style quality-core-tool use.
Control Plans should consume relevant process-risk information rather than being independently invented inspection lists.

### P2-C-Q-002 — Calibration alone does not establish measurement-system adequacy
status: STRONG.
Measurement adequacy can involve repeatability, reproducibility, stability, bias, resolution, linearity, hysteresis, drift and configuration effects.

### P2-C-Q-003 — Stability and capability are different questions
status: STRONG.
Capability compares stable/in-control process behavior against specification limits.

### P2-C-Q-004 — Control limits and specification limits are not interchangeable
status: STRONG.
They arise from different questions and must not be substituted for each other.

### P2-C-Q-005 — A high calculated Cpk cannot rescue poor evidence quality
status: STRONG ENGINEERING SYNTHESIS.
The mathematical result inherits limitations in measurement, representativeness, stability and model assumptions.

## Podcast hooks
- “Your Cpk is 1.67. Do you actually know what you measured?”
- “A calibrated gauge can still be the wrong measurement system.”
- “Inspection catches mistakes. Process control is supposed to stop you making them repeatedly.”
- “Inside spec does not mean in control; in control does not mean capable.”

## Next P2.03 work
1. add a numeric MSA/Gauge R&R mini-dataset and show how measurement error changes interpretation;
2. add a numeric SPC example with a special-cause shift that remains inside specification;
3. add explicit reaction-plan and containment worked example;
4. package the chain into a one-page listener quality-gate tool;
5. technical review and promote P2.03 to NEAR PODCAST READY.