# Episode 52 Production Blueprint — Manufacturing Data Engineers Can Actually Use

status: PRODUCTION BLUEPRINT COMPLETE
season: Season 5 — Automation, Data and the Connected Factory
lifecycle: LVP → SVP → FIELD
maps_to: MASTER_WBS 9.13, 9.14, 9.15

## Listener transformation
Before: equates more connected tags, dashboards and stored data with better manufacturing insight.
After: defines decision-grade manufacturing datasets with configuration, genealogy, units, measurement context, quality state and provenance — while treating OT/ICS security, availability and recovery as production requirements.

## Narrative hook
A data lake contains millions of machine samples, but an engineer cannot compare two failed units because recipe revisions, calibration state and rework history are missing. A new analytics connector is then installed directly into the production network and creates an availability/security concern. The factory has data, but not yet engineering-grade data architecture.

## Teaching flow
1. Start from engineering decisions/questions, not available tags.
2. Minimum context: product/configuration, operation, unit/lot, time, equipment and recipe.
3. Units, sampling, state and measurement-system identity.
4. Quality/disposition/rework context and accepted outcome.
5. Supplier/material and maintenance/configuration context where causal decisions require them.
6. Data completeness, latency and provenance fit the decision consequence.
7. Derived features/AI outputs never replace raw evidence lineage.
8. Manufacturing connectivity changes the attack/availability surface.
9. OT principles: safety/availability/integrity, segmentation, least privilege, controlled remote access, asset/configuration awareness, backup/recovery and monitored change.
10. Cyber/configuration incidents can invalidate manufacturing evidence; recovery means restoring trustworthy configuration, WIP/genealogy, quality and release evidence — not merely restarting machines.

## Core framework — Engineering-Grade Manufacturing Dataset
`Decision/question → product/config → unit/lot → operation → equipment/fixture → recipe/software → parameter + unit/time → measurement-system context → quality/rework/disposition → material/supplier → maintenance/change → provenance → security/access → retention/recovery`.

## Listener tools
- Engineering Data Fitness Check: identity, context, units, timing, genealogy, provenance, completeness, measurement adequacy and decision consequence.
- SECURITY 12 / Secure Data Path Review: asset, trust boundary, data direction, least privilege, remote access, credential/identity, segmentation, monitoring, change, backup, recovery, evidence impact.

## DEV / LVP / SVP
DEV: small exports/scripts are fine when context is preserved and production control is not exposed casually. LVP: stable identifiers, provenance and controlled interfaces become necessary. SVP: governed data pipelines, role/access control, OT-aware architecture, monitoring and tested recovery must protect both production and evidence integrity.

## Common mistakes
- collecting everything and defining context later;
- timestamps/units/calibration assumed rather than recorded;
- AI model output stored without input/model/version lineage;
- enterprise/cloud connector granted broad direct OT access for convenience;
- IT security patterns copied into OT without availability/safety consequence analysis;
- machine restart treated as full recovery after cyber/configuration event;
- analytics dashboard becoming a competing source of release truth.

## Standards/source architecture
Priority source families include ISA/IEC 62443 and NIST OT security guidance, plus applicable enterprise-control/data standards. Exact parts, revisions and normative claims remain source/edition/applicability gated. Security architecture must be site/system/risk specific; the episode does not prescribe one universal network topology.

## Season closing
Season 5 ends with an automated and connected production system whose data remains linked to physical configuration, execution and evidence, and whose connectivity is designed not to compromise production safety, availability or integrity. Season 6 can now use the full operating system through cases and decision playbooks.
