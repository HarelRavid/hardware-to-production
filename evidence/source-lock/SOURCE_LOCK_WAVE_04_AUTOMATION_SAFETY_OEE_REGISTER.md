# Source-Lock Wave 04 — Automation / Machinery Safety / OEE Shared Source Register

status: SHARED SOURCE REGISTER LOCKED
checked: 2026-09-19
scope: EP41 / EP42 / EP43 / EP44 / EP45 / EP46 + P2.07
backbone: Automation / Qualification / OEE / Maintenance / Recovery / Release

## 1. Purpose

Lock the authoritative/public source layer shared by the automation episodes while keeping machinery-safety standards, legal obligations and proprietary standard clauses explicitly scoped.

Wave 04 separates:
- public standard identity/scope/current-edition metadata;
- open NIST technical evidence for robotics, automation, OEE, maintenance and measurement;
- internal Hardware-to-Production automation frameworks;
- jurisdiction/customer-specific legal and conformity obligations.

No episode may imply that a named ISO/IEC standard automatically applies to every machine, site or jurisdiction.

## 2. Current machinery / automation standards status

### W4-S01 — ISO 12100:2010
Title: Safety of machinery — General principles for design — Risk assessment and risk reduction
Edition: 1
Published: 2010-11
Current status checked: published/current; last reviewed and confirmed in 2022; revision project active.
Official source:
https://www.iso.org/standard/51528.html

Publicly supportable scope:
- machinery-design safety terminology/principles;
- risk assessment and risk reduction methodology;
- hazard identification, risk estimation/evaluation and risk-reduction principles across relevant machine lifecycle phases.

Revision watch:
ISO/DIS 12100.3 is under development and expected to replace the current published edition.
Do not treat the draft as the current normative edition.

### W4-S02 — ISO 13849-1:2023
Title: Safety of machinery — Safety-related parts of control systems — Part 1: General principles for design
Edition: 4
Published: 2023-04
Official source:
https://www.iso.org/standard/73481.html

Publicly supportable scope:
methodology/requirements/recommendations/guidance for design and integration of safety-related parts of control systems performing safety functions, including software, within stated scope.

Guardrail:
Exact PL/category/architecture calculations or requirements remain licensed-standard gated.

### W4-S03 — ISO 13849-2:2012
Title: Safety of machinery — Safety-related parts of control systems — Part 2: Validation
Edition: 2
Published: 2012-10
Current status checked: still published/current; revision active.
Official source:
https://www.iso.org/standard/53640.html

Publicly supportable scope:
validation by analysis and testing of safety functions and achieved category/performance level for SRP/CS designed according to ISO 13849-1.

Revision watch:
ISO/DIS 13849-2 Edition 3 is under development and intended to replace the 2012 edition.
Do not narrate draft requirements as current normative content.

### W4-S04 — IEC 62061 consolidated current family
Title: Safety of machinery — Functional safety of safety-related control systems
Base edition: IEC 62061:2021, Edition 2
Current consolidated version checked:
IEC 62061:2021 + AMD1:2024 + AMD2:2026
Consolidated edition: 2.2
Publication of AMD2: 2026-03-20
Stability date: 2028
Official source:
https://webstore.iec.ch/en/publication/112847

Publicly supportable scope:
requirements/recommendations for design, integration and validation of safety-related control systems for machinery within stated scope.

Guardrail:
Do not present IEC 62061 and ISO 13849 as universally interchangeable methodologies.
Exact SIL calculations/requirements remain licensed-standard gated.

### W4-S05 — ISO 10218-1:2025
Title: Robotics — Safety requirements — Part 1: Industrial robots
Edition: 3
Published: 2025-02
Official source:
https://www.iso.org/standard/73933.html

Publicly supportable scope:
industrial-robot safety requirements addressing the robot itself as partly completed machinery before integration.

### W4-S06 — ISO 10218-2:2025
Title: Robotics — Safety requirements — Part 2: Industrial robot applications and robot cells
Edition: 2
Published: 2025-02
Official source:
https://www.iso.org/standard/73934.html

Publicly supportable scope:
integration, commissioning, operation, maintenance, decommissioning and disposal of industrial robot applications/cells.

Strong episode implication:
a compliant/safety-rated robot component does not by itself establish a safe integrated application/cell.

