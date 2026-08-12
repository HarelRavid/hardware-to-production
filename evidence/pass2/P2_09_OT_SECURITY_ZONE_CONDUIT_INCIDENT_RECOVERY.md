# P2.09 — OT Security Zone/Conduit + Cyber→Quality Incident + Recovery Model

Status: ACTIVE — WORKED EXAMPLE
Provenance: [SRC/GNR]. ISA/IEC 62443 family mapping is source-backed at family/part-title level; detailed normative clauses/security-level claims require licensed primary-source verification before Podcast Ready. NIST SP 800-82 Rev.3 provides public OT-security guidance.

## Purpose

Turn OT cybersecurity from a generic firewall discussion into a manufacturing-control problem tied to production truth, product quality, recovery and configuration management.

Canonical chain:

Production function → consequence → zone → permitted conduit → identity/authority → controlled change → detection → containment → recovery → product/evidence reconciliation → requalification

## Sentinel Factory — zone model

### Z1 — Enterprise IT
Examples: corporate identity, business applications, email, office endpoints.

Manufacturing principle: no assumed direct trust into cell-control assets.

### Z2 — Manufacturing Operations / Atlas
Examples: work-order dispatch, genealogy/data services, production dashboards, controlled interfaces to ERP/QMS.

Critical claims: production identity, routing/effectivity, result association and manufacturing records must remain trustworthy.

### Z3 — Engineering / Maintenance
Examples: engineering workstation, PLC/robot programming tools, approved recipe/configuration repository, maintenance tooling.

High consequence: authorized users here may be able to alter the physical process.

### Z4 — Production Cell
Examples: PLC, HMI, robot/motion controller, insertion station, local sensors/actuators.

Primary objective: safe, deterministic, controlled execution of the approved manufacturing process.

### Z5 — Test / Quality
Examples: functional-test station, measurement acquisition, quality-result services.

Critical issue: test data is product-release evidence, not merely telemetry.

### Z6 — Safety-related boundary
Safety functions and safety-related control assets are treated according to the actual machinery/safety architecture. Cybersecurity design must not casually assume that a network control is equivalent to a safety function.

### Z7 — Vendor remote-access boundary
No persistent implicit trust. Vendor access is a controlled conduit with explicit authorization and logging.

## Conduit matrix

| From | To | Business/manufacturing purpose | Default posture | Key evidence |
|---|---|---|---|---|
| Z1 Enterprise | Z2 Manufacturing | orders/master-data/reporting | only required flows | interface inventory + logs |
| Z2 Manufacturing | Z4 Cell | dispatch approved job/recipe reference; collect execution status | constrained, authenticated | message/transaction trace |
| Z4 Cell | Z5 Test | unit identity/state handoff where required | constrained | serial association |
| Z5 Test | Z2 Manufacturing | results/release evidence | authenticated/integrity protected | test-result genealogy |
| Z3 Engineering | Z4 Cell | approved engineering/maintenance change | normally restricted; controlled elevation | change ticket + version diff + approval |
| Z7 Vendor | Z3/Z4 as approved | time-bound support | deny by default; brokered/time-limited | identity + session/change log |
| Z1 Enterprise | Z4 Cell | none in baseline architecture | prohibited unless explicitly justified | architecture exception |

NIST SP 800-82 Rev.3 describes segmentation/zoning as a common defense-in-depth architecture and recommends using mapped data flows to determine required communications between segments and enforce restrictions.

## IEC 62443 part-role map — source packaging target

Do not treat the series as one checklist.

- 62443-2-1 — security program requirements for IACS asset owners. Verify current edition/status before final claims.
- 62443-2-4 — security program requirements for IACS service providers/integration/maintenance context. Verify current adopted edition.
- 62443-3-2 — security risk assessment for system design; official ISA listing identifies this part specifically for system-design risk assessment.
- 62443-3-3 — system security requirements and security levels.
- 62443-4-1 — secure product development lifecycle requirements.
- 62443-4-2 — technical security requirements for IACS components.

Podcast guardrail: asset owner, integrator/service provider, system and component/product responsibilities are related but not interchangeable.

## Worked incident — silent recipe manipulation

### Normal approved process

Connector insertion recipe RCP-INS-07 Rev D:
- controlled force/displacement window;
- seating acceptance logic;
- approved product applicability;
- results linked to serial genealogy.

### Cyber/configuration event

A remote maintenance session is opened for troubleshooting. A privileged engineering account modifies an insertion acceptance threshold. The cell continues running. No obvious outage occurs.

This is intentionally more dangerous pedagogically than ransomware: production remains green while process truth has changed.

### Immediate manufacturing consequences

Potential chain:

Unauthorized threshold change
→ acceptance window no longer equals approved process
→ marginal connector seating can be accepted
→ latent product defect risk
→ final-test escape may or may not detect it
→ affected WIP/finished-goods population must be reconstructed
→ existing process-capability/qualification evidence may no longer apply.

### Detection sources

Useful evidence can include:
- PLC/recipe configuration checksum/version mismatch;
- engineering workstation/session log;
- remote-access log;
- unexpected parameter change event;
- CTQ distribution shift;
- quality escape/rework trend;
- Atlas as-run configuration mismatch against released definition.

No single signal is assumed sufficient in all implementations.

