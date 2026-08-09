# 9.6 Parameter & Measurement Model

status: Researching
provenance: [GNR]

## Purpose
Represent process parameters, setpoints, actual values, measurements, test results and derived metrics with enough context to support genealogy, process analysis, quality decisions and evidence-backed engineering conclusions.

## Parameter objects
- Parameter Definition
- Parameter Unit
- Parameter Role: setpoint / limit / actual / calculated / recipe input / environmental boundary
- Parameter Value
- Source Device/System
- Timestamp
- Operation Execution
- Recipe Revision
- Equipment Asset
- Quality/validity flag

## Measurement objects
- Characteristic / measurand
- Measurement Definition
- Measurement Method
- Measurement System
- Instrument/Gauge/Sensor
- Fixture/setup
- Measurement Result
- Unit
- uncertainty/MSA boundary
- operator/automation
- environmental condition
- timestamp
- acceptance result boundary

## Test objects
Test Definition -> Test Recipe Revision -> Test Execution -> Raw Observations -> Calculated Metrics -> Acceptance Decision.

## Critical distinctions
- setpoint != actual process value
- machine-displayed value != independently verified part condition
- raw observation != derived KPI
- engineering specification limit != statistical control limit
- measurement result != pass/fail decision
- parameter definition != recipe instance

## Provenance for derived values
Every derived metric should retain:
- source observations
- algorithm/formula/version
- unit conversion
- filtering/aggregation window
- software/model revision
- timestamp of calculation

## Data-quality dimensions
- valid/invalid
- missing
- substituted
- out-of-range
- sensor fault
- manually entered
- estimated/inferred
- late-arriving/backfilled

## Engineering principle
A number without units, time, source, context and semantic meaning is not reliable manufacturing evidence.

## Decision objects
### D-DH-PARAM-001 — Which process parameters require execution-level genealogy?
### D-DH-MEAS-001 — What context is required to interpret a measurement result correctly?
### D-DH-DER-001 — Which derived metrics require reproducible lineage back to raw observations?

## Cross-links
Parameter <-> Recipe Revision
Measurement <-> MSA
Measurement Result <-> Quality Gate
Sensor <-> Equipment Asset
Derived Metric <-> Analytics/AI
Observation <-> Claim/Evidence boundary

## Integrity rule
Do not overwrite raw data with cleaned/derived data; preserve lineage and transformation history.