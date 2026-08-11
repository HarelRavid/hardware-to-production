# Automation Business Case / Qualification / OEE — Evidence Source Map

status: IN PROGRESS — FAT/SAT/MAINTENANCE/OEE BACKBONE CAPTURED
campaign: A7
maps_to: MASTER_WBS Section 8; PODCAST_MAP Episodes 41–46
provenance: primary-source-first

## Purpose
Build the evidence backbone for deciding when automation creates value, how automated equipment/processes should be qualified, and how OEE/maintenance/reliability data should be interpreted without confusing high equipment utilization with good manufacturing economics.

## Primary / authoritative backbone captured

### ISA-105 / ANSI-ISA-62381 / IEC 62381 — FAT, SAT and SIT
ISA describes ANSI/ISA-62381-2026 / IEC 62381:2024 as a structured methodology for Factory Acceptance Test, Site Acceptance Test and Site Integration Test of automation systems in process industries. The framework includes pre-test planning, execution/readiness, punch lists/completion criteria, documentation, hardware/software, operator interfaces, communications and roles across owner/vendor/contractor.

Engineering use:
- FAT verifies agreed automation-system requirements before field deployment where applicable;
- SAT verifies the installed system/site context;
- SIT addresses integration in the site environment;
- these tests should be planned against requirements and explicit acceptance criteria rather than treated as demonstrations.

Important applicability boundary:
ISA explicitly notes that FAT/SAT/SIT do not by themselves cover all subsequent activities such as loop checks, commissioning or MES testing. Regulated industries may require additional qualification/validation frameworks.

### NIST AMS 100-18 — Costs and Benefits of Advanced Maintenance in Manufacturing
NIST frames maintenance strategy as an economic/manufacturing-performance problem and identifies the need to estimate costs, losses and data requirements associated with maintenance approaches.

Engineering use:
- automation economics must include maintenance and downtime exposure;
- maintenance strategy should be part of lifecycle business-case assumptions;
- predictive/preventive/reactive approaches have different data and economic implications.

### NIST — Manufacturing Machinery Maintenance / maintenance strategy research
NIST distinguishes predictive/condition-based, preventive/scheduled and reactive/run-to-failure maintenance and emphasizes the connection between manufacturing complexity, equipment health information, reliability and downtime.

Engineering use:
- maintenance architecture is a design input to automation, not an afterthought;
- monitoring/diagnostics can support reliability, but value depends on actionable decisions and process/equipment context.

### NIST / ISO 22400 reference — OEE and asset-performance measurement
NIST manufacturing research explicitly references ISO 22400 for asset-performance metrics and studies the impact of machine OEE in manufacturing environments.

Engineering use:
- OEE belongs to a defined manufacturing-performance measurement context;
- OEE can support loss diagnosis and asset-performance analysis;
- OEE alone is not evidence of profitability, system throughput, customer service or optimal capital allocation.

## Source families still to deepen
### NIST manufacturing automation / robotics / digital manufacturing research
Use for automation feasibility, interoperability, system performance and deployment constraints.

### ISO 10218 / ISO/TS 15066 and machinery safety families where applicable
Use for industrial robot/cobot safety boundaries, risk assessment and safeguarding concepts.
Applicability: specific machine/robot context required.

### IEC 60204-1 / ISO 12100 / relevant machinery safety architecture
Use for machine electrical/safety and risk-reduction boundaries.
Applicability: standards mapping reserved for Pass 2.

### OEE / TPM authoritative sources
Need deeper Pass-2 clause/definition work around Availability x Performance x Quality and loss categorization. Avoid unsourced universal benchmark claims.

## Initial decision dimensions
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
status: STRONG ENGINEERING DIRECTION
Business decision must also consider demand, process stability, flexibility, integration, maintenance, support, downtime, lifecycle and TCO.

### C-AUTO-002 — Automating an unstable or poorly understood process can preserve or amplify existing losses
status: HIGH PRIORITY SYNTHESIS
Need stronger primary Lean/automation case evidence before Podcast Ready. Do not present slogan as universal law.

### C-AUTO-003 — Automation business cases should include lifecycle costs beyond direct labor savings
status: STRONG DIRECTION
NIST maintenance economics supports inclusion of maintenance/downtime; Pass 2 should add integration/tooling/spares/obsolescence cases.

### C-AUTO-004 — FAT, SAT/SIT and production qualification answer different acceptance questions
status: STRONG / APPLICABILITY-SCOPED
ISA-62381 provides the FAT/SAT/SIT backbone. Production qualification/validation remains industry/context dependent and must not be collapsed into SAT.

### C-AUTO-005 — OEE is an equipment/manufacturing-performance metric, not equivalent to profitability or customer value
status: STRONG DIRECTION
NIST/ISO 22400 context supports asset-performance use. Need precise OEE formula/definitions in Pass 2.

