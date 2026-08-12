# P2.09 — OT/ICS Cybersecurity Architecture Worked Example

Status: ACTIVE — FOUNDATION CAPTURED
Provenance: primary-source-backed concepts plus [GNR] implementation synthesis. Exact IEC/ISA 62443 editions, normative requirements, clauses and jurisdictional obligations require source-level verification before Podcast Ready.

## Purpose

Build OT/ICS cybersecurity as part of the manufacturing system architecture rather than as a generic IT-security appendix.

Sentinel Node manufacturing environment is used as the worked example so cybersecurity connects directly to the Manufacturing Atlas, automation cell, PLC/control layer, quality data, supplier/service access and change control developed in P2.01–P2.08.

Canonical principle:

> OT cybersecurity protects the ability to operate the physical process safely, reliably and as intended — not only the confidentiality of information.

NIST SP 800-82 Rev. 3 explicitly frames OT security around unique performance, reliability and safety requirements. ISA describes ISA/IEC 62443 as a lifecycle-oriented IACS cybersecurity series spanning people, process and technology and multiple stakeholder roles.

## 1. Why ordinary IT thinking is insufficient

A manufacturing environment contains cyber-physical consequences.

A compromised office document may create confidentiality or business loss.

A compromised manufacturing recipe, PLC program, robot coordinate, safety-related configuration, calibration parameter or genealogy record can also create:
- unsafe motion or process state;
- damaged tooling/equipment;
- hidden product defects;
- false quality acceptance;
- production stoppage;
- corrupted traceability;
- inability to recover confidently;
- incorrect release decisions.

Therefore the manufacturing security model must explicitly preserve:
- safety;
- availability/recoverability;
- integrity of control and manufacturing truth;
- authorized operation/change;
- traceability/accountability;
- appropriate confidentiality.

## 2. Sentinel manufacturing architecture

Illustrative environment:

Enterprise/IT:
- identity/email/collaboration;
- engineering repositories;
- ERP/business systems;
- cloud services.

Manufacturing operations / site services:
- Manufacturing Atlas/MES-like execution service;
- QMS records;
- historian/analytics;
- engineering workstation services;
- patch/update repositories;
- backup services.

Cell/OT:
- insertion cell PLC/controller;
- robot/servo/actuator controller where applicable;
- HMI;
- vision/force/displacement sensors;
- calibration/test station;
- local industrial network;
- safety system interfaces;
- barcode/serial readers.

External:
- machine OEM remote support;
- integrator/service provider;
- component/product supplier portals;
- cloud analytics or support services where approved.

The security question is not simply “is the factory network behind a firewall?” It is:

> Which assets and functions must communicate, why, under whose authority, through which controlled path, and what happens if that communication is unavailable or malicious?

## 3. Roles and shared responsibility

ISA/IEC 62443 uses role-specific responsibility across the IACS lifecycle. For this project, keep at least these conceptual roles visible:

### Asset Owner
Owns/operates the manufacturing system and accepts operational risk.

Typical responsibilities include governance, risk decisions, architecture requirements, access policy, operation, monitoring, incident/recovery expectations and supplier requirements.

### System Integrator / Service Provider
Designs, integrates, commissions, maintains or supports the solution.

Security-relevant question:
- can the integrator alter PLC/robot/HMI/network configuration?
- how is that access authorized, logged and removed?

### Product Supplier
Provides PLCs, robots, industrial PCs, software or other IACS components/products.

Security-relevant questions include product capabilities, secure development/support, vulnerability handling and update mechanisms.

Guardrail:

> Buying a “62443-certified” component does not automatically make the manufacturing system secure or compliant.

System architecture, configuration, operation, integration and lifecycle controls remain essential.

## 4. Zones and conduits — worked architecture

ISA/IEC 62443 uses security zones and conduits as core concepts in risk-based system partitioning. NIST SP 800-82 similarly recommends segmentation/isolation architectures based on mapped required communications, while considering operational performance, safety and response capability.

Illustrative Sentinel zones:

### Z1 — Enterprise IT Zone
Contains corporate user services and general business systems.

Trust assumption:
- not trusted to initiate arbitrary control-layer communication.

### Z2 — Manufacturing Operations Zone
Contains Atlas/MES-like services, approved production scheduling/execution interfaces and manufacturing data services.

Purpose:
- bridge business intent and controlled manufacturing execution without exposing cell controllers directly to enterprise clients.

### Z3 — Engineering / Maintenance Zone
Contains authorized engineering tools used to configure or maintain PLC/robot/HMI/test equipment.

Higher-risk capability:
- users here may be able to change executable/configuration state.

Therefore access must not be treated like ordinary production viewing access.

### Z4 — Production Cell Zone
Contains PLC/controller, HMI, cell devices, industrial I/O and process equipment for connector insertion.

### Z5 — Test / Quality Equipment Zone
Contains calibration/functional-test equipment and measurement interfaces where separation is justified by architecture/risk.

