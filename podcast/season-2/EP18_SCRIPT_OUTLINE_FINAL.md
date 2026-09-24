# EP18 Final Script Outline — Surface Engineering, Cleaning and Heat Treatment

status: FINAL SCRIPT OUTLINE COMPLETE — SEASON CONTINUITY PENDING
season: Season 2 — How Hardware Is Actually Made
audience: design / NPI / manufacturing / quality / materials
lifecycle: DEV → LVP → SVP
source_lock: evidence/source-lock/wave-06/W6H_EP18_CLAIM_LOCK.md
technical_review: evidence/source-lock/wave-06/W6H_INTERNAL_TECHNICAL_REVIEW.md
blueprint: podcast/season-2/EP18_PRODUCTION_BLUEPRINT.md

## Listener transformation

Before:
“Cleaning, coating and heat treatment are secondary finishing steps.”

After:
“I can treat surface/cleanliness/metallurgical state as part of the final product definition and manage the sequence, dimensional effects, verification and rework accordingly.”

## Two-character opportunity

Rona:
“If the machined part already passed inspection, why should coating or heat treatment force us to revisit dimensions?”

Oz:
Because the final product state exists after the state-changing process, not before it.

## Cold open

[ILLUSTRATIVE]
A machined housing passes dimensional inspection, then coating shifts a sealing interface. Another joint fails because “cleaning” left a surface incompatible with bonding.

## Beat 1 — Final state is more than shape

Claim: EP18-C01.

Surface condition
+ cleanliness
+ coating/conversion
+ metallurgical state
can be part of the released product state.

## Beat 2 — Cleaning must have an objective

Claim: EP18-C02.

Ask:
- what contamination?
- why remove it?
- what downstream process depends on it?
- how do we know it is clean enough?

Guard:
no universal cleanliness criterion.

## Beat 3 — Surface preparation is process input

Claim: EP18-C03.
Callback to EP14 adhesive bonding.

Use ISO 8501 examples only as scoped steel/coating context.

## Beat 4 — Select a surface system, not a coating name

Claim: EP18-C04.

Substrate
→ preparation
→ treatment/coating
→ cure/post-treatment
→ masking/racking
→ inspection
→ handling.

## Beat 5 — Thickness/masking can move function

Claim: EP18-C05.

Examples:
fit / thread / sealing land / electrical contact / thermal interface.

No generic thickness number.

## Beat 6 — Corrosion testing is not direct service-life prophecy

Claim: EP18-C06.
Source: ISO 9227:2022.

Explain:
test method evidence must be interpreted through product/environment/specification context.

## Beat 7 — Heat treatment changes material state

Claim: EP18-C07.

Use AMS2750H / CQI-9 only as scoped examples of controlled thermal-process evidence.

## Beat 8 — Furnace recipe vs actual part history

Claim: EP18-C08.

Load / fixture / geometry / atmosphere / quench or cooling / transfer can matter.

## Beat 9 — Distortion / residual stress / downstream dimensions

Claim: EP18-C09.

Connect:
heat treat ↔ machining ↔ GD&T ↔ coating ↔ joining.

## Beat 10 — Rework changes history

Claim: EP18-C10.

Stripping / recoating / reheating may affect substrate/state/evidence.

## Beat 11 — Process sequence compatibility

Claim: EP18-C11.

Examples:
- clean before bond;
- heat treat before/after machining;
- mask before coating;
- final inspect after state-changing process.

Preview EP19 without teaching full chain.

## Listener tool — State Transformation Card

Incoming state
→ preparation
→ process
→ critical variables
→ expected transformation
→ dimensional/property side effects
→ verification
→ allowed rework
→ next operation.

## Listener tool — Process-Sequence Compatibility Check

Current operation leaves what state?
Next operation requires what state?
What can invalidate evidence?
What must be remeasured/reverified?

## DEV / LVP / SVP

DEV:
fast/manual treatments acceptable if state/limitations are visible.

LVP:
controlled recipes/lots/fixtures/inspection and downstream compatibility.

SVP:
supplier/process qualification, traceability, rework controls, stable sequence and evidence.

## Misconceptions

- looks clean = clean enough;
- coating is cosmetic only;
- pre-coating dimensions are final;
- salt-spray hours equal field life;
- furnace setpoint equals part thermal history;
- hardness alone proves all heat-treatment properties;
- stripping/recoat is neutral.

## Closing action

Take one part with a surface or thermal process and fill a State Transformation Card from incoming state through the next operation.

## Handoff

EP18 proves that “secondary” processes can redefine the product state.
EP19 now connects every primary, joining, thermal, surface and inspection step into one controlled manufacturing chain.
