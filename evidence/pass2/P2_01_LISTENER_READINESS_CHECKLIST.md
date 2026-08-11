# Pass 2.01 — Listener Readiness Checklist

status: PRACTICAL PODCAST TOOL
created_on: 2026-08-11
maps_to: Opening Arc A1–A8; Episodes 1–5, 26–31, 60
companions: P2_01_HARDWARE_READINESS_DEFINITIONS.md; P2_01_WORKED_EXAMPLE_SENTINEL_NODE.md; P2_01_DEV_LVP_SVP_READINESS_MATRIX.md

## Purpose
Give a hardware team a compact self-audit that helps answer two questions:
1. Where are we actually operating today — DEV, LVP or SVP?
2. What evidence is missing before we can credibly claim the next level of production maturity?

This is not a certification checklist and does not create universal phase gates. It is a listener-facing evidence prompt informed by NASA PRR and DoD MRL concepts and adapted for startup/commercial hardware use.

## Step 1 — State the claim before scoring anything
Write one sentence:

> We believe __________ is ready for __________ under __________ conditions.

Examples:
- The sensing architecture is ready for an engineering prototype under the intended temperature range.
- The assembly process is ready for a 100-unit LVP build using trained production operators.
- The production system is ready to sustain 500 accepted units/week under the current product mix and staffing model.

If the claim is vague, the evidence discussion will also be vague.

## Step 2 — Check the twelve evidence dimensions
Mark each item:
- `0 — UNKNOWN / NOT CONTROLLED`
- `1 — ENGINEERING / DEV EVIDENCE`
- `2 — REPEATABLE LVP EVIDENCE`
- `3 — SUSTAINED SVP EVIDENCE`

Do not average blindly. A single weak critical dimension can block the claimed transition.

### 1. Requirements and CTQs
- [ ] Critical functional/environmental/safety requirements are explicit.
- [ ] CTQs relevant to manufacturing are identified.
- [ ] Verification/acceptance method exists for critical requirements.

Sentinel Node example:
DEV: detect vibration within a useful range.
LVP: defined sensing accuracy, sealing and connector requirements tied to production tests.
SVP: controlled requirements with field feedback and disciplined change.

### 2. Product configuration
- [ ] We can identify exactly which BOM/drawing/PCB/firmware revision was built or tested.
- [ ] Approved substitutions/deviations are visible.
- [ ] Change effectivity can identify which units/lots are affected.

Sentinel Node example:
If Rev B PCB + FW 1.4 + gasket supplier B cannot be reconstructed for a returned unit, the product is not configuration-controlled enough for mature production evidence.

### 3. Materials/components/suppliers
- [ ] Critical materials/components are production-intent or differences are explicitly bounded.
- [ ] Critical suppliers/processes have suitable qualification evidence for the current stage.
- [ ] Supplier/sub-tier changes trigger impact assessment where needed.

Sentinel Node example:
A dev-board accelerometer proves sensing physics; it does not prove the production sensor, PCB layout, solder process or supply chain.

### 4. Manufacturing route
- [ ] The intended production process is defined enough to reproduce the build.
- [ ] Prototype/bridge-process differences from target serial process are explicit.
- [ ] Process changes trigger revalidation assessment.

Sentinel Node example:
CNC enclosure evidence cannot automatically validate injection-molded enclosure behavior for sealing, warpage or tolerance stack.

### 5. Tooling/fixtures/equipment
- [ ] Critical fixtures/tooling are repeatable and controlled for the claimed stage.
- [ ] Calibration/maintenance state is known where relevant.
- [ ] Failure/recovery and spare strategy exist when equipment becomes production-critical.

### 6. Work instructions and operator independence
- [ ] A non-designer can build/test the unit from controlled information.
- [ ] Hidden tribal knowledge is identified and being retired.
- [ ] Exceptional engineering intervention is recorded, not normalized.

Sentinel Node red flag:
Every unit needs the design engineer to manually tune a hidden coefficient before final test passes.

### 7. Measurement and production test
- [ ] The measurement/test method is suitable for the decision being made.
- [ ] Test limits trace back to requirements/CTQs.
- [ ] Measurement-system limitations are understood.
- [ ] False-accept/false-reject risk is considered where material.