### Z6 — Safety-Critical Function Boundary
Where safety-related control functions exist, their architecture and independence/dependencies must be understood. Cybersecurity controls must not undermine required safety behavior.

This is a conceptual boundary; exact implementation depends on safety architecture and risk assessment.

### Z7 — Vendor Remote Access Boundary
Remote support does not receive implicit direct membership in the cell zone.

Access path should be explicitly mediated and controlled.

## 5. Conduits — communications are claims

Every allowed conduit should answer:
1. source zone;
2. destination zone;
3. business/operational purpose;
4. protocol/service;
5. direction;
6. initiating identity/system;
7. authorization condition;
8. monitoring/logging;
9. failure behavior;
10. owner.

Example:

Atlas → Cell conduit
- purpose: deliver approved work order/recipe identifier;
- direction: controlled manufacturing service to cell execution interface;
- forbidden behavior: arbitrary PLC programming through the production execution path;
- failure behavior: cell must not silently substitute an unknown recipe;
- evidence: transaction/audit log + recipe/configuration identity.

Cell → Atlas conduit
- purpose: return serial, operation result, process parameters and execution status;
- failure behavior: loss of connection must not create untraceable product; offline/hold/reconciliation behavior must be defined.

## 6. Remote access worked example

Scenario:

Machine OEM needs to diagnose intermittent insertion-cell faults.

Weak design:
- persistent vendor VPN;
- shared account;
- direct access to PLC engineering interface;
- no approval window;
- no session record;
- vendor can upload changes during production.

Controlled design intent:

Request
→ named owner approval
→ time-bounded access
→ authenticated individual identity
→ approved jump/mediation path
→ least required destination/service
→ monitored/logged session
→ production/change restrictions
→ explicit disconnect/revocation
→ review of any changes/actions
→ revalidation/release if configuration changed.

Connect to P2.02:

Remote maintenance that changes PLC/robot/HMI/recipe state is a configuration/change-control event, not merely an IT support event.

## 7. Identity and privilege

Separate at least:
- operator execution rights;
- supervisor disposition/release rights;
- quality authority;
- maintenance rights;
- engineering/programming rights;
- administrator/security rights;
- vendor/service rights.

Avoid shared engineering credentials where individual accountability is required.

Principle:

> The ability to run production is not the same permission as the ability to redefine production.

Examples:
- operator may select an approved work order;
- operator should not arbitrarily modify protected process limits;
- engineer may prepare a new recipe revision;
- release authority controls when that recipe becomes production-effective.

## 8. Secure configuration and change

Cybersecurity and configuration management overlap strongly in OT.

Security-relevant configuration includes:
- PLC/robot/HMI software versions;
- controller firmware;
- network/firewall rules;
- user/role definitions;
- remote-access configuration;
- recipes/process limits;
- certificates/keys where used;
- endpoint allowlists;
- logging configuration;
- backup/restore configuration.

Change chain:

Proposed change
→ security/production/safety impact
→ test
→ approval
→ effectivity
→ deployment
→ verification
→ rollback/recovery readiness
→ evidence update.

## 9. Patch and vulnerability management

IT logic such as “install every patch immediately” may conflict with validated OT operation, uptime or vendor support.

The alternative is NOT “never patch.”

Use risk-managed vulnerability handling:
- know assets/versions;
- receive vulnerability information;
- assess exposure and consequence;
- determine compensating controls if immediate patching is unsafe/impractical;
- test updates where needed;
- schedule deployment;
- verify function after update;
- preserve rollback/recovery path;
- document accepted residual risk.

Critical dependency:

> You cannot manage OT vulnerabilities reliably if you do not know what hardware/software/firmware is actually installed.

This directly connects P2.09 to the P2.02 configuration baseline and P2.08 Atlas.

## 10. Backup is not recovery

Backups should cover the state needed to reconstruct manufacturing capability, potentially including:
- PLC/controller programs;
- robot programs/configuration;
- HMI configuration;
- approved recipes;
- industrial PC images/configuration;
- network-device configuration;
- Atlas/MES/QMS databases and configuration;
- calibration/test configuration;
- security configuration/identity dependencies as appropriate.

But a backup file is only evidence of copying data.

Recovery readiness asks:
- can it be restored?
- to compatible hardware/software?
- by whom?
- how long does it take?
- what production/configuration state is recovered?
- how is integrity verified?
- what happens to WIP and genealogy during the outage?
- what first-good-piece/requalification is required after restoration?

Canonical line:

> A backup you have never restored is an assumption about recovery.

## 11. Availability and safe degradation

For each dependency, define failure behavior.

Examples:

Atlas unavailable:
- can cell finish current serialized unit?
- can it start another?
- where is result data buffered?
- how is reconciliation controlled?

Identity service unavailable:
- does production stop?
- is controlled cached authentication allowed?
- can engineering changes still occur?

Historian unavailable:
- does control continue?
- which evidence becomes unavailable?

Remote vendor service unavailable:
- local production should not depend unnecessarily on permanent vendor connectivity.

Security architecture must preserve the physical process's required safety and reliability characteristics.

