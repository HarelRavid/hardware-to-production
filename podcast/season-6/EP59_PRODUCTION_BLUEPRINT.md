# Episode 59 Production Blueprint — Lessons from Industrial Equipment

status: PRODUCTION BLUEPRINT COMPLETE
season: Season 6 — Manufacturing Atlas: Decision Playbooks and Case Studies
primary_audience: industrial hardware, automation, service, operations and lifecycle engineering teams
lifecycle: SVP → INSTALLED BASE → RETROFIT / END-OF-LIFE
maps_to: MASTER_WBS 10.7 + lifecycle/change/recovery synthesis
source_basis: `EP59_CASE_EVIDENCE_PACK.md`
entry_point: YES WITH EP10 SERVICE + CHANGE 9 RECAP
technical_depth: practitioner

## Listener transformation
Before: treats fielded industrial equipment as a finished product whose later work is “maintenance” until it is finally replaced.
After: manages the installed base as a living configuration system in which obsolescence, spares, software, networking, retrofit, safety, commissioning and recovery can all change the evidence required to keep production trustworthy.

## Narrative hook
A bottling line still makes product, but its drives, PLC generation, network, HMI and engineering tools are becoming obsolete. Replacing “the old controller” quickly becomes a multi-layer production-system migration.

The opening question is:

> When a machine still runs but you can no longer reliably repair, restore or support its demonstrated configuration, is it still technically healthy?

## Teaching flow
1. CCBSA Phoenix modernization: obsolescence appears across drives, PLCs, network, HMI, diagnostics and backups — not at one component only.
2. Define obsolescence operationally: loss of ability to restore/support the demonstrated production state, not merely age.
3. Show installed-base configuration as hardware + software/firmware + network/protocol + parameters/recipes + engineering backups where those affect production/recovery.
4. Safilin retrofit: one modernization crosses mechanics, drives, HMI and safety; retrofit is CHANGE 9 applied to an installed asset.
5. Explain impact-based recommissioning: reverify affected functions, hazards, interfaces, process outputs and recovery paths — not blindly everything and not only the replacement component.
6. Use OSHA lockout/tagout modification rule as a jurisdiction-specific illustration that modifications can trigger changed safety-control obligations.
7. Use ABB lifecycle material only as support for the reality of long-lived assets and obsolescence planning, not as an industry standard.
8. Introduce EU Machinery Regulation 2023/1230 only as a date-qualified transition example; do not present its substantial-modification regime as generally applicable before the application date.
9. Close with installed-base genealogy: knowing what is installed where becomes the foundation for spares, service, safety, retrofit and requalification decisions.

## Core framework — Installed-Base Change Review
`Installed configuration → support/obsolescence risk → proposed change → affected mechanical/electrical/software/network/safety/process interfaces → site population → new obligations/applicability → migration/rollback plan → commissioning evidence → updated backups/baselines → operator/service documentation → release to production → lifecycle support ownership`.

This reuses CHANGE 9 / configuration / recovery logic; it is not a new backbone model.

## Case spine
### Case 1 — CCBSA Phoenix bottling plant
Owns: controls/network/HMI/drive obsolescence and migration as a production-system problem.
Guardrail: Siemens is the vendor source; architecture/benefit claims remain vendor/customer case material, not universal technology recommendations.

### Case 2 — Safilin spinning-machine retrofit
Owns: multi-domain retrofit impact across mechanics, motion/control, HMI and safety.
Guardrail: exact servo/HMI solution is implementation-specific; transfer the cross-domain change logic.

### Regulatory support — OSHA 29 CFR 1910.147
Owns: current U.S. illustration that major modification/renovation can affect energy-isolation design obligations.
Guardrail: U.S. workplace-safety scope only; do not universalize.

### Lifecycle support — ABB / EU Machinery Regulation
Owns: obsolescence/lifecycle context and date-qualified substantial-modification concept.
Guardrail: vendor lifecycle language is not a standard; EU Regulation general application date must be rechecked before publication.

## Listener tool — Retrofit Impact Sheet
Before touching an installed machine capture:
`Exact installed version/site → reason for change → obsolete dependency → interfaces touched → hazard/safety functions touched → recipes/parameters/data interfaces touched → expected production-output impact → rollback option → spare/support plan → commissioning tests → quality/release evidence → new baseline/version → training/procedure changes`.

## Lifecycle lens
SUPPORTED CONFIGURATION: preserve exact identity, backups, spares and service evidence.
CONSTRAINED SUPPORT: identify single points of lifecycle failure and migration lead time before emergency failure.
PLANNED RETROFIT: perform cross-domain impact/applicability review before replacement BOM is finalized.
MODIFIED CONFIGURATION: create a new controlled as-built/as-configured state with updated support procedures and evidence.
END-OF-SUPPORT: retire/replace deliberately when technical, safety, economic or supportability envelope is no longer defensible.

## Boundary with EP10
EP10 owns designing serviceability/reliability into a product before/around release.
EP59 owns the already-deployed installed base: multiple generations, site-specific retrofits, obsolescence, changed safety/applicability, recommissioning and support ownership.

Do not re-teach EP10 access/replaceability fundamentals.

## Common mistakes
- replacing a controller as if interfaces around it are unchanged;
- assuming successful power-up equals production release;
- restoring from a backup without proving it is the correct configuration;
- letting site-specific retrofit history live only in technician memory;
- using vendor lifecycle categories as universal standards;
- ignoring changed safety/legal applicability after major modification;
- keeping obsolete systems indefinitely because they have not yet failed catastrophically.

## Source / script gates
Before script lock:
- verify current Siemens case URLs/details if vendor pages have moved;
- anchor any OSHA obligation in current regulation text and exact U.S. scope;
- recheck EU Machinery Regulation 2023/1230 application/transitional status at publication time;
- avoid independent performance/economic claims from vendor case studies;
- keep retrofit re-verification impact-based rather than prescribing universal test scope.

## Season handoff
EP59 closes the external case arc: failures, successes, startup constraints and four industry lenses have all exercised the frozen frameworks. EP60 now returns to one fictional product and walks the full Hardware Evolution Ladder end to end, showing how every earlier decision changes as evidence, volume and production context mature.
