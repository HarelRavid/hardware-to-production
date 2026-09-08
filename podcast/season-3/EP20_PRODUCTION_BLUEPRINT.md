# Episode 20 Production Blueprint — From EBOM to MBOM and Process Flow

status: PRODUCTION BLUEPRINT COMPLETE
season: Season 3 — Build the Factory Before You Need the Factory
lifecycle: LVP → Production Validation → Ramp

## Listener transformation
Before: sees the engineering BOM as the product definition needed by production.
After: understands how the released product definition must be translated into a manufacturing structure, routings, subassemblies, consumables and executable process flow.

## Narrative hook
Engineering releases a clean EBOM. Production still asks: which subassembly is built first, where adhesive belongs, when firmware is loaded, what packaging/consumables are needed, and which station owns each operation? The BOM is correct, but the production system is undefined.

## Teaching flow
1. EBOM purpose versus MBOM purpose.
2. Manufacturing decomposition: subassemblies, kits, consumables and phantom structures.
3. Build sequence and routing.
4. Operation ownership, input/output state and CTQs.
5. Link MBOM/routing to configuration/effectivity.
6. Alternate routes, rework and controlled deviations.
7. Sentinel product example from engineering structure to first LVP route.
8. Close with process-flow review before tooling/WI investment.

## Core framework — Product-to-Process Translation Map
`Released product definition → manufacturing breakdown → operation sequence → material/consumable inputs → equipment/tooling → CTQ/test → output state → traceability → next operation`.

## DEV/LVP/SVP
DEV: lightweight build notes may be enough if identity is preserved. LVP: explicit MBOM/routing and operation sequence become necessary. SVP: routings, effectivity, alternates, rework and execution records must remain controlled at scale.

## Common mistakes
- copying EBOM directly into production;
- hiding consumables/adhesives/labels/programming from the MBOM;
- sequencing operations without considering datum/state changes;
- letting rework create undocumented alternate routes;
- changing routing without effectivity review.

## Source/evidence backlog
ISA-95/IEC 62264 and MES/ERP object definitions require exact applicability if cited normatively. Internal translation framework remains synthesis.

## Closing handoff
Episode 20 defines what production must execute. Episode 21 asks what tooling and equipment are needed to execute it repeatedly.
