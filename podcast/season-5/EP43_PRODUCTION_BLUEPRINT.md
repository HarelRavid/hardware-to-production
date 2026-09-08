# Episode 43 Production Blueprint — Semi-Automation, Robotics and Machine Vision

status: PRODUCTION BLUEPRINT COMPLETE
season: Season 5 — Automation, Data and the Connected Factory
lifecycle: LVP → Ramp → SVP
maps_to: MASTER_WBS 8.3, 8.4, 8.5

## Listener transformation
Before: frames automation as manual versus fully automatic.
After: decomposes the process into functions and assigns human, fixture, assisted, robotic, sensing or vision roles according to variability, consequence, economics and maintainability.

## Narrative hook
A fully robotic station is proposed for an assembly where only one repetitive alignment/dispense step is painful. A simple fixture plus controlled dispenser would remove most of the loss while keeping operator judgement where variability remains. The right automation boundary is smaller than the sales proposal.

## Teaching flow
1. Decompose the operation into handling, locating, transformation, verification and decision functions.
2. Identify repetitive/ergonomic/hazardous/precision burdens.
3. Preserve human judgement where variability is not yet modeled.
4. Mechanization and powered tooling before robotics where appropriate.
5. Robot/cobot selection as application-specific, not maturity labels.
6. Feeding, fixturing, end effectors and part presentation as system design.
7. Machine vision: lighting/optics/feature stability before algorithms.
8. Error handling, recovery and abnormal states.
9. Safety, access, changeover and maintenance from the start.
10. Scale only after the chosen boundary is demonstrated.

## Core framework — Function Automation Map
`Process step → function → variation → consequence → human strength → machine strength → sensing/measurement → fixture/handling → automation level → abnormal/recovery mode → evidence`.

## Listener tools
- Function Automation Map.
- Vision Feasibility Card: feature, contrast, lighting, pose, occlusion, tolerance, reference truth, false-pass/fail consequence and calibration/change control.

## DEV / LVP / SVP
DEV: automate experiments only where it accelerates learning. LVP: favor modular assistance and semi-automation with easy changeover. SVP: robotic/vision systems require controlled interfaces, validation, maintenance and recovery.

## Common mistakes
- robot purchased before feeding/fixturing is solved;
- cobot assumed inherently safe for every application;
- vision algorithm blamed for bad lighting/part presentation;
- operator flexibility removed before variation is understood;
- abnormal/recovery states omitted from cycle-time and quality logic.

## Source/evidence backlog
Robot/cobot/machine safety and vision validation requirements are application- and jurisdiction-dependent. Exact ISO/IEC/ANSI/industry requirements require edition and applicability verification.

## Closing handoff
Episode 44 focuses on one automation boundary with unusually high evidence burden: automated inspection and end-of-line acceptance.