### W4-S06A — ISO/TS 15066:2016 + revision watch

Title: Robots and robotic devices — Collaborative robots
Current published technical specification: ISO/TS 15066:2016, Edition 1
Published: 2016-02
Official source:
https://www.iso.org/standard/62996.html

Current status checked 2026-09-19:
- still published/current;
- last reviewed/confirmed in 2022;
- revision has started;
- ISO/AWI 15066-1 is under development and is intended to replace ISO/TS 15066:2016.

Publicly supportable scope:
safety requirements for collaborative industrial robot systems/work environments supplementing ISO 10218 industrial-robot application safety.

Guardrail:
do not treat ISO/AWI 15066-1 as current normative authority.
Do not use “cobot” as a complete safety conclusion; the integrated task/application still requires risk assessment and protective-measure validation.

### W4-S07 — IEC 60204-1
Title: Safety of machinery — Electrical equipment of machines — Part 1: General requirements
Current public consolidated family checked:
IEC 60204-1:2016 + AMD1:2021
Official source:
https://webstore.iec.ch/en/publication/26037

Publicly supportable scope:
electrical/electronic/programmable electronic equipment and systems of machinery within stated scope, beginning at the point of connection of supply to the machine electrical equipment.

Guardrail:
This is not a substitute for whole-machine risk assessment or functional-safety design.

### W4-S08 — IEC 62381:2024
Title: Automation systems in the process industry — Factory acceptance test (FAT), site acceptance test (SAT), and site integration test (SIT)
Edition: 3
Published: 2024-07-30
Stability date: 2029
Official source:
https://webstore.iec.ch/en/publication/67572

Publicly supportable scope:
requirements/checklists for FAT, optional FIT, SAT and SIT demonstrating that an automation system meets applicable specification requirements; project-specific test plans may be adapted.

Important boundary:
FAT/SAT/SIT do not by themselves prove downstream manufacturing-process qualification, sustainable accepted throughput, or all commissioning/production-release claims.

### W4-S09 — ANSI/ISA-62381-2026 / IEC 62381:2024 IDT
Owner: ISA / ANSI adoption
Public status source:
https://www.isa.org/standards-and-publications/isa-standards/news

Use:
status/watch only. No ISA protected standard content is reproduced or used as AI-derived detailed requirements.

## 3. OEE current reference layer

### W4-S10 — ISO 22400-2:2014 + Amd 1:2017
Title: Automation systems and integration — Key performance indicators for manufacturing operations management — Part 2: Definitions and descriptions
Edition: 1
Published: 2014-01
Amendment: 2017
Official source:
https://www.iso.org/standard/54497.html

Current status:
published, revision active.
ISO/DIS 22400-2 Edition 2 is under development and approved for progression toward FDIS.

Guardrail:
The draft is not current normative authority.

### W4-S11 — NIST AMS 300-11 manufacturing-data recommendations
Owner: NIST
Source:
https://nvlpubs.nist.gov/nistpubs/ams/NIST.AMS.300-11.pdf

Open technical support:
OEE is described as the product of availability/uptime, performance/speed versus design, and quality/first-pass-yield rate.

Episode use:
generic OEE formula and metric context without reproducing protected ISO content.

### W4-S12 — NIST AMS 100-18 maintenance economics
Owner: NIST
Source:
https://nvlpubs.nist.gov/nistpubs/ams/NIST.AMS.100-18.pdf

Support:
- OEE is commonly used in manufacturing/TPM contexts;
- OEE = Availability × Performance Rate × Quality Rate;
- maintenance strategy, downtime and maintenance losses are economically material.

Episode use:
EP45 maintenance/OEE/economics.

### W4-S13 — NIST MEP KEATS OEE case
Owner: NIST MEP
Source:
https://www.nist.gov/mep/successstories/2023/keats-hydraulic-press-oee-system

Support:
manufacturer implemented measurement of availability, process performance and quality to calculate OEE and expose equipment losses.

Guardrail:
case outcomes are not universal OEE benchmarks.

## 4. Robotics / automation technical source layer

### W4-S14 — NIST MEP Robotics and Manufacturing Automation
Source:
https://www.nist.gov/mep/robotics-and-manufacturing-automation

Support:
automation assessment should begin with operational needs/business case; potential benefits include productivity/capacity, consistency/quality/yield, safety and data, depending on application.

