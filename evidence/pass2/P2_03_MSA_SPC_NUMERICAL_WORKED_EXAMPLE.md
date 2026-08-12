# Pass 2.03 — MSA + SPC Numerical Worked Example

status: ACTIVE — NUMERICAL WORKED EXAMPLE
created_on: 2026-08-12
maps_to: Quality foundations; Pilot/PVT; Sentinel Node

## Purpose
Demonstrate with one compact Sentinel Node CTQ why three different questions must not be collapsed:
1. Can we trust the measurement system?
2. Is the manufacturing process statistically stable?
3. If stable, is it capable relative to engineering specifications?

This is a teaching example, not a universal MSA/SPC acceptance standard.

## CTQ
Connector seating depth after assembly.

- Target: 5.00 mm
- LSL: 4.80 mm
- USL: 5.20 mm

Failure mechanism: insufficient seating can damage/partially engage connector pins and create intermittent or final-test failures.

---

## Part A — Measurement-system study

### Study design
Ten representative parts spanning the process range are measured by three operators, twice each, in randomized order. The production measurement method is a manual depth gauge/fixture.

The exact study design and acceptance thresholds must be chosen for the application; this example is intended to expose repeatability/reproducibility risk.

### Reference part values used to generate the teaching dataset
| Part | Reference-like depth (mm) |
|---|---:|
| P1 | 4.86 |
| P2 | 4.90 |
| P3 | 4.94 |
| P4 | 4.97 |
| P5 | 4.99 |
| P6 | 5.02 |
| P7 | 5.05 |
| P8 | 5.08 |
| P9 | 5.11 |
| P10 | 5.15 |

### Observed production-gauge pattern
The manual method exhibits two effects:
- repeat readings on the same part commonly differ by roughly 0.02–0.04 mm;
- Operator C tends to read roughly 0.02–0.03 mm higher than Operator A on the same parts.

This is deliberately large relative to the total 0.40 mm specification width.

### Engineering interpretation
A calibration sticker alone would not expose this operator-method interaction. Before using measured production variation to make a strong capability claim, the team should characterize whether the measurement method has adequate repeatability, reproducibility, stability, resolution and bias for the decision being made.

### Improvement action
The team introduces:
- a hard datum locating feature;
- controlled gauge orientation;
- constant-force contact;
- explicit measurement work instruction;
- operator training;
- periodic check-standard monitoring.

The MSA is then repeated before relying on the method for capability evidence.

---

## Part B — SPC example: every unit is in specification, but the process shifts

Assume the improved measurement system is adequate for monitoring this CTQ.

### Baseline process
Twenty sequential baseline measurements establish an approximately centered process around 5.00 mm with short-term variation near 0.03 mm.

For the teaching example, use:
- center line ≈ 5.00 mm
- process sigma estimate ≈ 0.03 mm
- illustrative 3-sigma control limits ≈ 4.91 to 5.09 mm

These are process-behavior limits, not engineering specification limits.

### Subsequent production sequence
| Unit | Seating depth (mm) | Within spec? | SPC interpretation |
|---|---:|---|---|
| 21 | 5.01 | Yes | normal |
| 22 | 5.02 | Yes | normal |
| 23 | 5.04 | Yes | high side |
| 24 | 5.06 | Yes | high side |
| 25 | 5.07 | Yes | high side |
| 26 | 5.08 | Yes | high side |
| 27 | 5.10 | Yes | outside illustrative UCL |
| 28 | 5.11 | Yes | outside illustrative UCL |
| 29 | 5.12 | Yes | outside illustrative UCL |
| 30 | 5.13 | Yes | outside illustrative UCL |

Every unit remains below the USL of 5.20 mm, so a simple pass/fail inspection reports 100% conformity.

But the process has clearly moved away from its established behavior. The control chart should trigger investigation before the process reaches the specification boundary.

### Plausible special cause in the Sentinel story
Fixture wear or an assembly stop backing out gradually changes connector seating position.

