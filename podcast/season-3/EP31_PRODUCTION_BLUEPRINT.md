# Episode 31 Production Blueprint — Engineering Changes During Ramp-Up

status: PRODUCTION BLUEPRINT COMPLETE
season: Season 3 — Build the Factory Before You Need the Factory
lifecycle: Ramp → SVP

## Listener transformation
Before: thinks an engineering change is mainly a revised CAD/BOM/document package.
After: understands change as a controlled transition across product, process, supplier, tooling, test, documentation, WIP, field/service and evidence populations.

## Narrative hook
A connector is changed during ramp. Engineering updates the BOM, but old stock, open WIP, fixture geometry, test limits and supplier purchase orders remain mixed. Weeks later failures cannot be tied confidently to old or new configuration.

## Teaching flow
1. Change reason and affected claims.
2. ECO/ECN concepts without assuming one universal workflow.
3. Effectivity: date/serial/lot/build/order boundaries.
4. Disposition of existing stock, WIP and finished goods.
5. Supplier/CM communication and acknowledgements.
6. Tooling, WI, software, test and measurement updates.
7. Verification/revalidation after change.
8. Traceability of mixed populations and deviations.
9. Emergency change versus controlled permanent release.
10. Effectiveness review after implementation.

## Core framework — Change Effectivity Map
`Change reason → affected requirements/interfaces → product definition → process/tooling/test/WI/supplier impacts → inventory/WIP disposition → effectivity boundary → verification evidence → release communication → population monitoring → effectiveness`.

## DEV/LVP/SVP
DEV: changes are frequent; lightweight records may suffice if builds remain reconstructable. LVP: effectivity becomes essential as several units and suppliers coexist. Ramp/SVP: uncontrolled change can invalidate capability, compliance and customer evidence across large populations.

## Common mistakes
- updating BOM but not tooling/test/WI;
- date-only effectivity when WIP spans dates;
- mixed stock with no serial/lot boundary;
- supplier substitution treated as purchasing-only event;
- skipping revalidation because the change seems minor;
- emergency deviation becoming permanent silently.

## Source/evidence backlog
Configuration-management and sector change-control standards require exact applicability. Customer/regulatory notification requirements are product/industry dependent.

## Season closing
The listener now has a production system that can be defined, piloted, validated, ramped and changed without losing the evidence chain. Season 4 moves into sustained quality, compliance, traceability and supplier resilience at scale.
