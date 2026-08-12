# P2.07 — OEE Loss Tree & Recovery Worked Example

Status: ACTIVE — NUMERICAL DEPTH CAPTURED
Provenance: [GNR] synthesis with public-source anchors; standard-level applicability remains gated for episode packaging.

## Purpose

Show why an OEE value is only the beginning of engineering analysis. Two workcells can have nearly identical OEE while requiring opposite corrective actions.

Canonical principle:

> Same OEE does not mean same manufacturing problem.

OEE is a compact loss-accounting lens. Engineering action comes from decomposing the losses, connecting them to physical mechanisms, and testing recovery under representative conditions.

## OEE structure

For an equipment-centric process:

OEE = Availability × Performance × Quality

The components answer different questions:
- Availability: how much planned production time was actually operating time?
- Performance: while operating, how closely did the process approach the defined ideal rate?
- Quality: how much output was accepted/good output?

A composite value hides which mechanism dominates.

## Sentinel Node — two cells, almost identical OEE

### Cell A — Reliability / recovery problem

Semi-automatic connector insertion station.

- Availability = 82.0%
- Performance = 99.0%
- Quality = 99.0%

OEE = 0.82 × 0.99 × 0.99 = 80.37%

Loss signature:
- frequent sensor/interlock faults;
- jam recovery requires technician access;
- restart sequence is long;
- when running, cycle time is excellent;
- product quality is excellent.

Engineering interpretation:

The dominant issue is not insertion speed and not process quality. It is availability/recovery.

Likely work:
- fault Pareto;
- sensor robustness;
- jam mechanism;
- diagnostic quality;
- safe recovery sequence;
- spare strategy;
- technician/operator recovery boundary;
- MTTR/maintenance evidence.

Buying a faster actuator would be the wrong response.

### Cell B — Process / quality problem

A second insertion station reports:

- Availability = 99.0%
- Performance = 99.0%
- Quality = 82.0%

OEE = 0.99 × 0.99 × 0.82 = 80.37%

Same OEE.

Loss signature:
- almost no downtime;
- machine cycles at target speed;
- seating-force distribution is unstable;
- connector damage and false rejects consume output;
- rework is growing.

Engineering interpretation:

The dominant issue is the process/quality mechanism, not reliability.

Likely work:
- force/displacement window;
- alignment and fixture condition;
- component variation;
- measurement adequacy;
- PFMEA/Control Plan update;
- rework loop analysis;
- process stabilization before further speed optimization.

Making the machine more available would not solve the dominant loss.

## Why the comparison matters

Cell A and Cell B both report approximately 80.4% OEE.

Yet:

| Dimension | Cell A | Cell B |
|---|---:|---:|
| Availability | 82% | 99% |
| Performance | 99% | 99% |
| Quality | 99% | 82% |
| OEE | 80.37% | 80.37% |
| Dominant engineering problem | Reliability / recovery | Process / quality |
| First response | Fault/recovery engineering | Process stabilization / quality |

Therefore:

> OEE can rank the magnitude of productive-time loss, but the loss tree determines the engineering program.

## Sentinel failure/recovery dataset

Representative one-shift dataset for Cell A:

| Event | Count | Total lost min | Typical recovery owner | Observation |
|---|---:|---:|---|---|
| Part-presence sensor false fault | 6 | 24 | Operator | reset often works, cause not removed |
| Connector jam | 3 | 27 | Technician | guard access + manual extraction |
| Force sensor communication fault | 2 | 18 | Technician | controller restart required |
| Recipe mismatch | 1 | 11 | Engineer | configuration/release issue |
| Material starvation | 2 | 8 | Operator/logistics | upstream replenishment issue |
| Total | 14 | 88 | mixed | availability loss is heterogeneous |

The 88 minutes should not be treated as one generic “downtime” bucket. Each event class has a different owner and countermeasure.

### Recovery metrics to retain

For each important fault class capture:
- event frequency;
- time to detect;
- time to diagnose;
- time to make safe;
- time to repair/clear;
- time to restart;
- first-good-piece confirmation time;
- required skill level;
- genealogy/configuration impact;
- recurrence after restart.

A nominal MTTR average can hide a dangerous tail. For ramp decisions, the distribution and worst credible recovery cases may matter more than the mean.

## Recovery qualification scenario

A cell is not production-ready merely because nominal automatic operation passed.

Qualification should deliberately inject representative abnormal states, for example:

1. missing connector;
2. wrong orientation;
3. partial insertion;
4. force signal outside window;
5. sensor disagreement;
6. loss of pneumatic pressure;
7. loss of network/PLC communication as applicable;
8. power interruption;
9. wrong recipe/configuration attempt;
10. jam requiring guarded access.