### Reaction
1. contain affected production according to the reaction plan;
2. verify measurement system/check standard;
3. inspect fixture stop and setup;
4. identify last-known-good boundary;
5. correct the special cause;
6. verify restored process behavior;
7. disposition affected product based on risk and evidence;
8. update PFMEA/control plan/maintenance control if the failure mechanism was not adequately controlled.

---

## Part C — Why capability comes after measurement adequacy and stability

If the process were truly stable at mean 5.00 mm with sigma 0.04 mm:

Cp = (5.20 - 4.80) / (6 × 0.04) = 1.67

and, because it is centered:

Cpk = min[(5.20 - 5.00)/(3 × 0.04), (5.00 - 4.80)/(3 × 0.04)] = 1.67

But this number is only meaningful if the observed variation is a credible representation of a stable manufacturing process and the measurement system is fit for the intended decision.

If the process mean shifts to 5.10 mm while sigma remains 0.04 mm:

Cp remains 1.67 because the specification width and spread did not change.

Cpk falls to:

Cpk = min[(5.20 - 5.10)/(3 × 0.04), (5.10 - 4.80)/(3 × 0.04)] ≈ 0.83

This is a useful teaching contrast:
- Cp asks mainly about potential spread relative to tolerance;
- Cpk also reflects centering;
- neither should substitute for stability analysis or measurement-system validation.

---

## Three-question quality gate

### Gate 1 — Can I trust the numbers?
Check measurement-system adequacy for the intended decision.

### Gate 2 — Is the process behaving predictably?
Use an appropriate control-chart/runs-rule strategy and investigate special causes.

### Gate 3 — Is predictable behavior good enough for the requirement?
Only then interpret capability relative to specification limits and application-specific acceptance criteria.

Mnemonic:

**Trust the measurement → stabilize the process → assess capability.**

---

## Claims and evidence boundaries

### P2-C-Q-005 — Specification conformity does not prove statistical control
Status: STRONG.
NIST control-chart guidance distinguishes process-derived control limits from specification limits and describes signals indicating instability.

### P2-C-Q-006 — Capability analysis assumes an in-control/stable process
Status: STRONG.
NIST explicitly frames process capability as comparing the output/natural variability of a stable or in-control process with specification limits.

### P2-C-Q-007 — Gauge characterization is broader than calibration status
Status: STRONG.
NIST Gauge R&R guidance includes repeatability, reproducibility, stability, bias, resolution, linearity, hysteresis, drift and configuration/operator effects.

### P2-C-Q-008 — A capability index can be mathematically correct but decision-invalid when the measurement/process assumptions are not credible
Status: STRONG ENGINEERING SYNTHESIS.
Do not present this wording as a direct quotation from NIST.

---

## Podcast visual / show-note concept
One graphic with three horizontal bands:

1. **Specifications:** 4.80 — 5.20 mm
2. **Control limits:** approximately 4.91 — 5.09 mm
3. **Actual sequence:** points drift through the UCL while still remaining inside specification

Caption:

**The customer limit tells you when the product is unacceptable. The control chart can warn you that the process changed before you get there.**

## Guardrails
- Do not teach 1.33, 1.67 or any other Cpk value as a universal acceptance threshold.
- Do not present the illustrative 3-sigma limits above as a substitute for selecting the correct chart/subgrouping method.
- Do not use a fixed %GRR threshold as universal across all industries/applications without source and applicability.
- Do not claim calibration alone proves measurement-system adequacy.
- Do not pool machines/cavities/operators/lots blindly if the pooling hides distinct process populations.

## Next P2.03 work
1. connect this numerical example back into the PFMEA and Control Plan rows;
2. add a reaction-plan object and containment boundary;
3. add a small-data/LVP section explaining what can and cannot responsibly be inferred from 20–30 units;
4. technical review and source packaging;
5. produce listener one-page Quality Chain checklist.