### 8. Quality controls and reaction plan
- [ ] Critical failure mechanisms have prevention/detection controls.
- [ ] Out-of-control/nonconforming conditions have a defined reaction path.
- [ ] NCR/deviation/CAPA or equivalent mechanisms match the maturity/risk level.

### 9. Yield/rework/scrap
- [ ] FPY is visible separately from final yield where useful.
- [ ] Rework and scrap are captured by operation/failure mode.
- [ ] Yield loss feeds design/process improvement rather than disappearing into final-pass reporting.

Sentinel Node example:
15% final-test failure that is later repaired is still production-system loss; if caused by connector-pin damage during assembly, it should feed fixture/work-instruction/process controls.

### 10. Rate/capacity/flow
- [ ] Takt, cycle time, throughput and capacity are not being used interchangeably.
- [ ] The system bottleneck/constraint is identified.
- [ ] Capacity assumptions include realistic downtime, staffing, product mix and rework.
- [ ] Target rate has been demonstrated for a meaningful duration when claimed.

Sentinel Node example:
Fast mechanical assembly does not prove system capacity if calibration/test is the actual constraint.

### 11. Economics
- [ ] Cost model includes actual or bounded yield/rework/inspection/logistics assumptions.
- [ ] Bridge/serial process trade-offs include NRE/tooling and design-change risk.
- [ ] Automation decisions use lifecycle/TCO logic, not labor-only arithmetic.

### 12. Traceability/service/field feedback
- [ ] Build genealogy is sufficient to investigate defects/returns for the current risk level.
- [ ] Field/service failures can be tied back to relevant configuration/process/supplier evidence where needed.
- [ ] Lessons from returns feed requirements, design, PFMEA/control plan or process changes.

## Step 3 — Identify your dominant maturity pattern

### Mostly `1` → DEV / Learning System
You are primarily proving the product and retiring technical uncertainty.
This is healthy if prototype shortcuts and evidence limitations are explicit.

### Mostly `2` → LVP / Learning Production System
You are proving repeatability through controlled, increasingly representative production.
The central question becomes whether ordinary production resources can build conforming units repeatedly without continuous design-engineer rescue.

### Mostly `3` → SVP / Sustained Production System
You have evidence that rate, quality, cost, supply, maintenance and change discipline can be sustained under defined operating conditions.

## Critical-gate rule
Do not promote maturity from a numeric average alone.
A product can score highly overall and still be blocked by one critical weakness, for example:
- unsafe/unverified requirement;
- unreconstructable configuration;
- unqualified critical supplier/process;
- unreliable measurement system;
- unsustainable constraint capacity;
- hidden engineering rescue needed on every unit.

## Five questions before declaring the next stage
1. **What exactly are we claiming is ready?**
2. **What evidence proves that claim?**
3. **Was that evidence generated on a representative product/process/environment?**
4. **What workaround, sorting, rework or expert intervention was required?**
5. **What changed since then that could invalidate the evidence?**

## Transition mini-checklists

### DEV → LVP
Proceed only when the planned build will teach you about the intended production system, not just about prototype craftsmanship.

Minimum prompts:
- [ ] Build configuration is reproducible.
- [ ] Prototype-vs-production-intent differences are explicit.
- [ ] Non-designers can build/test from controlled information.
- [ ] CTQs and core controls exist.
- [ ] Critical supplier/process assumptions are representative enough.
- [ ] Traceability/change/NCR mechanisms preserve learning.

### LVP → SVP
Proceed only when the integrated production system can sustain business-required output without exceptional intervention.

Minimum prompts:
- [ ] Accepted rate is sustainable, not a short burst.
- [ ] Constraint capacity is known.
- [ ] Yield is acceptable without hidden sorting/rework dependence.
- [ ] Measurement/control systems are trustworthy for CTQs.
- [ ] Suppliers/material flow support planned rate.
- [ ] Maintenance/recovery/downtime assumptions are realistic.
- [ ] Cost per good part reflects actual production behavior.
- [ ] Change cut-in preserves configuration/genealogy/evidence.

## Listener takeaway
Do not ask only, “How many units have we built?”
Ask:

> **What kind of system produced those units, under what conditions, with what evidence, and can that evidence survive the next change in volume, process, supplier or configuration?**

## Governance / applicability
This checklist is an editorial synthesis. Tailor rigor to product risk, complexity, regulation, lifecycle and business context. It must not be presented as a NASA, DoD or ISO checklist.