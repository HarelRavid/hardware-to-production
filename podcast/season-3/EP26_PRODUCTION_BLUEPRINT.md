# Episode 26 Production Blueprint — How to Plan a Pilot Build

status: PRODUCTION BLUEPRINT COMPLETE
season: Season 3 — Build the Factory Before You Need the Factory
lifecycle: LVP → Production Validation

## Listener transformation
Before: thinks a pilot is simply a small batch before production.
After: can design a pilot as an evidence-generating experiment with explicit objectives, configuration, sample logic, data capture, stop rules and exit criteria.

## Narrative hook
A team builds 25 units, ships most of them and declares the pilot successful. Later nobody can answer which process assumptions were tested, how many units were reworked, or whether the same configuration was used throughout.

## Teaching flow
1. Pilot purpose: learn versus prove.
2. Define exact build configuration and allowed deviations.
3. Select objectives across product/process/supplier/test/people.
4. Quantity rationale based on learning needs, not magic numbers.
5. Data plan: defects, rework, cycle, measurement, intervention and shortages.
6. Stop/containment criteria.
7. Change rules during the build and effectivity.
8. Daily/shift learning loop and evidence closure.
9. Pilot exit decision and carryover gaps.

## Core framework — Pilot Build Plan
`Decision after pilot → objectives → configuration → population/quantity rationale → route/tooling/suppliers → CTQs/test → staffing/qualification → data capture → allowed intervention → stop rule → change/effectivity → exit evidence → carryover gaps`.

## DEV/LVP/SVP
DEV: prototype builds can change freely if evidence is labeled. LVP pilot: changes are allowed but must preserve identity/effectivity. Production validation: tighter configuration and execution control is required.

## Common mistakes
- pilot quantity as the objective;
- mixing configurations and reporting one yield;
- undocumented engineer rescue;
- shipping units before learning capture is complete;
- no stop rule for repeated critical defects;
- changing process mid-build without effectivity.

## Source/evidence backlog
Customer/industry pilot and PPAP-style requirements remain applicability gated. No universal unit count or exit threshold.

## Closing handoff
Episode 26 plans the experiment. Episode 27 defines what a production-validation build must actually demonstrate before ramp.
