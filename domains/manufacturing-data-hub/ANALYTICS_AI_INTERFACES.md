# 9.14 Dashboards, Analytics & AI Interfaces

status: Researching
provenance: [GNR]

## Purpose
Expose manufacturing data and engineering knowledge for monitoring, analysis and decision support while preserving semantics, lineage, uncertainty and human decision boundaries.

## Interface layers
### Operational dashboards
- current production state
- WIP/throughput
- yield/FPY/RTY
- downtime/OEE losses
- quality holds/NCR
- bottlenecks
- material/supplier status

### Engineering analytics
- parameter-to-quality relationships
- defect Pareto and creation/detection points
- capability/SPC trends
- genealogy comparison
- process revision comparison
- supplier/process/site comparison
- reliability/failure analysis

### Decision-support interfaces
- query Atlas alternatives
- retrieve applicable claims/standards/evidence
- instantiate decision models
- compare options/tradeoffs
- expose assumptions/open questions/conflicts
- return evidence maturity and applicability

### AI interfaces
AI may retrieve, summarize, compare, classify, detect anomalies, generate hypotheses and populate structured decision inputs. AI output must retain provenance and must not silently become authoritative master data or approved engineering disposition.

## Semantic query pattern
User question -> intent/decision context -> semantic objects -> authoritative operational data + Knowledge OS evidence -> transformations/analytics -> result with lineage/uncertainty -> human/system action boundary.

## Analytics lineage
Every derived KPI/model output should retain where applicable:
- source objects/events
- source system
- time window
- filters/exclusions
- transformation/formula/model
- version
- units
- aggregation
- confidence/uncertainty boundary

## Decision objects
### D-DH-DASH-001 — Which operational decision should this dashboard support?
### D-DH-KPI-001 — Is KPI definition semantically stable and traceable to raw data?
### D-DH-AI-001 — What may AI recommend versus execute/write authoritatively?
### D-DH-MODEL-001 — What validation/change control applies to an analytical/AI model?

## Anti-patterns
- dashboard metrics with different hidden definitions
- AI reading only current master data for historical failure analysis
- correlation presented as causal engineering conclusion
- derived KPI without formula/version lineage
- autonomous write-back to controlled engineering data without defined authority
- model retraining/change without validation/effectivity

## Integrity rule
AI should increase access to evidence and decisions, not erase the distinction between evidence, inference and approval.