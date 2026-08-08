# 8.9 OEE, Maintenance & Spares

status: Researching
provenance: [GNR]

## OEE objects
- planned production time
- availability
- performance
- quality
- ideal cycle-time basis
- downtime taxonomy
- microstops boundary
- speed loss
- rejects/rework boundary

## Engineering principle
OEE is a loss-accounting framework, not a standalone proof of capacity, profitability or process capability. Definitions and counting rules must be explicit before comparing machines, lines or sites.

## Maintenance objects
- preventive maintenance
- predictive/condition monitoring boundary
- corrective maintenance
- calibration/verification
- cleaning/lubrication
- wear-part replacement
- backup/restore
- software/configuration backup
- maintenance access
- mean-time metrics boundary

## Spare-parts objects
- critical spare
- consumable/wear part
- lead time
- failure impact
- commonality
- shelf life/storage
- repairable spare
- obsolescence
- vendor dependency

## Questions
1. Which failures stop the constraint versus a noncritical resource?
2. Does maintenance restore the qualified state, and how is that verified?
3. Are software/robot/PLC/vision configurations backed up and revision controlled?
4. Which spare has low purchase cost but catastrophic lead-time risk?
5. Are chronic microstops hidden by broad downtime categories?
6. Is ideal cycle time physically demonstrated and sustainable?

## Decision objects
### D-AUTO-OEE-001 — OEE/counting architecture and loss taxonomy
### D-AUTO-PM-001 — Maintenance strategy by failure mode/criticality
### D-AUTO-SPARE-001 — Critical-spares strategy
### D-AUTO-RESTORE-001 — Post-maintenance verification/requalification requirement

## Cross-links
OEE <-> capacity/bottleneck
Maintenance <-> qualification
Spares <-> supply-chain resilience
Downtime <-> Data Hub
Maintenance <-> safety

No universal OEE target, PM interval or spare-stock level is asserted.