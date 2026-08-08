# 5.8–5.9 Supplier Readiness & Engineering Changes During Ramp

status: Researching
provenance: [GNR]

## Supplier-readiness dimensions
- drawing/specification clarity
- process capability
- tooling readiness
- capacity
- lead time
- raw-material availability
- sub-tier dependency
- inspection/test capability
- MSA
- quality history
- change control
- traceability
- packaging/logistics
- business continuity

## Supplier evidence objects
- sample/FAI/approval evidence boundary
- capability data
- control plan/PFMEA boundary
- process flow
- special-process approval
- material certificates
- measurement evidence
- capacity evidence
- open deviations/actions

## Engineering-change objects during ramp
- design revision
- BOM change
- supplier/material change
- tooling change
- routing/process change
- parameter/recipe change
- WI/test/software change
- temporary deviation
- cut-in/effectivity
- WIP disposition
- validation impact

## Engineering principle
Ramp is often when the product changes fastest and evidence is easiest to invalidate. Configuration control therefore becomes more important during ramp, not less.

## Questions
1. Which units/lots were built before and after the change?
2. What happens to WIP and inventory at the cut-in point?
3. Does the change invalidate prior pilot/validation/capability evidence?
4. Has the supplier implemented the same revision/effectivity?
5. Are temporary deviations becoming an undocumented alternate process?
6. Does a supplier have demonstrated capacity at required yield, not only quoted capacity?

## Decision objects
### D-RAMP-SUP-001 — Supplier readiness status
### D-RAMP-CAPSUP-001 — Is supplier capacity demonstrated at required quality/yield?
### D-RAMP-CHG-001 — Change impact and revalidation scope
### D-RAMP-CUTIN-001 — Change cut-in/effectivity and WIP disposition
### D-RAMP-DEV-002 — Temporary deviation control and expiry

## Cross-links
Supplier readiness <-> Section 7
Ramp change <-> PLM/configuration management
Change <-> MBOM/routing/WI/control plan
Supplier change <-> qualification
Effectivity <-> genealogy

## Integrity rule
A supplier's stated or nameplate capacity is not equivalent to demonstrated good-output capacity.