Guardrail:
automation benefits are possible outcomes, not guaranteed causal results.

### W4-S15 — NIST robotic systems interoperability/integration
Source:
https://www.nist.gov/programs-projects/robotic-systems-interoperability-and-integration

Support:
robot integration can be difficult/expensive; custom hardware/software, constrained environments and human expertise can remain barriers; reconfiguration/interoperability matter.

Episode use:
EP41/43/46.

### W4-S16 — NIST assembly robot benchmarking
Source:
https://www.nist.gov/publications/benchmarking-protocols-evaluating-small-parts-robotic-assembly-systems

Support:
robotic assembly systems require application-relevant performance metrics/test methods; technical demonstration is not sufficient without representative evaluation.

### W4-S17 — NIST task-based HRC safety
Source:
https://www.nist.gov/publications/characterizing-task-based-human-robot-collaboration-safety-manufacturing

Support:
human-robot collaboration safety can be evaluated from the task/application perspective, including tooling, expected contact and force/pressure transfer.

Episode implication:
"cobot" is not a safety conclusion.

### W4-S18 — NIST industrial robot performance/repeatability
Source:
https://www.nist.gov/publications/helping-robots-stay-target

Support:
robot repeatability and accuracy are distinct; both can matter to manufacturing process requirements and can degrade without preparation/maintenance.

Episode use:
EP43/45.

## 5. Shared engineering claims

### W4-C01 — Automation is a process-design decision, not a maturity badge
Status: VERIFIED + V6 SYNTHESIS
Support: W4-S14/S15/S16 + Wave 03 economics.
Claim:
technical feasibility is only one dimension; process stability, safety, integration, recovery, change, economics and system constraint matter.

### W4-C02 — Simplest effective intervention should be compared with full automation
Status: VERIFIED AS DECISION SYNTHESIS
Support: NIST automation/business-case sources + Wave 03 economics.
Claim:
fixture/poka-yoke/assisted/semi-automatic alternatives should be considered where they can solve the demonstrated mechanism with lower irreversible complexity.

### W4-C03 — Robot component safety does not establish application/cell safety
Status: VERIFIED PUBLIC SCOPE
Support: W4-S05/S06.
Claim:
robot and integrated application/cell are separate safety scopes.

### W4-C04 — Collaborative operation is task/application dependent
Status: VERIFIED
Support: W4-S17 + ISO 10218-2 scope.
Claim:
human-robot task, tooling, contact and protective measures must be assessed for the integrated application.

### W4-C05 — FAT/SAT/SIT and production release answer different questions
Status: VERIFIED + V6 SYNTHESIS
Support: W4-S08.
Claim:
IEC 62381 acceptance tests demonstrate automation-system conformance to applicable specification; production quality/rate/recovery release may require additional evidence.

### W4-C06 — OEE is a composite loss metric
Status: VERIFIED OPEN SOURCE
Support: W4-S11/S12.
Claim:
OEE = Availability × Performance × Quality for the episode's equipment-centric analysis.

### W4-C07 — OEE is not root-cause proof or system-capacity proof
Status: VERIFIED + V6 SYNTHESIS
Support: OEE composite nature + Wave 03 capacity/constraint logic.
Claim:
the loss decomposition and physical mechanism determine corrective action; local OEE does not establish accepted system throughput.

### W4-C08 — Equal OEE can represent different problems
Status: ILLUSTRATIVE ARITHMETIC VERIFIED + V6 SYNTHESIS
Support:
Cell A and B worked examples.

### W4-C09 — Automated test remains a measurement/decision system
Status: DEPENDENCY — Wave 02
Claim:
100% automated test coverage does not remove measurement adequacy, false-accept/reject, calibration/configuration and genealogy requirements.

### W4-C10 — Maintenance and recovery are part of automation qualification/economics
Status: VERIFIED
Support: W4-S12 + robotics integration sources.
Claim:
sustained automation readiness includes fault diagnosis/recovery, maintenance/spares/support and post-maintenance verification where affected.

### W4-C11 — Changes can invalidate automation evidence selectively
Status: DEPENDENCY — Wave 01 + V6 automation application
Claim:
product/tooling/software/recipe/sensor/layout/speed/task changes require impact assessment against the qualified/safety evidence envelope.