## Cyber→Quality containment workflow

1. Put the affected cell/process in controlled state.
2. Preserve volatile and configuration evidence as practicable.
3. Identify last-known-good configuration/time.
4. Identify first-known-bad or uncertainty boundary.
5. Query genealogy for all units processed in the uncertainty window.
6. Segregate WIP, finished goods and potentially shipped population according to risk.
7. Restore/verify approved process configuration.
8. Determine product reinspection/retest/rework/disposition strategy.
9. Run first-good-piece/process verification before unrestricted restart.
10. Reconcile Atlas/as-run records where cyber event compromised data trust.
11. Update NCR/CAPA/change/security records without rewriting history.
12. Close containment only when product and process evidence support release.

Key principle:

> An OT cyber incident can invalidate manufacturing evidence even when no machine is visibly damaged.

## Population reconstruction example

Assume:
- last verified recipe hash: 09:42;
- unauthorized session begins: 09:47;
- discrepancy detected: 12:18;
- configuration history cannot prove exact modification timestamp more narrowly.

The conservative uncertainty window is therefore based on defensible evidence, not operator memory.

Atlas query target:

All serials whose OP30 connector-insertion execution occurred during the uncertainty window on Cell INS-01, plus any units whose execution/configuration identity cannot be proven.

The containment population is then narrowed only with evidence.

## Backup ≠ Recovery qualification

### What backup proves
A copy exists.

### What recovery must prove
- correct asset/configuration can be restored;
- restore media/repository is accessible during incident conditions;
- compatible hardware/software/tooling exists;
- identity/keys/certificates/licenses are recoverable where needed;
- process configuration is verified against approved baseline;
- Atlas/genealogy/test data are reconciled;
- WIP state is known or conservatively dispositioned;
- safety and quality checks required for restart are completed;
- production can return inside the approved envelope.

## Recovery test — Sentinel Cell

Scenario: engineering workstation and PLC project repository are unavailable/corrupted while the physical cell remains intact.

Qualification test records:
1. recovery initiation authority;
2. source of trusted backup;
3. restored PLC/HMI/robot/recipe versions;
4. checksum/version comparison;
5. communication/interface verification;
6. safety-function verification as required by the machine safety architecture;
7. dry-cycle/controlled functional checks;
8. first-piece CTQ verification;
9. functional test;
10. genealogy/event reconciliation;
11. time to controlled production recovery;
12. unresolved assumptions/deviations.

A successful restore of software files without steps 3–10 is not a demonstrated manufacturing recovery.

## Vendor remote-access qualification test

Test the access path rather than merely documenting a policy.

Inject/verify:
- unapproved vendor identity → denied;
- approved identity outside authorization window → denied;
- approved session → only approved target/resources accessible;
- privilege escalation outside scope → blocked/detected;
- session start/stop and operator approval recorded;
- file/configuration transfer traceable;
- configuration modification generates manufacturing change evidence;
- connection terminates at expiry;
- emergency revocation works;
- post-session configuration reconciliation performed.

## Security Level guardrail

Do not infer an IEC 62443 Security Level from:
- number of firewalls;
- network segmentation alone;
- use of MFA;
- vendor marketing;
- a generic cyber maturity score.

62443-3-2 and 3-3 concepts must be applied using their actual normative definitions and risk/system context. Detailed SL-T/SL-C/SL-A terminology and foundational-requirement mapping are deferred to licensed-source verification.

## OT SECURITY RELEASE 10

Before releasing a connected manufacturing architecture, ask:

1. Which production/safety/quality functions can cyber compromise affect?
2. Are assets and trust boundaries identified?
3. Are required data flows mapped?
4. Are zones/conduits justified by function and consequence?
5. Are identities/privileges appropriate to the physical consequence?
6. Is remote/vendor access controlled and tested?
7. Are configuration changes detectable and tied to manufacturing change control?
8. Can incidents be translated into affected-product/WIP populations?
9. Has recovery been demonstrated, not merely backup configured?
10. Which claims remain unsupported and who owns the residual risk?

## Cross-links to existing Pass-2 packages

P2.02 Configuration & Change Control:
cyber-authorized or unauthorized configuration changes affect released/as-run truth and effectivity.

P2.03 Quality:
process manipulation can shift CTQs, invalidate capability evidence or create escapes.

P2.04 Capacity/Ramp:
security controls/recovery architecture must preserve realistic availability and restart behavior.

P2.06 Supplier Industrialization:
OEM/integrator/vendor access and component/product security responsibilities must be contractually and technically understood.

P2.07 Automation:
connected machine qualification includes fault/recovery/configuration behavior; cyber controls do not replace machinery safety engineering.

P2.08 Manufacturing Atlas:
genealogy and as-run configuration are essential to cyber-driven product containment.

## Remaining P2.09 closure work

1. Build the canonical IEC 62443 responsibility/applicability matrix with verified editions/status.
2. Build OT Security Release Gate packaging from this worked example.
3. Verify primary-source language for 62443 parts and avoid unsupported normative detail.
4. Package NIST SP 800-82 Rev.3 public-source anchors for segmentation, remote access, incident response and recovery.
5. Final claim/evidence audit and maturity status.

Recommended current status: ACTIVE — advanced worked example complete; not yet Near Podcast Ready.
