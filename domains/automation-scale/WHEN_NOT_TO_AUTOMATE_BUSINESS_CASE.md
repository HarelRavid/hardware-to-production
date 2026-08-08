# 8.1–8.2 When Not to Automate & Automation Business Case

status: Researching
provenance: [GNR]

## Warning conditions before automation
- unstable process parameters
- frequent engineering changes
- poorly understood defect mechanisms
- high product mix / low repeatability
- immature tooling/fixtures
- weak incoming-material consistency
- inadequate measurement system
- undefined Standard Work
- automation would hide quality problems
- missing maintenance/technical support capability

## Business-case objects
- baseline labor content
- takt/capacity requirement
- scrap/rework
- ergonomics/safety risk
- quality variation
- floor space
- utilities
- CapEx
- integration/NRE
- commissioning/qualification
- maintenance
- spares
- software/licensing
- training
- downtime risk
- product-change flexibility
- residual/manual labor

## Benefits beyond labor reduction
- repeatability
- traceability/data capture
- safety
- ergonomics
- controlled process timing/force
- improved inspection coverage
- capacity
- contamination control
- consistency across shifts

## Engineering principle
The automation business case must compare total lifecycle economics and risk against an improved manual/semi-automated baseline, not against an intentionally inefficient current state.

## Decision objects
### D-AUTO-NOT-001 — Which process instability must be solved before automation?
### D-AUTO-BC-001 — Automation business case
### D-AUTO-LEVEL-001 — Assistive, semi-automatic or full automation?
### D-AUTO-FLEX-001 — Required flexibility for product/volume change

## Integrity rule
Do not justify automation solely by direct labor savings without including support, downtime, maintenance, qualification, product-change and failure costs.