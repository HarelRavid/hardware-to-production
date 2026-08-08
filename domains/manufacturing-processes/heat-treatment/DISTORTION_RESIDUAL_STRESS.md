# 3.14.5 Distortion, Residual Stress & Dimensional Control

status: Researching
provenance: [GNR]

## Objects
- residual stress
- thermal gradient
- phase-transformation strain boundary
- quench distortion
- warpage
- bow/twist
- ovality
- dimensional growth/shrinkage
- stress relief
- fixture restraint
- machining stress redistribution
- straightening/rework

## Engineering chain
Material history + geometry + machining/forming stress + heating uniformity + phase change + cooling/quench gradients + fixture restraint -> residual stress/distortion -> final dimensional capability.

## DFM questions
1. Which dimensions/datums are most sensitive to heat-treatment distortion?
2. Should critical surfaces be finish-machined after thermal processing?
3. Can section transitions be redesigned to reduce thermal response differences?
4. Does fixturing reduce distortion or merely move/create residual stress?
5. Is straightening permitted, controlled and requalified?
6. Should distortion be modeled statistically from production data rather than handled by a fixed machining allowance?

## Decision objects
### D-HT-DIST-001 — Distortion-control strategy
### D-HT-ALLOW-001 — Pre-heat-treatment machining allowance strategy
### D-HT-STRAIGHT-001 — Straighten/rework or reject?

## Cross-links
Distortion <-> GD&T
Residual stress <-> fatigue
Machining <-> stress redistribution
Quench <-> distortion/cracking
Fixtures <-> dimensional repeatability

No universal distortion allowance is asserted.