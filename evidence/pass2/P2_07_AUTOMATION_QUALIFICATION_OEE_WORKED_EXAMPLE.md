# P2.07 — Automation / Qualification / OEE — Worked Example

Status: ACTIVE — WORKED EXAMPLE CAPTURED
Provenance: [GNR] architecture/synthesis pending source-level packaging; public-source anchors noted below.

## Purpose

Build a decision framework for automation that begins with the manufacturing problem and evidence, not with a robot purchase.

Canonical progression:

Manual → Fixture / Poka-Yoke → Assisted → Semi-Automatic → Automatic

Automation maturity is not a prestige ladder. The correct level is the lowest-complexity solution that can robustly satisfy the required safety, quality, rate, flexibility and economics envelope.

## Sentinel Node scenario

Process: connector insertion and seating verification.

Observed LVP problem:
- manual insertion is operator-sensitive;
- connector-pin damage has already appeared in the quality-chain example;
- seating depth is a CTQ;
- variation is driven by alignment, insertion force, operator technique and inspection method;
- the downstream calibration/test station is already capacity-sensitive.

The team proposes a fully automated robotic insertion cell.

The engineering question is not “Can a robot perform the motion?”

It is:

> Which intervention removes the dominant failure mechanism with acceptable safety, quality, recovery, flexibility, rate and lifecycle economics?

## Intervention ladder

### Level 0 — Manual

Operator aligns and inserts connector by hand and verifies seating.

Useful when:
- volume is low;
- design is changing rapidly;
- the task remains safe;
- learning value is high.

Risk:
- operator variation;
- weak force control;
- inconsistent detection of partial seating.

### Level 1 — Fixture / Poka-Yoke

Add keyed alignment nest, hard stops and controlled support of the mating component.

Hypothesis:
- remove misalignment before adding automation complexity.

Required evidence:
- reduction in pin-damage failure mode;
- repeatable seating depth;
- ergonomic/safety review;
- fixture wear and maintenance behavior.

### Level 2 — Assisted process

Operator loads the product; guided tooling applies controlled insertion force/displacement and records the result.

Potential benefits:
- controlled force;
- better repeatability;
- automatic data capture;
- human retains flexible loading/recovery.

### Level 3 — Semi-automatic

Operator loads/unloads; machine executes alignment, insertion, verification and result capture.

Now qualification must include:
- part presence/orientation detection;
- force/displacement window;
- error detection;
- recovery logic;
- wrong-part prevention;
- data association to serial number;
- maintenance/calibration requirements.

### Level 4 — Automatic cell

Automated handling + insertion + verification + routing/reject handling.

The burden of evidence expands:
- guarding/collaborative safety as applicable;
- interfaces and interlocks;
- abnormal-condition behavior;
- restart/recovery;
- recipe/configuration control;
- traceability;
- changeover/product-mix performance;
- maintainability and spare-parts strategy;
- sustained availability and throughput.

## Automation qualification chain

User need / manufacturing problem
→ CTQ and failure mechanism
→ automation concept
→ risk assessment
→ acceptance criteria
→ design verification
→ installation/integration verification
→ process qualification
→ production-rate demonstration
→ recovery/maintenance demonstration
→ controlled release
→ ongoing performance monitoring
→ change control / requalification

The exact IQ/OQ/PQ terminology is industry-specific and must not be presented as universally mandatory. The underlying engineering logic is broader: prove installation/integration, operating envelope, product/process performance and sustained operation appropriate to the claim.

## OEE: useful but not the automation decision itself

For an equipment-centric process, OEE is commonly decomposed conceptually into:

OEE = Availability × Performance × Quality

Worked example for the semi-automatic insertion station:
- Planned production time: 420 min
- Unplanned downtime: 42 min
- Availability = 378 / 420 = 90.0%
- Ideal cycle time: 45 s
- Total cycles: 470
- Operating time: 378 min = 22,680 s
- Performance = (45 × 470) / 22,680 = 93.25%
- Good units: 451
- Quality = 451 / 470 = 95.96%

OEE ≈ 0.900 × 0.9325 × 0.9596 ≈ 80.5%

But the 80.5% number alone does not identify the engineering action.

