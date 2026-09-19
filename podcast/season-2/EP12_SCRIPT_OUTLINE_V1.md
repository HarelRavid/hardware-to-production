# EP12 Script Outline V1 — Polymer Parts: Injection Molding and the Alternatives

status: SCRIPT OUTLINE COMPLETE
season: Season 2 — How Hardware Is Actually Made
audience: design / NPI / manufacturing / sourcing
lifecycle: DEV → LVP → SVP
source_lock: evidence/source-lock/wave-06/W6B_EP12_CLAIM_LOCK.md
technical_review: evidence/source-lock/wave-06/W6B_INTERNAL_TECHNICAL_REVIEW.md
blueprint: podcast/season-2/EP12_PRODUCTION_BLUEPRINT.md

## Listener promise

Choose a polymer manufacturing route and identify which material/process mechanisms must be represented before tooling or production release.

## Cold open

[ILLUSTRATIVE]
A CNC polymer enclosure seals perfectly. The molded version arrives with a shifted opening, sink near a boss and visible warp. CAD did not suddenly become wrong; the process created a different material/geometry state.

## Beat 1 — Exact material grade/state matters

Claims: EP12-C01 / C10.
Sources: W6B-S03/S04/S05/S06.
Key message:
“Plastic” is not an engineering material definition.

## Beat 2 — Map the polymer process families

Claims: EP12-C11.
Injection moulding, extrusion, blow moulding, thermoforming, rotational moulding, compression/transfer/reactive moulding, plus bridge routes.

Guard:
descriptive comparison only; no unsourced capability table.

## Beat 3 — Injection moulding as anchor process

Claim: EP12-C02.
fill → pack → cool → eject.
Tool/process conditions create the produced state.

## Beat 4 — Moulded tolerance is plastics-specific

Claims: EP12-C03/C04.
Source: ISO 20457:2026 public scope.
CNC prototype dimensions do not automatically predict moulded variation.

## Beat 5 — Shrinkage and warpage

Claims: EP12-C05/C06.
Sources: ISO 294-4 + Moldflow.
Directional shrinkage, cooling, orientation and geometry interactions.

## Beat 6 — Sink/void and local geometry

Claim: EP12-C07.
Source: Moldflow technical guidance.
Teach mechanism; no rib/wall percentage rule.

## Beat 7 — Weld/meld lines and flow path

Claim: EP12-C08.
Source: Moldflow.
Consequence depends on location/material/process.

## Beat 8 — Tooling is product/process architecture

Claim: EP12-C09.
Gate, runner, cooling, venting, ejection and access interact with quality and geometry.

## Beat 9 — Moisture and conditioning

Claim: EP12-C10.
ISO 62 + BASF examples.
Guard: material specific; no drying recipe.

## Beat 10 — Bridge route and exit trigger

Claims: EP12-C11/C12.
Reuse Wave 06A:
machining / AM / soft tooling may be rational while design or demand remains uncertain.

## Listener tool — Polymer Route Review

Function/material → geometry → forming mechanism → tooling → expected defects/variation → inspection → stage/volume → economics → evidence → route decision.

## Moldability / Bridge Review

Check:
- exact grade/state;
- important flow/geometry interactions;
- shrink/warp-sensitive interfaces;
- sink/weld-line consequence;
- tooling/gate/ejection dependencies;
- CTQs/measurement;
- what prototype route does not represent;
- tooling-change sensitivity;
- bridge exit trigger.

## Misconceptions

- “plastic” defines properties;
- molded part should match CNC dimensions;
- one shrink factor works everywhere;
- tighter tolerances fix warpage;
- simulation is qualification;
- injection molding automatically wins at production volume.

## Closing action

For one polymer part, list the product claims your current prototype actually represents—and the moulding-specific mechanisms it does not.

## Handoff

EP13 applies the same route logic to metals, where material state, grain flow, thermal history and secondary operations dominate the decision.
