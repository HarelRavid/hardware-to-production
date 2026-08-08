# 3.11.6 Feedstock, Qualification & Build Traceability

status: Researching
provenance: [GNR]

## Feedstock objects
### Powder
- chemistry
- particle-size distribution
- morphology
- flowability
- apparent/tap density boundary
- moisture/oxygen/contamination
- virgin/reused/blended state
- sieving/conditioning
- storage/handling

### Filament/pellet/resin/wire/binder feedstock
- lot
- moisture/conditioning
- viscosity/rheology boundary
- diameter/dimensional consistency
- storage life
- exposure/out-time where applicable
- contamination

## Qualification layers
- material/feedstock qualification
- machine qualification
- parameter-set qualification
- build/process qualification
- operator authorization where applicable
- post-process qualification
- inspection-method qualification
- part/application qualification

## Build genealogy
Part/serial -> build ID -> machine -> software/build file revision -> parameter set -> feedstock lots/reuse history -> build plate/location/orientation -> atmosphere/process logs -> operator -> post-processing -> machining -> inspection/test records.

## Process monitoring objects
- chamber temperature
- oxygen/inert atmosphere
- laser/beam/process energy signals
- layer imaging
- melt-pool monitoring boundary
- recoater/spreader events
- powder-bed imaging
- extrusion pressure/temperature boundary
- machine alarms

## Decision objects
### D-AM-QUAL-001 — What must be qualified for this application?
### D-AM-TRACE-001 — Required genealogy depth
### D-AM-REUSE-001 — Is feedstock reuse permitted and under what validated controls?
### D-AM-MON-001 — Which in-process signals have validated quality meaning?

## Integrity rule
Collecting process data is not equivalent to demonstrating that the data predicts part quality. Correlation/acceptance claims require validation.