Loss decomposition matters:
- Availability loss may be sensor faults or jam recovery;
- Performance loss may be slow insertion caused by part variation;
- Quality loss may be connector damage or false rejects.

Therefore:

> OEE is a loss lens, not a root-cause analysis and not proof that the automation was the right investment.

## The “high OEE / wrong automation” trap

A cell can have high OEE and still be a bad manufacturing decision if:
- demand is too low to justify the investment;
- product changes make it obsolete;
- manual/fixture solutions would meet the requirement more cheaply;
- changeovers destroy system-level capacity;
- maintenance expertise is unavailable;
- upstream/downstream constraints dominate;
- safety or recovery complexity is excessive.

Conversely, an early production cell may have modest OEE while still being valuable if the losses are understood and rapidly improving inside a deliberate learning phase.

## Qualification test categories

1. Safety and abnormal states
   - e-stop / protective functions as applicable;
   - loss of air/power/network;
   - unexpected part state;
   - safe restart.

2. Product quality
   - CTQ distribution;
   - defect/escape detection;
   - false reject behavior;
   - measurement adequacy.

3. Process envelope
   - expected component variation;
   - environmental/utility variation;
   - recipe limits;
   - tooling wear.

4. Rate
   - cycle-time distribution, not only best cycle;
   - sustained accepted throughput;
   - interaction with bottlenecks and WIP.

5. Recovery
   - mean time to diagnose/recover relevant faults;
   - operator vs technician intervention;
   - restart without genealogy/configuration loss.

6. Maintainability
   - preventive maintenance;
   - calibration;
   - consumables/spares;
   - access and service time.

7. Change and flexibility
   - product variant;
   - firmware/recipe revision;
   - component substitution;
   - tooling/changeover;
   - requalification triggers.

## AUTOMATE 10 — listener tool

Before approving automation, ask:

1. Problem — what failure, constraint, safety exposure or cost are we solving?
2. Mechanism — do we understand the physical/process mechanism?
3. Simpler — can fixture, poka-yoke, method or assisted tooling solve it first?
4. Stability — is the underlying process sufficiently understood/stable to automate?
5. Quality — how will CTQs and failures be measured/detected?
6. Safety — what new hazards and abnormal states does automation create?
7. Rate — does it improve the actual system constraint and accepted throughput?
8. Recovery — who restores production when it fails, and how long does that take?
9. Change — how will variants, revisions and substitutions be controlled?
10. Economics — does lifecycle evidence justify the investment under uncertainty?

Hard-stop principle:

> Do not automate an unstable or poorly understood failure mechanism merely to make it fail faster and less visibly.

## Sentinel decision

Initial recommendation for the connector problem:

Do not jump directly to full robotic automation.

First test:
1. alignment poka-yoke fixture;
2. controlled insertion force/displacement;
3. automatic seating verification and traceable data capture;
4. evaluate resulting FPY, cycle time and recovery burden;
5. only then evaluate semi/full automation if rate/economics evidence requires it.

This preserves learning while attacking the failure mechanism directly.

## Public-source anchors for later evidence packaging

- NIST MEP, “Robotics and Manufacturing Automation”: automation opportunities should be assessed against operational need/business case; cited benefits include productivity, capacity, consistency/quality/yield, worker safety and operational data.
- NIST robotics programs: robotic performance must be characterized and verified at both component and integrated-system level; safety, agility and ease of integration are explicit concerns.
- NIST discussion of collaborative robotics references ISO/TS 15066 safety requirements; any episode-level standards claim requires current standard/version applicability review before publication.

## Guardrails

- “Collaborative robot” does not automatically mean a complete application is safe.
- OEE targets such as “85% world class” must not be treated as universal engineering requirements.
- OEE is most natural for equipment-centric processes; manual operations may require different loss/accounting metrics.
- A short successful demo does not establish sustained availability, maintainability or capacity.
- Automation acceptance must use production-representative product, people, interfaces and operating conditions appropriate to the claim.

## Next work

1. Build automation failure/recovery dataset for Sentinel Node.
2. Create OEE loss-tree example showing why equal OEE values can require completely different actions.
3. Build Automation Qualification / Release Gate.
4. Add safety-standard applicability map (robot/cobot/machinery/application-specific).
5. Package P2.07 canonical listener framework and move toward NEAR PODCAST READY.
