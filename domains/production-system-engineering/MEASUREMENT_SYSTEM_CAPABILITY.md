# 4.9 Measurement-System Capability

status: Researching
provenance: [GNR]

## Scope
Determine whether the measurement/test system is capable of supporting the manufacturing decision being made, rather than assuming calibration alone proves measurement adequacy.

## Measurement-system objects
- measurand
- specification/tolerance
- resolution/discrimination
- accuracy/bias
- repeatability
- reproducibility
- stability
- linearity boundary
- uncertainty
- operator
- fixture/setup
- environment
- method
- software/data reduction
- reference standard

## Study families
- gauge R&R boundary
- bias study
- linearity study
- stability study
- attribute agreement boundary
- test-system repeatability
- destructive measurement strategy
- measurement uncertainty analysis

## Engineering principle
Calibration answers whether an instrument agrees with a reference under defined conditions. MSA asks whether the complete measurement process — instrument, method, fixture, operator, environment and analysis — is capable of making the intended production decision.

## Questions
1. Is resolution adequate relative to the tolerance/process variation?
2. Does part fixturing dominate measurement variation?
3. Are operators measuring the same feature in the same way?
4. Is the measurement stable across temperature/time/location?
5. Is the characteristic inherently difficult/destructive to measure?
6. Can measurement noise create false rejects or false accepts?
7. Does automated measurement eliminate operator variation but introduce algorithm/setup variation?

## Decision objects
### D-PSE-MSA-001 — Required MSA method
### D-PSE-GAUGE-001 — Select measurement technology/gauge
### D-PSE-FIXMSA-001 — Is a dedicated measurement fixture required?
### D-PSE-UNC-001 — Is formal uncertainty evaluation required for this decision/application?

## Cross-links
MSA <-> control plan
MSA <-> SPC/capability
MSA <-> test/calibration
MSA <-> inspection fixture
MSA <-> supplier quality
MSA <-> acceptance/rejection risk

## Integrity rule
A calibrated gauge can still be an incapable measurement system.