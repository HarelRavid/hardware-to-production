# Automation Business Case / Qualification / OEE — Evidence Source Map

status: BREADTH COMPLETE
campaign: A7
maps_to: MASTER_WBS Section 8; PODCAST_MAP Episodes 41–46
provenance: primary-source-first

## Purpose
Build the evidence backbone for deciding when automation creates value, how automated equipment/processes should be qualified, and how OEE/maintenance/reliability data should be interpreted without confusing high equipment utilization with good manufacturing economics.

## Primary / authoritative backbone captured

### ISA-105 / ANSI-ISA-62381 / IEC 62381 — FAT, SAT and SIT
Structured methodology for Factory Acceptance Test, Site Acceptance Test and Site Integration Test of automation systems. FAT/SAT/SIT are requirements-based acceptance layers and do not by themselves prove every downstream commissioning, MES or production-validation requirement.

### NIST AMS 100-18 — Costs and Benefits of Advanced Maintenance in Manufacturing
Supports treating maintenance, downtime and maintenance strategy as lifecycle/economic inputs to automation rather than post-installation overhead.

### NIST / ISO 22400 context — manufacturing performance and OEE
Supports OEE as a manufacturing/asset-performance metric. OEE must not be equated automatically with profitability, customer value or system throughput.

### ISO 10218-1:2025 and ISO 10218-2:2025 — industrial robot safety
ISO 10218-1 addresses safety requirements for industrial robots as partly completed machinery. ISO 10218-2 addresses industrial robot applications/cells and explicitly extends the safety problem into integration, commissioning, operation, maintenance and decommissioning.

Engineering use:
- robot safety is not solved by purchasing a compliant robot alone;
- application/cell integration creates its own risk-assessment and safeguarding obligations;
- tooling, workpiece, interfaces, operating mode, maintenance and human interaction matter to the system-level safety case.

Applicability boundary: industrial robots/applications only; other machinery and sector requirements may apply in parallel.

### NIST — task-based human-robot collaboration safety
NIST research demonstrates a task-based approach to human-robot collaboration risk assessment during design, considering tooling, expected contact and force/pressure transfer.

Engineering use:
- collaborative operation is application/task dependent, not an inherent universal property of a robot;
- human-automation allocation should include safety, task structure and recovery, not only nominal cycle time.

### NIST Assembly Task Board / robotic assembly benchmarking literature
Benchmarking of off-the-shelf robotic assembly solutions identifies adoption constraints including expertise dependence, limited applicability, interoperability limitations, lack of scene awareness/error recovery and cost.

Engineering use:
- technical demonstration is not the same as robust production deployment;
- recovery behavior, integration and internal expertise belong in the automation business case;
- flexible automation value depends on actual task/product variability.

## Decision dimensions
- process stability/maturity
- volume/rate and demand certainty
- labor content and ergonomic/safety benefit
- CTQ/capability opportunity
- automation technical feasibility
- product mix/changeover/flexibility
- NRE/integration/tooling cost
- maintenance/spares/support
- uptime/reliability
- programming/change complexity
- inspection/data benefit
- cybersecurity/OT integration
- operator/technician skill needs
- failure/recovery mode
- lifecycle/obsolescence
- ROI/payback/TCO

## Claim register
### C-AUTO-001 — Technical feasibility does not by itself justify automation
status: STRONG ENGINEERING SYNTHESIS
Feasibility must be separated from business/system justification: demand, process maturity, flexibility, integration, maintenance, support, downtime, safety, lifecycle and TCO matter.

### C-AUTO-002 — Automating an unstable or poorly understood process can preserve existing losses and make recovery harder
status: STRONG SYNTHESIS / PASS-2 CASE NEEDED
Do not present as a universal slogan. The mechanism is strong; Pass 2 should add a direct industrial case.

### C-AUTO-003 — Automation business cases should include lifecycle costs beyond direct labor savings
status: STRONG
Maintenance/downtime evidence plus deployment constraints support a broader TCO boundary including integration, tooling, support, training, recovery, spares and change costs.

### C-AUTO-004 — FAT, SAT/SIT and production qualification answer different acceptance questions
status: STRONG / APPLICABILITY-SCOPED

### C-AUTO-005 — OEE is a composite manufacturing-performance metric, not equivalent to profitability or customer value
status: STRONG DIRECTION
Precise formula/ISO 22400 definition work remains Pass 2.

### C-AUTO-006 — High local utilization can worsen system flow when disconnected from system constraints
status: STRONG SYNTHESIS from A5
Pass 2 should add a worked flow/WIP example.

### C-AUTO-007 — Automated systems require explicit failure/recovery, maintenance and safe-state strategies
status: STRONG
Robot-system safety and deployment evidence support system-level treatment beyond nominal automatic operation.

### C-AUTO-008 — Product/configuration change can invalidate automation qualification or economics
status: STRONG SYNTHESIS
A new geometry, material, tolerance, software interface, cycle requirement or product mix can alter tooling, safety, process window, inspection, cycle time and business-case assumptions. Exact requalification requirements remain context-specific.