For each state verify, as applicable:
- hazard is controlled;
- machine enters the intended state;
- fault is diagnosable;
- recovery instructions are unambiguous;
- unauthorized bypass is prevented/controlled;
- restart does not silently lose serial/result association;
- suspect product is identified and dispositioned;
- first-good-piece criteria are defined;
- recovery time is compatible with the production claim.

## OEE loss tree

### Availability branch

Planned production time
→ operating time loss
→ equipment failure
→ sensor/interlock fault
→ jam/blockage
→ utility loss
→ material starvation where included in local accounting
→ setup/changeover where included in local accounting
→ maintenance/recovery delay

Engineering questions:
- What physically stopped production?
- Is the loss internal to the equipment or imposed by the production system?
- Who can recover it?
- Is recurrence controlled?

### Performance branch

Operating time
→ speed loss
→ micro-stops
→ reduced cycle rate
→ waiting inside automatic cycle
→ degraded motion/process settings
→ component variation causing slower execution

Engineering questions:
- Is “ideal cycle time” technically defensible?
- Is speed loss intentional for quality/safety?
- Are micro-stops being hidden as normal cycle variation?

### Quality branch

Total output
→ accepted output loss
→ scrap
→ rework
→ false reject
→ process escape detected downstream
→ startup/restart loss

Engineering questions:
- Is rework counted consistently?
- Does the quality metric reflect accepted output or merely machine-completed cycles?
- Are downstream escapes attributed back to the source process?

## System-level guardrail

A local OEE improvement can damage system performance.

Example:
- insertion cell is accelerated;
- local Performance rises;
- downstream calibration remains the bottleneck;
- WIP grows;
- total accepted throughput does not improve.

Therefore P2.07 inherits P2.04:

> Optimize the production system constraint, not the prettiest local OEE number.

## OEE accounting guardrails

Before comparing OEE values, define consistently:
- planned production time;
- what counts as downtime;
- ideal cycle time;
- what counts as a completed unit;
- what counts as good output;
- treatment of rework;
- treatment of changeover;
- treatment of planned maintenance;
- product mix and recipe differences;
- aggregation level: machine, cell, line, or plant.

Without common definitions, OEE comparisons can be numerically precise but operationally misleading.

## Public-source anchors

### NIST — OEE as availability × performance/productivity × quality

NIST publications on robot-workcell health describe OEE as a commonly used manufacturing metric composed of availability, performance/productivity, and quality, and use it as a starting point for selecting health/performance data.

Applicability: supports the OEE decomposition and its use as a performance-loss lens. It does not prescribe the Sentinel loss tree or universal thresholds.

### NIST MEP — OEE measurement for loss visibility

NIST MEP case material describes manufacturers implementing measurement of machine availability, process performance, and product quality in order to calculate OEE and understand productivity losses.

Applicability: supports using OEE to expose losses and guide improvement. Case-study outcomes are not universal benchmark requirements.

### NIST — robot workcell health and maintenance data

NIST robot-workcell health research identifies multiple useful data streams including controller/PLC data, maintenance logs, process/part quality data, and fault/failure data.

Applicability: supports the integrated recovery dataset concept. The exact fields in this document are a project synthesis.

## Listener tool — LOSS 8

When someone presents an OEE number, ask:

1. Definition — are A/P/Q and time boundaries defined consistently?
2. Dominant loss — which component actually drives the number?
3. Mechanism — what physical/operational mechanism creates that loss?
4. Distribution — is the average hiding recurring or long-tail events?
5. Recovery — who restores production and how reliably?
6. Quality loop — are rework and downstream escapes attributed correctly?
7. System effect — does improving this machine improve accepted system throughput?
8. Evidence — was the value demonstrated under representative product, staffing, mix and duration?

## Podcast-ready claims

Safe claims after source packaging:
- OEE is commonly represented as Availability × Performance × Quality for equipment-centric manufacturing analysis.
- Equal OEE values can arise from very different loss structures and therefore do not imply equal corrective actions.
- Recovery and maintenance performance are part of sustaining automated production, not post-launch housekeeping.
- Integrated workcell assessment benefits from equipment, fault, maintenance and product-quality data.

Claims that remain project synthesis:
- LOSS 8 mnemonic;
- exact loss-tree taxonomy;
- Sentinel numerical examples;
- exact recovery dataset fields;
- the proposed abnormal-state qualification sequence.

## Next work

1. Build Automation Qualification & Release Gate.
2. Map machinery/robot/cobot safety applicability without presenting one standard as universal.
3. Connect release criteria to P2.03 quality, P2.04 capacity, P2.05 economics and P2.02 change control.
4. Package P2.07 as NEAR PODCAST READY.