### W4-C12 — Scale can replicate defects and evidence weaknesses
Status: VERIFIED AS SYSTEM SYNTHESIS
Support: Wave 02 quality + Wave 03 scale/capacity + W4 integration sources.
Claim:
replicating a cell multiplies both capability and unresolved instability unless equivalence and process maturity are demonstrated.

## 6. Safety applicability rule

The generic standards map is engineering guidance only.

Before a script uses language equivalent to "required by law", "CE requires", "OSHA requires", "Israel requires", or similar:
- jurisdiction must be explicit;
- applicable legal/regulatory source must be locked;
- standards/legal status must be distinguished;
- exact edition/transition/conformity route must be verified.

Wave 04 scripts should normally say:
"Depending on machine, application and jurisdiction, standards such as ... may form part of the safety engineering/conformity framework."

Do not convert an international engineering standard into a generic legal obligation.

## 7. Sentinel OEE arithmetic lock

### Semi-automatic insertion station
Planned production time: 420 min
Unplanned downtime: 42 min
Operating time: 378 min = 22,680 s
Availability: 378/420 = 0.9000

Ideal cycle: 45 s
Total cycles: 470
Performance: (45×470)/22,680 = 0.93253968 ≈ 93.25%

Good units: 451
Quality: 451/470 = 0.95957447 ≈ 95.96%

OEE:
0.9000 × 0.93253968 × 0.95957447 = 0.80535714 ≈ 80.54%

Status:
ARITHMETIC VERIFIED — ILLUSTRATIVE MODEL.

### Equal-OEE worked example
Cell A:
0.82 × 0.99 × 0.99 = 0.803682 = 80.3682%

Cell B:
0.99 × 0.99 × 0.82 = 0.803682 = 80.3682%

Status:
ARITHMETIC VERIFIED — illustrates equal composite metric with different dominant loss branches.

## 8. Hard guardrails

1. No "85% OEE = world class" universal benchmark.
2. No OEE value used as root-cause proof.
3. No local OEE used as proof of system capacity.
4. Planned-production-time, ideal-cycle and good-output definitions must be explicit.
5. Robot repeatability is not equivalent to process capability.
6. "Cobot" is not a safety conclusion.
7. Robot component conformity does not establish application/cell conformity.
8. ISO 12100/13849/10218, IEC 62061/60204-1 and other standards are not automatically legal requirements in every jurisdiction/application.
9. Exact PL/SIL/safety-function calculations require licensed/current standards and competent safety engineering.
10. FAT/SAT success is not production qualification by itself.
11. Predictive maintenance is not automatically superior to preventive maintenance.
12. Restart after a fault/repair does not automatically restore configuration, genealogy, measurement or release trust.
13. Automation economics must reuse Wave 03 evidence and not assume labor savings, demand, uptime or yield improvement.
14. Automated test must reuse Wave 02 measurement rules.
15. Replicated cells are not assumed equivalent without evidence.

## 9. Episode mapping

EP41:
automation readiness; process stability, constraint and do-not-automate conditions.

EP42:
automation economics; direct reuse of Wave 03 P2.05 source lock and W4 lifecycle/integration/maintenance sources.

EP43:
function-level automation boundary, robotics, vision, human/automation allocation and safety applicability.

EP44:
automated inspection/EOL test; direct reuse of Wave 02 measurement evidence plus automation configuration/drift/recovery.

EP45:
automation qualification, IEC 62381 FAT/SAT/SIT scope, OEE/loss tree, maintenance/recovery, safety applicability and release envelope.

EP46:
scale readiness, replicated-equipment equivalence, moving constraint and controlled incremental scaling.

## 10. Unresolved application gates

Not blockers for current generic scripts:
- exact machine-safety legal obligations in Israel/EU/US or other jurisdiction;
- exact ISO/IEC clauses, PL/SIL calculations, guard/interlock design requirements;
- exact FAT/SAT acceptance checklists from IEC 62381;
- exact customer validation protocols;
- site-specific lockout/commissioning/permit requirements;
- machine-specific maintenance intervals;
- OEE benchmark targets;
- exact robot/cell conformity-assessment route;
- exact vision false-accept/fail thresholds;
- sector-specific automated-test acceptance statistics.

These require separate applicability/source locks if added to final narration.
