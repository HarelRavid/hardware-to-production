# Episode 11 Production Blueprint — How to Select a Manufacturing Process

status: PRODUCTION BLUEPRINT COMPLETE
season: Season 3 — Manufacturing Processes
lifecycle: DEV → LVP → SVP

## Listener transformation
Before: chooses processes by familiarity, prototype convenience or quoted piece price.
After: compares candidate manufacturing routes against product function, material/state, geometry, tolerance, surface, volume, tooling, capability, inspection, supplier maturity, lead time and cost per accepted good unit.

## Narrative hook
A machined prototype works beautifully. The team assumes injection molding will simply be the cheaper production version. Tooling is ordered, then wall/warpage/tolerance and inspection assumptions collapse. The failure began before the mold: the team never made a process-selection decision, only a process-name decision.

## Teaching flow
1. Why geometry alone does not select a process.
2. Start with product claims/CTQs and required material state.
3. Translate geometry/tolerance/surface into process constraints.
4. Add production stage: DEV, bridge/LVP, SVP.
5. Add tooling/NRE, lead time and design-change flexibility.
6. Add supplier/equipment capability and inspection burden.
7. Compare total economics using accepted good output.
8. Build a process-chain candidate, not only a primary operation.
9. Define bridge-process expiration triggers.
10. Hand off to process-family deep dives.

## Core framework — Process Selection Decision Grid
`Function → Material/state → Geometry → Tolerance/surface → Stage/volume → Candidate route → Capability evidence → Inspection → Supplier → Tooling/NRE → Yield/secondary ops → Cost per good unit → Exit trigger`.

## DEV / LVP / SVP
- DEV: maximize learning speed; document what production behavior is not represented.
- LVP: bridge processes are acceptable when controlled and economically rational.
- SVP: route must support demonstrated capability, rate, quality, supply and economic envelope.

## Worked example
Sentinel Node enclosure: FDM for packaging learning → CNC/urethane/high-quality AM candidates for LVP → injection molding only if geometry, material, volume, tooling economics and capability justify it. The lesson is not that molding is more mature; it is that each route supports a different evidence/economic envelope.

## Listener tools
1. Process Selection Decision Grid.
2. Bridge-Process Exit Check: cost, lead time, unrepresented behavior, capability, manual rescue, supplier dependence, redesign cost and evidence needed before switch.

## Visual asset plan
- Multi-axis process-selection radar/table.
- Same part shown across printed, machined and molded routes.
- Process-chain diagram with primary + secondary operations.
- Cost-vs-volume conceptual curve labelled as illustrative only.

## Standards/source architecture
Foundation claims are synthesis/backbone. Process-specific limits are deferred to Episodes 12–18 and their exact sources. Source families to map include ISO/ASTM/ASME/SAE/AWS/IPC and material/process-specific standards as applicable. No universal numeric process limits enter the script without verified source/equipment context.

## Common mistakes
- lowest piece price = lowest total cost;
- high-volume process = automatically better;
- prototype success = production capability;
- supplier brochure capability = demonstrated source capability;
- treating post-processing as an afterthought;
- retaining bridge manufacturing with no exit trigger.

## Closing handoff
Now that the listener can choose a route systematically, Episode 12 applies the logic to polymer parts, where material flow, tooling and geometry become tightly coupled.
