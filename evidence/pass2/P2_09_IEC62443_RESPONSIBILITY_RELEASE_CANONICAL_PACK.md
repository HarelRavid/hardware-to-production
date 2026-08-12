# P2.09 — IEC 62443 Responsibility Matrix + OT Security Release Gate

Status: NEAR PODCAST READY
Provenance: primary ISA/ISAGCA role/series structure checked 2026-08-12; exact normative clauses still require licensed-standard verification before Podcast Ready.

## Purpose

Close P2.09 by connecting OT cybersecurity to accountable lifecycle roles, system evidence, production release, recovery, configuration control and product-quality risk.

Canonical chain:

Business/production function → consequence → system under consideration → zones/conduits → risk → required capabilities → role responsibility → implementation → verification → controlled operation → monitoring/change → recovery/requalification

## 1. Shared responsibility is not shared ambiguity

ISA/IEC 62443 treats IACS cybersecurity as a lifecycle problem involving multiple principal roles. For the Sentinel manufacturing system we use four practical responsibility buckets:

1. Asset Owner — accountable for the operating IACS and equipment under control.
2. Integration Service Provider — designs, integrates, configures, tests, commissions and hands over the automation solution; may assist with zones/conduits and risk assessment.
3. Maintenance/Service Provider — supports the automation solution during operation.
4. Product Supplier — develops and supports hardware/software products used in the solution.

A single company may perform more than one role. The role model exists to make responsibilities explicit, not to force four separate companies.

## 2. Core IEC 62443 applicability map

### 62443-2-1 — Asset-owner security program

Primary question:
How does the organization establish and sustain the OT/IACS security program governing its operating environment?

Sentinel relevance:
- governance and responsibilities;
- asset-owner operational security processes;
- lifecycle security management;
- policy/procedure framework for the operating IACS.

Current ISA listing checked: ANSI/ISA-62443-2-1-2024.

### 62443-2-4 — Security program requirements for IACS service providers

Primary question:
What security processes/capabilities are expected from organizations providing integration or maintenance services to the asset owner?

Sentinel relevance:
- machine integrator practices;
- vendor/maintenance support;
- remote service behavior;
- secure configuration/maintenance responsibilities.

Current ISA listing checked: ANSI/ISA-62443-2-4-2018 / IEC 62443-2-4:2015+AMD1:2017 CSV.

### 62443-3-2 — Security risk assessment for system design

Primary question:
How is the system under consideration assessed and partitioned so cyber risk can be treated systematically?

Sentinel relevance:
- system under consideration;
- zones and conduits;
- consequence/risk assessment;
- target security requirements/levels as supported by the normative method.

Current ISA listing checked: ANSI/ISA-62443-3-2-2020.

### 62443-3-3 — System security requirements and security levels

Primary question:
What technical security requirements/capabilities must the IACS system provide at system level?

Sentinel relevance:
- technical system requirements;
- security capabilities across the integrated automation solution;
- system-level verification rather than component-label inference.

Current ISA listing checked: ANSI/ISA-62443-3-3-2013.

### 62443-4-1 — Secure product development lifecycle

Primary question:
How does a product supplier develop and support secure IACS products through a defined security lifecycle?

Sentinel relevance:
- PLC/HMI/industrial software/vendor product development practices;
- vulnerability handling and updates;
- security lifecycle evidence from product suppliers.

Current ISA listing checked: ANSI/ISA-62443-4-1-2018.

### 62443-4-2 — Technical security requirements for IACS components

Primary question:
What security capabilities are required at component level?

Sentinel relevance:
- embedded devices;
- host devices;
- network devices;
- software applications used in the IACS.

Current ISA listing checked: ANSI/ISA-62443-4-2-2018.

## 3. Responsibility × evidence matrix

| Security lifecycle activity | Asset Owner | Integrator / Service Provider | Product Supplier | Sentinel evidence |
|---|---|---|---|---|
| Define business/production consequences | A/R | C | I | consequence register |
| Define system boundary | A | R/C | C | system-under-consideration diagram |
| Zone/conduit partition | A | R/C | C | zone/conduit model + flow matrix |
| Risk assessment | A | R/C | C | risk assessment + assumptions |
| Select system security requirements | A | R/C | C | security requirement specification |
| Product/component capability evidence | C | C | A/R | supplier docs/certificates/test evidence |
| Secure integration/configuration | A | A/R for delivered work | C | baseline configs + verification |
| Remote-access design | A | R/C | C | access architecture + test records |
| Operational identity/access governance | A/R | R within contracted scope | C | accounts/roles/approvals/logs |
| Patch/update decision | A | R/C | R for product guidance/update | compatibility/risk/change record |
| Backup/recovery capability | A | R/C | C/support | restore test + recovery evidence |
| Vulnerability response | A for site response | R/C | R for product vulnerability process | incident/vulnerability records |
| Configuration change control | A | R within scope | C | approved change/effectivity/history |
| Cyber→quality containment | A/R | C | C | genealogy + WIP containment record |
| Requalification after relevant change | A | R/C | C | targeted verification/release record |

A = accountable, R = responsible, C = consulted, I = informed. This RACI is a Sentinel implementation framework, not a normative IEC 62443 table.

## 4. Sentinel OT Security Release Gate — SECURE RELEASE 12

Before releasing a connected production system, ask:

