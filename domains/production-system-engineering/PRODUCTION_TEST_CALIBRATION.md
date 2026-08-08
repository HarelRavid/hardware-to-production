# 4.8 Production Test & Calibration

status: Researching
provenance: [GNR]

## Scope
Design of production tests and calibration operations that verify or establish product function at appropriate points in the routing with controlled limits, equipment, software, traceability and reaction plans.

## Test families
- incoming verification boundary
- in-process functional test
- leak/pressure test
- electrical test
- sensor/actuator test
- dimensional/force/torque functional test boundary
- calibration
- end-of-line test
- burn-in/run-in boundary
- safety/interlock test
- software/firmware verification boundary

## Test-system objects
- requirement being tested
- test method
- stimulus
- response
- acceptance limits
- guard band boundary
- fixture/interface
- instrument
- reference standard
- software/version
- environmental condition
- sequence
- cycle time
- raw data
- result/disposition
- operator/automation

## Calibration objects
- as-found state
- adjustment
- as-left state
- reference/standard
- calibration coefficients
- serial-specific parameters
- software/configuration write-back
- verification after adjustment

## Engineering principle
A production test is valuable only if it has a defined relationship to the requirement/failure mode it is intended to detect or calibrate. Testing everything at end-of-line is not a substitute for controlling upstream processes.

## Questions
1. What failure mechanism or requirement does each test cover?
2. Is the test performed early enough to avoid expensive late discovery?
3. Can the test itself damage or alter the product?
4. Are test limits engineering requirements or historically chosen numbers?
5. Are test fixtures/software/instruments revision controlled?
6. What happens to previously accepted product if the test system is later found out of tolerance?

## Decision objects
### D-PSE-TEST-001 — Test location in routing
### D-PSE-LIMIT-001 — Acceptance/test-limit architecture
### D-PSE-CAL-001 — Calibration versus verification-only strategy
### D-PSE-DATA-001 — Which raw test/calibration data must be retained?

## Genealogy
Unit/serial -> test station -> fixture -> instrument/reference -> software revision -> test recipe -> raw data -> calculated result -> calibration coefficients where applicable -> operator/time -> disposition.

## Cross-links
Production test <-> DFT
Test <-> PFMEA/control plan
Calibration <-> traceability
Test equipment <-> MSA
EOL <-> ramp/yield
Test data <-> failure analysis

No universal test coverage percentage or guard-band rule is asserted.