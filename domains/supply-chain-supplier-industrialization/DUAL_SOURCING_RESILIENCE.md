# 7.8 Dual Sourcing & Supply Resilience

status: Researching
provenance: [GNR]

## Scope
Design supply resilience without assuming that nominally equivalent suppliers or parts are technically interchangeable.

## Resilience objects
- single-source dependency
- dual/multi-source strategy
- approved alternate
- geographic concentration
- sub-tier concentration
- tooling ownership/duplication
- lead time
- inventory buffer
- safety stock boundary
- capacity reserve
- logistics route
- business continuity
- disaster recovery
- geopolitical/export/regulatory boundary

## Technical equivalence objects
- drawing/specification equivalence
- material/source equivalence
- process route equivalence
- special-process equivalence
- tooling equivalence
- measurement/test equivalence
- functional interchangeability
- qualification status

## Engineering principle
Two suppliers producing the same drawing do not automatically produce equivalent process histories, capability, reliability or change risk. Resilience requires qualified alternatives, not merely additional vendor names.

## Questions
1. Is the real single point of failure the Tier-1 supplier or a shared sub-tier/raw-material source?
2. Does the alternate require product/process requalification?
3. Is duplicated tooling actually independent, or does it depend on the same equipment/supplier?
4. How much inventory buys meaningful recovery time?
5. Is the alternate's capacity available when the primary supplier is disrupted?
6. Can specifications tolerate alternate manufacturing processes without changing function/reliability?

## Decision objects
### D-SUP-DUAL-001 — Single, dual or multi-source strategy
### D-SUP-ALT-001 — Qualification scope for alternate supplier/process
### D-SUP-BUF-001 — Inventory/capacity buffer strategy
### D-SUP-BCP-001 — Business-continuity and recovery evidence

## Integrity rule
A purchase-approved alternate is not necessarily an engineering-qualified alternate.