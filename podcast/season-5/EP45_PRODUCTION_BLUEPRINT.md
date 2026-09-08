# Episode 45 Production Blueprint — Automation Qualification, OEE and Maintenance

status: PRODUCTION BLUEPRINT COMPLETE
season: Season 5 — Automation, Data and the Connected Factory
lifecycle: Ramp → SVP
maps_to: MASTER_WBS 8.8, 8.9

## Listener transformation
Before: considers an automated cell production-ready when it completes nominal cycles at the integrator or during a short acceptance run.
After: requires evidence for intended product/process envelope, sustained accepted output, abnormal recovery, maintenance and controlled configuration.

## Narrative hook
A machine hits its quoted cycle time during FAT. On the production floor, micro-stops, sensor faults, changeovers and fixture cleaning reduce good output dramatically. OEE falls, but the number alone does not explain why. The cell was fast; the system was not ready.

## Teaching flow
1. Qualification/acceptance must reference a defined process/product envelope.
2. FAT/SAT concepts versus production-validation evidence.
3. Repeatability, quality and rate under representative material/operators/environment.
4. Abnormal states: jam, power loss, sensor fault, bad part, restart and WIP status.
5. OEE as availability × performance × quality loss lens, not root-cause proof.
6. Downtime taxonomy and loss Pareto.
7. Preventive/predictive maintenance only where failure mechanisms/data justify them.
8. Spares, wear items, calibration and software/configuration backup.
9. Recovery evidence: configuration, quality, genealogy and release after intervention.
10. Ownership and escalation model for sustaining equipment.

## Core framework — Automation Production-Readiness Pack
`Intended envelope → acceptance criteria → representative run → quality/rate evidence → abnormal/recovery cases → OEE/loss model → maintenance plan → spares/calibration → config/backup → owner/escalation → release evidence`.

## Listener tools
- Automation Production-Readiness Pack.
- LOSS 8/OEE Loss Review: classify losses before choosing countermeasures.

## Common mistakes
- FAT success = production capability;
- OEE treated as root cause or capacity proof;
- short peak rate used as sustainable throughput;
- planned stops hidden to improve a metric;
- maintenance plan copied from OEM without process criticality;
- restart after repair assumed to restore evidence automatically.

## Quantitative gate
OEE, accepted throughput, downtime and maintenance examples require explicit definitions, time bases and audited arithmetic. Comparisons must state exclusions and planned/unplanned treatment.

## Source/evidence backlog
Exact OEE definitions should use authoritative TPM/industry references when attributed. Machine acceptance, safety, validation and maintenance obligations remain sector/site/equipment specific.

## Closing handoff
Episode 46 integrates the first half of the season: before scaling automation, confirm that it is amplifying a controlled process rather than a controlled defect generator.
