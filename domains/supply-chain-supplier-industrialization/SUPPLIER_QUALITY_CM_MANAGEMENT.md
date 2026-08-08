# 7.6–7.7 Supplier Quality & Contract Manufacturer Management

status: Researching
provenance: [GNR]

## Supplier-quality objects
- approved supplier
- approved site/process scope
- supplier quality agreement
- incoming defect history
- process audit
- capability evidence
- special-process approval
- SCAR/CAPA
- deviation/concession
- change notification
- supplier scorecard
- escalation status

## Contract-manufacturer objects
- manufacturing scope
- supplied-by-customer vs supplied-by-CM materials
- ownership of tooling/fixtures/test equipment
- approved sub-tier suppliers
- MBOM/routing ownership
- WI/process specification ownership
- test/calibration ownership
- quality release authority
- change-control authority
- data/traceability interface
- intellectual-property/configuration boundaries

## Engineering principle
Outsourcing manufacturing does not outsource product/process responsibility. The technical and quality interfaces must remain explicit even when the supplier owns day-to-day execution.

## Questions
1. Which process variables/specifications are controlled by us versus by the supplier?
2. Can the supplier change a sub-tier, material, tool, recipe, software or site without approval?
3. Who owns root cause and containment when a defect is discovered?
4. Is supplier process data available at the granularity required for genealogy and investigation?
5. Are quality metrics normalized for mix, volume and severity?
6. Does the supplier quality agreement define notification and approval triggers?

## Decision objects
### D-SUP-QA-001 — Supplier-control depth by risk/criticality
### D-SUP-CM-001 — Responsibility matrix for CM-managed production
### D-SUP-AUD-001 — Audit/oversight frequency and scope
### D-SUP-SCAR-001 — Escalation and corrective-action path

## Cross-links
Supplier quality <-> incoming inspection
CM management <-> MBOM/routing
Supplier change <-> qualification
Supplier metrics <-> ramp readiness
Supplier data <-> Manufacturing Data Hub

## Integrity rule
Supplier scorecards are indicators, not substitutes for understanding the failure mechanism and process capability behind the score.