## 12. Manufacturing integrity attack examples

### Recipe manipulation
Attacker changes insertion force limit.

Potential consequence:
- product passes automation but connector damage increases.

Controls span:
- authorization;
- version/effectivity;
- protected transfer;
- controller-side identity/check;
- audit;
- CTQ/final-test detection;
- change reconciliation.

### Genealogy manipulation
Serial/result association is altered.

Consequence:
- suspect population cannot be identified reliably.

Security consequence becomes quality/recall consequence.

### PLC program change
Unauthorized logic modifies sequence or interlock behavior.

Consequence may span safety, equipment damage, quality and downtime.

### Ransomware in manufacturing operations
Atlas/MES-like service becomes unavailable.

Question is not only how to remove malware; manufacturing must know whether controlled production can continue, what evidence is lost, and how recovery/reconciliation occurs.

## 13. SECURITY 12 — listener tool

Before connecting a production asset, ask:

1. What physical/business function does this asset control or support?
2. What happens if its data is disclosed, altered or unavailable?
3. Which zone should it belong to and why?
4. Which communications are actually required?
5. Who can operate it?
6. Who can change it?
7. How is vendor/service access controlled?
8. How do we know its hardware/software/firmware configuration?
9. How are vulnerabilities and patches handled without destabilizing production?
10. Can we restore it and reconstruct manufacturing truth after failure?
11. Which security change could invalidate safety, quality or qualification evidence?
12. Who owns the residual risk and the evidence supporting that decision?

## 14. DEV / LVP / SVP lens

### DEV
Do not build enterprise OT bureaucracy.

Minimum discipline:
- do not expose controllers casually to the public internet;
- identify devices/software versions;
- control engineering credentials;
- preserve known-good programs/configuration;
- know which cloud/vendor dependencies exist;
- separate experimentation from released production state.

Goal: secure learning without destroying iteration speed.

### LVP
Now manufacturing continuity and product genealogy matter materially.

Add:
- defined network boundaries;
- controlled engineering/vendor access;
- role separation;
- configuration/change logging;
- backup + restore tests;
- vulnerability/patch process;
- incident/recovery procedure;
- explicit offline/degraded production behavior;
- security requirements in supplier/integrator interfaces.

### SVP
Scale creates larger attack surface and larger consequence.

Add/strengthen:
- formal OT cybersecurity program;
- asset inventory/configuration automation;
- risk-based zones/conduits;
- security monitoring/logging;
- lifecycle supplier requirements;
- tested disaster recovery;
- controlled remote support at scale;
- vulnerability intelligence/patch governance;
- periodic reassessment;
- incident exercises;
- metrics and governance.

## 15. Relationship to ISA/IEC 62443 family

High-level mapping to verify during evidence packaging:
- foundational concepts/models: 62443-1-x family;
- asset-owner security program: 62443-2-1;
- service-provider/integration security program: 62443-2-4;
- system security risk assessment/design including zones/conduits: 62443-3-2;
- system technical security requirements/security levels: 62443-3-3;
- secure product development lifecycle: 62443-4-1;
- component technical security requirements: 62443-4-2.

Guardrail:

Do not cite “IEC 62443” as if it were one universal checklist. Different parts address different roles, lifecycle activities and system/component questions.

## 16. Security level guardrail

Security Levels are not a marketing adjective and should not be assigned casually.

Before the podcast makes SL claims, source-level work must verify:
- SL concepts and variants used by the relevant parts;
- risk-assessment path to target security level(s);
- foundational requirement vectors where applicable;
- distinction between target, achieved/capability concepts as defined in the applicable edition;
- system versus component claims.

Until then, use risk-based architecture language rather than claiming “the factory is SL2/SL3.”

## 17. Hard-stop anti-patterns

RED flags:
- PLC exposed directly to Internet without justified controlled architecture;
- permanent vendor access with shared credentials;
- undocumented controller/software versions;
- production recipe changes outside change control;
- no tested restore path;
- flat network justified only by convenience;
- security appliance added without checking latency/reliability/safety effects;
- cybersecurity team unable to identify production consequence;
- OT team saying “we are isolated” without verifying actual conduits;
- certified component treated as proof of secure system;
- security event that changes manufacturing state but does not trigger product/WIP assessment.

## 18. P2.09 next work

To move from foundation to NEAR PODCAST READY:
1. build a detailed zone/conduit table for Sentinel manufacturing;
2. create one cyber-to-quality incident worked example with WIP containment/genealogy;
3. create backup/restore + remote-access qualification tests;
4. build an IEC 62443 role/part/applicability matrix with current primary-source verification;
5. build canonical OT security release/review gate;
6. cross-link to P2.02, P2.06, P2.07 and P2.08;
7. package source notes and mark unresolved normative claims.

## 19. Current maturity

P2.09 status after this artifact:

ACTIVE — architecture foundation and listener framework captured.

Not yet Podcast Ready because exact normative mapping, current editions and clause-level evidence remain to be verified.