### C-AUTO-009 — FAT pass does not prove installed-site performance
status: STRONG

### C-AUTO-010 — SAT pass does not universally equal production-process qualification
status: STRONG / APPLICABILITY-SCOPED

### C-AUTO-011 — A safe robot component does not by itself establish a safe robot application/cell
status: STRONG
ISO 10218 separates robot requirements from application/cell integration requirements.

### C-AUTO-012 — Human-robot collaboration safety is task/application dependent
status: STRONG
NIST task-based HRC research supports evaluating tooling, contact and task-specific hazards during design.

## Automation decision ladder
1. Is the product/process stable enough to automate?
2. What problem are we solving: safety, ergonomics, quality, rate, labor availability, data, cost or a constraint?
3. Is automation technically feasible under representative variation?
4. What is the simplest viable level: manual aid, fixture/poka-yoke, semi-automation, flexible robot/cobot, dedicated automation?
5. What does the full lifecycle TCO include?
6. What new failure modes, maintenance skills and recovery paths are introduced?
7. What safety and OT/cyber boundaries are introduced?
8. What FAT/SAT/SIT/production evidence is required?
9. What product/process changes trigger reassessment?
10. What exit/upgrade trigger would justify the next automation level?

## Automation qualification ladder
Requirements -> Design/Risk Review -> FAT -> Installation Verification -> SAT/SIT -> Production Qualification -> Handover -> Sustained Performance -> Change/Requalification.

This is an editorial synthesis; exact required stages vary by industry, risk and contractual/regulatory context.

## OEE editorial guardrails
Always ask: boundary, time basis, planned stops, ideal cycle basis, good-part definition, micro-stops/changeovers, constraint relevance and downstream ability to consume output.
Never teach an unsupported universal benchmark such as “85% OEE is world class” as engineering truth.

## Maintenance / reliability lens
Record expected failure modes, diagnostics, maintenance strategy, spares/lead times, technician/vendor dependence, recovery procedure, safe manual state, downtime assumptions, obsolescence/software support and backup/restore/change control.

## Human / automation allocation lens
Do not frame the choice as “human versus robot.” Allocate work by:
- variability and judgment;
- precision/repeatability;
- hazardous/ergonomic exposure;
- change frequency;
- sensing/handling complexity;
- recovery complexity;
- training and skill availability;
- economics and required rate.

Semi-automation can be the production-optimal architecture when it removes the critical loss while retaining human adaptability.

## DEV / LVP / SVP lens
### DEV
Automate for learning/test/data/safety where useful; favor reversible tooling and avoid freezing product architecture around premature dedicated automation.

### LVP
Prefer selective semi-automation where repetitive labor, ergonomics, CTQ control or test/data benefits justify it while preserving flexibility for product/process change.

### SVP
Evaluate dedicated automation using sustained volume, process stability, capability, uptime, maintenance, changeover, support, safety, lifecycle and full TCO/ROI; qualify production performance under representative conditions.

## Myth register
- “If a robot can do it, we should automate it.” — FALSE/OVERBROAD.
- “Automation ROI = labor saved / machine cost.” — INCOMPLETE.
- “FAT passed, therefore the line is production ready.” — FALSE/OVERBROAD.
- “SAT passed, therefore production validation is complete.” — FALSE/CONTEXT DEPENDENT.
- “A cobot/robot is safe, therefore the application is safe.” — FALSE/OVERBROAD.
- “High OEE means the factory is profitable.” — FALSE/OVERBROAD.
- “Maximum machine utilization is always desirable.” — FALSE/OVERBROAD.
- “Full automation is always more advanced than semi-automation.” — FALSE/OVERBROAD.
- “Predictive maintenance is always better than preventive maintenance.” — NOT SUPPORTED; economics/context required.

## Breadth result
A7 now has authoritative/source-backed coverage for:
- FAT/SAT/SIT boundaries;
- maintenance economics and strategy;
- OEE context/guardrails;
- industrial robot versus application/cell safety;
- task-based human-robot safety;
- deployment constraints including expertise, integration and recovery;
- lifecycle automation decision dimensions;
- DEV/LVP/SVP automation strategy.

Remaining detail belongs to Pass 2 rather than blocking breadth closure.

## Pass-2 targets
- automation ROI/TCO worked example with sensitivity analysis;
- manual vs fixture vs semi-automated vs robot vs dedicated-cell comparison;
- direct premature-automation industrial case;
- FAT/SAT/SIT/production-qualification checklist;
- ISO 22400/OEE definition extraction and decomposition case;
- bottleneck/local-utilization/WIP example;
- maintenance/recovery case;
- product-change requalification case;
- ISO 10218/ISO 12100/IEC 60204 applicability map;
- human-robot collaboration case.

## Readiness
Source map: BREADTH COMPLETE
Critical claims identified: YES
Primary-source backbone: YES
Applicability conflicts visible: YES
Pass-2 depth targets: YES
Podcast Ready: NO