### C-AUTO-006 — High local utilization can worsen system flow when it is disconnected from system constraints
status: STRONG SYNTHESIS from A5
Need operations/automation case corroboration.

### C-AUTO-007 — Automated systems require explicit failure/recovery and maintenance strategies
status: STRONG DIRECTION
NIST maintenance research supports reliability/downtime importance; machinery safety evidence still required.

### C-AUTO-008 — Product/configuration change can invalidate automation qualification or economics
status: STRONG SYNTHESIS
Need change/requalification cases.

### C-AUTO-009 — FAT pass does not prove installed-site performance
status: STRONG
The existence of distinct FAT, SAT and SIT stages in ISA-62381 supports this boundary.

### C-AUTO-010 — SAT pass does not universally equal production-process qualification
status: STRONG / APPLICABILITY-SCOPED
ISA explicitly bounds FAT/SAT/SIT scope; regulated/industry-specific validation may add further requirements.

## Automation qualification ladder
1. Requirements defined — what must the cell/system do and under what conditions?
2. Design/risk review — architecture, interfaces, safety and failure modes understood.
3. FAT — vendor/factory-context requirements tested where applicable.
4. Installation/site verification — physical/configuration/interface state confirmed.
5. SAT/SIT — installed behavior and integrations tested.
6. Production qualification — representative product/process/rate/quality evidence demonstrated under applicable framework.
7. Handover — documentation, training, spares, maintenance and ownership established.
8. Sustained performance — losses, downtime, quality, rate and maintenance monitored.
9. Change/requalification — product, software, tooling, equipment or process changes assessed for validation impact.

This ladder is an editorial synthesis; exact required stages vary by industry, risk and contractual/regulatory context.

## OEE editorial guardrails
Do not teach OEE as a magic factory score.
Ask:
- What is the equipment/system boundary?
- What time basis is included/excluded?
- How are planned stops treated?
- How is ideal cycle time defined?
- What counts as a good part?
- Does the equipment constrain system throughput?
- Are micro-stops and changeovers visible?
- Is high OEE creating WIP because downstream cannot consume output?

Never use an unsupported universal statement such as “85% OEE is world class” as engineering truth without source, context and applicability.

## Maintenance / reliability lens
Automation business cases should explicitly record:
- expected failure modes;
- detection/diagnostics;
- preventive/predictive/reactive strategy;
- spare-parts strategy and lead times;
- technician skills and vendor dependence;
- recovery procedure and safe manual state;
- planned/unplanned downtime assumptions;
- obsolescence/software support;
- change-control and backup/restore capability.

MTBF/MTTR are useful only when definitions, censoring/time basis, failure boundary and data quality are clear. Pass-2 evidence required before detailed reliability teaching.

## DEV / LVP / SVP lens
### DEV
Automate mainly for learning/test/data/safety where useful. Favor reversible tooling and avoid freezing product architecture around premature automation.

### LVP
Use selective semi-automation where repetitive labor, ergonomics, CTQ control or test/data benefits justify it while preserving flexibility for product/process change. Acceptance should include maintainability and recovery, not only nominal cycle demonstration.

### SVP
Evaluate dedicated automation using sustained volume, process stability, capability, uptime, maintenance, changeover, support, lifecycle and full TCO/ROI; qualify equipment and production performance under representative conditions.

## Myth register
- “If a robot can do it, we should automate it.” — NOT SUPPORTED.
- “Automation ROI = labor saved / machine cost.” — INCOMPLETE.
- “FAT passed, therefore the line is production ready.” — FALSE/OVERBROAD.
- “SAT passed, therefore production validation is complete.” — FALSE/CONTEXT DEPENDENT.
- “High OEE means the factory is profitable.” — FALSE/OVERBROAD.
- “Maximum machine utilization is always desirable.” — FALSE/OVERBROAD.
- “Predictive maintenance is always better than preventive maintenance.” — NOT SUPPORTED; economics/context required.

## Breadth gaps remaining
1. primary automation ROI/TCO cases and decision frameworks;
2. process-maturity prerequisite / automation-too-early case evidence;
3. precise OEE definition/decomposition and ISO 22400 applicability;
4. machinery/robotics safety applicability;
5. human/automation work allocation and recovery modes;
6. product/configuration change and requalification evidence;
7. strong automation case studies for Episodes 41–46.

## Pass-2 targets
- automation ROI worked example;
- manual vs semi-automated vs dedicated-cell comparison;
- FAT/SAT/SIT/production-qualification checklist;
- OEE decomposition case showing misleading aggregate values;
- bottleneck/local-utilization example;
- maintenance/recovery case;
- product-change requalification case;
- machinery-safety applicability map.

## Readiness
Source map: IN PROGRESS
Critical claims identified: YES
Primary-source backbone: FAT/SAT + maintenance + OEE context captured
Applicability conflicts visible: YES
Podcast Ready: NO