1. SYSTEM — What exact IACS/system is inside the release boundary?
2. CONSEQUENCE — What can cyber failure/manipulation do to safety, quality, availability, environment, equipment and genealogy?
3. INVENTORY — Do we know the relevant hardware/software/network identities and versions?
4. FLOWS — Are required communications mapped and unnecessary paths constrained?
5. ZONES — Are assets grouped and conduits controlled based on function/risk rather than diagram aesthetics?
6. IDENTITY — Are human, service and machine identities/privileges appropriate and reviewable?
7. REMOTE — Is vendor access individually attributable, approved, bounded, logged and revocable?
8. CONFIGURATION — Can we detect/reconstruct changes to PLC/HMI/robot/recipe/network/security configuration?
9. QUALITY — Can a cyber/configuration event invalidate CTQ/test/release evidence, and can affected product be found?
10. RECOVERY — Have restore/restart/reconciliation/first-good-piece behaviors actually been tested?
11. SUPPLY — Do integrator/service/product suppliers provide the security evidence and lifecycle support their role requires?
12. CHANGE — Which patches, replacements, upgrades, network changes or remote actions trigger risk review/reverification/requalification?

## 5. Release outcomes

GREEN — security architecture and operational controls support release inside the demonstrated configuration and operating envelope.

AMBER — conditional release with explicit compensating control/containment, owner, expiry/stop condition and closure evidence.

RED — release unsupported because a critical risk/control/evidence dependency is unresolved.

Hard stops cannot be averaged away by a weighted score. Examples:
- unknown or uncontrolled remote access capable of modifying production logic;
- inability to identify the approved PLC/robot/recipe configuration;
- inability to identify affected product after a potentially quality-relevant cyber/configuration event;
- recovery path not capable of restoring controlled operation;
- critical safety/security dependency unresolved.

## 6. Security Level guardrail

Do not say “the factory is SL2/SL3” as shorthand without showing:
- the relevant system/zone/conduit context;
- the risk-assessment method;
- whether the statement concerns target, capability or achieved security level terminology;
- which requirements were assessed;
- evidence and scope.

Security Level is not a generic maturity score and not a marketing adjective.

## 7. Cyber → Quality worked decision

Scenario:
A vendor remote session changes the connector insertion acceptance threshold.

Required response chain:

Remote-session evidence
→ detect configuration difference
→ determine change timestamp/effectivity
→ identify work orders/serials processed under changed state
→ contain affected WIP/finished goods
→ assess CTQ/test evidence validity
→ restore approved configuration
→ verify configuration and security controls
→ targeted process/quality requalification
→ first-good-piece/release
→ corrective action on remote/change governance.

Key principle:

> A cyber event that can change the manufacturing process can also invalidate manufacturing evidence.

## 8. Recovery qualification

A backup file is evidence that data/configuration was copied. It is not evidence that production can be recovered.

Recovery qualification should demonstrate, as applicable:
- restore of approved PLC/HMI/robot/recipe versions;
- account/credential/security configuration restoration;
- communications and interface validation;
- safety-function checks affected by recovery/change;
- calibration/measurement/test readiness;
- genealogy/database reconciliation;
- WIP disposition;
- first-good-piece or targeted requalification;
- recovery time and required skills/resources;
- documented deviations and release authority.

## 9. DEV / LVP / SVP security evolution

### DEV — avoid unmanaged future debt

Minimum useful controls:
- know connected assets and owners;
- separate engineering/admin access where practical;
- preserve source/configuration history;
- avoid shared permanent vendor credentials;
- maintain recoverable backups;
- document remote access and major configuration changes.

Goal: do not build a prototype architecture that becomes impossible to govern when production starts.

### LVP — controlled production security

Add:
- formal asset/configuration baseline;
- mapped flows and segmentation;
- controlled vendor access;
- patch/vulnerability/change workflow;
- tested recovery;
- cyber→quality containment logic;
- production-relevant logging and accountability.

Goal: preserve safe, trustworthy and recoverable manufacturing while the system is changing rapidly.

### SVP — scalable lifecycle security

Add/scale:
- mature asset-owner security program;
- supplier/service-provider requirements;
- repeatable risk assessment and architecture governance;
- vulnerability/patch lifecycle at fleet scale;
- centralized monitoring appropriate to OT;
- tested incident/recovery exercises;
- auditable identities/configurations/changes;
- integration with enterprise security without violating OT safety/availability constraints.

Goal: scale security governance with the production system, supplier ecosystem and installed automation base.

## 10. Listener framework — SECURITY 12

Function → Consequence → Boundary → Zone → Flow → Identity → Remote → Configuration → Quality → Recovery → Supplier → Change.

If a team can answer these twelve with evidence, it has moved beyond “we put the PLC behind a firewall.”

## 11. Canonical P2.09 message

OT cybersecurity is manufacturing engineering because it can change:
- whether the machine is available;
- whether the machine is safe;
- what process the machine actually executes;
- whether measurements/tests can be trusted;
- whether genealogy is complete;
- whether production evidence remains valid;
- whether the plant can recover into a controlled state.

## 12. Completion assessment

P2.09 now contains:
- OT-vs-IT framing;
- Sentinel zone/conduit architecture;
- flow matrix;
- vendor remote-access qualification logic;
- cyber→quality incident;
- WIP containment/effectivity logic;
- backup-vs-recovery qualification;
- IEC 62443 core-part applicability map;
- role/responsibility matrix;
- SECURITY 12;
- SECURE RELEASE 12;
- DEV/LVP/SVP evolution;
- release outcomes and hard stops.

Remaining before PODCAST READY:
1. licensed/primary normative clause verification for claims that cite IEC/ISA 62443 requirements;
2. current-edition/status check at episode packaging time;
3. technical cybersecurity review;
4. jurisdiction-specific legal/regulatory overlay where an episode makes legal claims;
5. episode source notes and provenance conversion from remaining GNR synthesis.

Recommended status: NEAR PODCAST READY.
