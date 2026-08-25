# Episode 18 Production Blueprint — Surface Engineering, Cleaning and Heat Treatment

status: PRODUCTION BLUEPRINT COMPLETE
season: Season 2 — How Hardware Is Actually Made
lifecycle: DEV → LVP → SVP

## Listener transformation
Before: sees coating, cleaning and heat treatment as secondary finishing operations.
After: treats surface/material state as controlled product definition that can change function, dimensions, corrosion, wear, adhesion, contamination and later process evidence.

## Narrative hook
A machined part passes inspection, then fails after coating because masking, thickness and surface preparation shift a sealing interface. Another joint fails because “cleaning” left contamination incompatible with bonding. The geometry was right before the final process — and wrong for the final product state.

## Teaching flow
1. Why final product state includes surface and metallurgical/chemical condition.
2. Cleaning: contamination type, cleanliness objective, sequence and verification.
3. Surface preparation: activation, roughness and compatibility before bonding/coating.
4. Coatings/finishes: corrosion, wear, friction, electrical/thermal and cosmetic functions.
5. Masking and selective treatment.
6. Heat treatment: material-state transformation, distortion and property evidence.
7. Sequence interactions: machine-before/after, clean-before-join, heat-treat-before-finish, etc.
8. Rework/stripping and configuration impact.
9. DEV/LVP/SVP control: recipe, bath/furnace state, lot/fixture and inspection evidence.

## Core framework — State Transformation Card
`Incoming material/surface state → preparation → process → critical parameters → expected transformation → dimensional/property side effects → verification → allowed rework → next operation`.

## Worked example
Machined aluminum housing requires corrosion protection and a precision sealing surface. The team decides which areas are coated/masked, whether final machining occurs before/after treatment, how coating thickness affects fit, and what cleaning state is required before assembly.

## Listener tools
1. State Transformation Card.
2. Process-Sequence Compatibility Check: what the next operation needs, what the current one leaves behind, and what evidence can be invalidated.

## Visual asset plan
- Cross-section of coating/masking/tolerance interaction.
- Surface-prep → coating → verification flow.
- Heat-treatment distortion timeline.
- Contamination pathway example before adhesive/joining.

## Standards/source architecture
Potential sources include ISO/ASTM coating/cleanliness/corrosion test methods, SAE/AMS heat-treatment and pyrometry requirements, material specifications and sector/customer standards. AMS2750 and related heat-treatment standards are source targets where applicable, not universal requirements. Exact coating thickness, cleanliness acceptance, furnace class/uniformity or heat-treatment recipe must remain scoped to material/process/product requirements.

## Common mistakes
- treating cleaning as “looks clean”;
- specifying coating without functional surface/masking definition;
- inspecting dimensions before a later process that changes them;
- ignoring stripping/recoat or heat-treatment rework effects;
- using generic heat-treatment names without exact alloy/state/process definition;
- losing traceability between treated batch and final units.

## Closing handoff
Episode 19 now connects the primary process, joining, thermal, cleaning, coating and inspection steps into one controlled process chain where sequence itself becomes part of design.
