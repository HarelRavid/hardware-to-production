# Episode 47 Production Blueprint — What PLM, ERP, MES, QMS, SCADA and Historians Actually Do

status: PRODUCTION BLUEPRINT COMPLETE
season: Season 5 — Automation, Data and the Connected Factory
lifecycle: LVP → SVP
maps_to: MASTER_WBS 9.11

## Listener transformation
Before: treats PLM, ERP, MES, QMS, SCADA and historian as overlapping software categories to be selected by feature lists.
After: maps information responsibilities and system-of-record boundaries so definition, transactions, execution, quality and machine history remain distinct but traceably linked.

## Narrative hook
A factory has the BOM in PLM, another BOM in ERP, work instructions in shared folders, recipes in machines and quality dispositions in email. Every system is “correct” locally, but nobody can reconstruct which definition actually built a unit. Digitalization created more truth, not better truth.

## Teaching flow
1. Start from information objects and decisions, not software brands.
2. PLM: product definition/configuration/change context.
3. ERP: commercial/material/resource transactions and planning context.
4. MES/MOM: manufacturing execution, routing, dispatch, WIP and production records where implemented.
5. QMS: quality events, controls, audit/nonconformance/CAPA context.
6. SCADA/HMI/control systems: operational supervision/control context.
7. Historians: time-series process/equipment history.
8. Ownership versus replication/caching: one authoritative identity per decision context.
9. Interfaces, identifiers and effectivity across systems.
10. Avoid tool-first architecture and define minimal viable digital thread.

## Core framework — Manufacturing System-of-Record Map
`Information object → authoritative owner → consuming systems → identifier → revision/effectivity → interface → latency/availability need → evidence retained → fallback/recovery`.

## Listener tools
- System-of-Record Map.
- Competing-Truth Audit: product revision, routing, recipe, quality status, unit genealogy, material lot and machine configuration.

## DEV / LVP / SVP
DEV: lightweight tools can work if identity/configuration is preserved. LVP: system boundaries and identifiers must become explicit. SVP: authoritative ownership, interfaces, access/change control, availability and recovery need production-grade evidence.

## Common mistakes
- ERP or MES declared master of everything;
- duplicate BOMs/recipes without effectivity rules;
- spreadsheet shadow systems hidden from architecture;
- machine-local recipe treated as detached from product configuration;
- data integration attempted before object ownership is defined.

## Source/evidence backlog
Vendor definitions are not architectural authority. ISA-95 and other references may support functional boundaries but exact edition/scope must be verified; implementation remains organization-specific.

## Closing handoff
Episode 48 uses these system boundaries to build the digital thread around the actual product population: genealogy, recipes, parameters and measurements.
