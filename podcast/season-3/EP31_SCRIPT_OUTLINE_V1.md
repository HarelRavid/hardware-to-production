# EP31 Script Outline V1 — Engineering Changes During Ramp-Up

status: SCRIPT OUTLINE COMPLETE
season: Season 3 — Build the Factory Before You Need the Factory
audience: engineering / NPI / manufacturing / quality / supply chain
lifecycle: Ramp → SVP
source_lock: evidence/source-lock/wave-03/W3_EP26_EP27_EP28_EP29_EP30_EP31_CLAIM_LOCK.md
technical_review: evidence/source-lock/wave-03/W3_INTERNAL_TECHNICAL_REVIEW.md
blueprint: podcast/season-3/EP31_PRODUCTION_BLUEPRINT.md

## Listener promise
Turn an engineering change during ramp into a controlled population transition across product, process, suppliers, WIP, tooling, test and evidence.

## Cold open
[ILLUSTRATIVE] Engineering releases a new connector BOM. Old stock, open WIP, fixture geometry, test limits and supplier POs remain mixed. Later field failures cannot be tied cleanly to old or new state.

## Beat 1 — Change reason and affected claims
Claims: EP31-C01
Dependency: Wave 01.

## Beat 2 — Product definition is only one layer
Map process/tooling/WI/software/test/supplier/inventory impacts.

## Beat 3 — Effectivity chooses the population
Claims: EP31-C02
Guard: date can be valid if it reconstructs the population; use serial/lot/order/build when needed.

## Beat 4 — Inventory and WIP disposition
Claims: EP31-C03
Old/new/mixed/rework/return states must be explicit.

## Beat 5 — Re-verification scope
Claims: EP31-C04
Dependency-based targeted evidence; neither full-retest reflex nor no-retest assumption.

## Beat 6 — Emergency change
Claims: EP31-C05
Fast change can be controlled: scope, approval, expiration, effectivity, evidence and closure.

## Beat 7 — Supplier and CM cut-in
Acknowledgement, tooling/material/test readiness, old PO/WIP handling.

## Beat 8 — Post-cut-in effectiveness
Claims: EP31-C06
Monitor quality/yield/capacity/field signals for old vs new populations.

## Listener tool — Change Effectivity Map
reason → affected requirements/interfaces → product/process/tool/test/supplier → inventory/WIP → effectivity → verification → communication → monitoring/effectiveness.

## Misconceptions
- ECO = document update only;
- release date always proves effectivity;
- minor-looking supplier substitution needs no impact review;
- emergency means uncontrolled;
- change is closed at release, before implementation evidence.

## Closing action
For your last engineering change, try to identify the first unit definitely new and the last unit definitely old. If you cannot, the change is not fully reconstructable.

## Season close
Season 3 ends with a production system that can be defined, piloted, validated, ramped and changed without losing its evidence chain.