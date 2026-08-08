# 8.7 End-of-Line Systems

status: Researching
provenance: [GNR]

## Scope
Integrated production stations that combine final functional verification, calibration/configuration, safety checks, data capture, product identification and release/disposition logic.

## EOL objects
- unit/serial identification
- product variant/configuration
- fixture/interface
- test sequence
- stimulus/load
- sensor/measurement
- calibration/configuration write
- firmware/software verification boundary
- safety/interlock test
- leak/pressure/electrical/functional test boundary
- raw data
- calculated result
- acceptance limits
- disposition
- label/marking
- genealogy/release record

## Engineering principle
EOL should confirm defined release requirements and capture evidence; it should not become a universal repair station that hides unstable upstream manufacturing processes.

## Questions
1. Which requirements truly need EOL verification versus earlier process control?
2. Can EOL diagnose likely creation point rather than only detect final failure?
3. Are repeated test/adjust cycles visible in FPY and genealogy?
4. Are fixture, instrument, software and test-recipe revisions controlled?
5. Can the station safely handle wrong variant, failed communication or interrupted sequence?
6. What happens when the EOL system itself is later found out of tolerance?

## Decision objects
### D-AUTO-EOL-001 — EOL test/calibration architecture
### D-AUTO-EOLCOV-001 — Requirement/failure-mode coverage map
### D-AUTO-EOLR-001 — Automated release versus human review boundary
### D-AUTO-EOLREC-001 — Raw data and genealogy retention

## Cross-links
EOL <-> Production Test & Calibration
EOL <-> PFMEA/control plan
EOL <-> MSA
EOL <-> traceability
EOL <-> ramp/yield

No universal EOL test coverage percentage is asserted.