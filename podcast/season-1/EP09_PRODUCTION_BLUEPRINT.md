# Episode 9 Production Blueprint — Tolerance, GD&T/GPS and Variation

status: PRODUCTION BLUEPRINT COMPLETE
season: Season 1 — Build the Right Hardware Before Production Finds Your Mistakes

## Listener transformation
The listener learns to move from nominal geometry to population thinking: functional tolerances, datums/reference strategy, tolerance accumulation, process variation and measurement adequacy.

## Narrative hook
One prototype enclosure, PCB and connector align perfectly. The engineer assumes the drawing is good. In production, each contributor varies and the stack occasionally collides. The team reacts by tightening every dimension, raising cost without proving the interface is robust.

## Teaching flow
1. CAD nominal versus production distributions.
2. Functional requirement before tolerance value.
3. Datum/reference concept and why exact rules depend on invoked standard.
4. Tolerance accumulation and interface margin.
5. Worst-case versus statistical analysis: different questions and assumptions.
6. Measurement adequacy and why observed variation is not automatically true process variation.
7. ISO GPS versus ASME Y14.5 boundary: do not mix rules casually.
8. Enclosure/PCB/connector worked example.
9. Functional Tolerance Chain and Variation Evidence Review.
10. Redesign for margin before defaulting to tighter tolerances.

## Listener tools
**Functional Tolerance Chain:** `Function → Related features → Reference/datum concept → Contributors → Allowed envelope → Process contributors → Measurement → Analysis assumption → Evidence → Reaction`.

**Variation Evidence Review:** ask what fails, which contributors combine, what model is used, whether the process can hold it, whether measurement can resolve it and whether architecture can create more margin.

## DEV/LVP/SVP
DEV: identify consequential interfaces and hand-fit assumptions. LVP: release bounded specifications and measure real populations. SVP: maintain specification, capability, measurement and supplier evidence under controlled change.

## Common mistakes
- Tight tolerance as a quality reflex.
- Working prototype treated as population evidence.
- RSS used without distribution/independence assumptions.
- Worst-case result interpreted as expected yield.
- ASME and ISO GPS treated as interchangeable rule systems.

## Source/evidence backlog
Exact ASME Y14.5 and ISO GPS editions/clauses must be verified before normative symbol/default teaching. Quantitative stack examples require independent arithmetic audit.

## Closing handoff
Episode 9 teaches variation across manufactured units. Episode 10 extends the time axis: variation plus stress, environment and service over the product’s life.
