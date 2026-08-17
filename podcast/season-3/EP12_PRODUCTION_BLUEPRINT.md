# Episode 12 Production Blueprint — Polymer Parts: Injection Molding and the Alternatives

status: PRODUCTION BLUEPRINT COMPLETE
season: Season 3 — Manufacturing Processes
lifecycle: DEV → LVP → SVP

## Listener transformation
Before: thinks plastic part = injection molding or 3D print.
After: can compare molding and alternate polymer routes by geometry, material behavior, tooling, variation, surface, volume and economics.

## Narrative hook
A CNC polymer enclosure fits perfectly. The molded version arrives with sink, warp and a shifted opening. Nothing was “wrong with the CAD”; the production process introduced behavior the prototype route never represented.

## Teaching flow
1. Polymer process-family map: injection molding, extrusion, blow molding, thermoforming, rotational molding, compression/transfer/RIM and bridge routes.
2. Injection molding as anchor: melt flow, fill/pack/cool/eject.
3. Geometry-process coupling: wall thickness, ribs/bosses, draft, radii, undercuts, gate/ejection implications.
4. Shrinkage, warpage, sink and weld-line concepts.
5. Material grade/state, moisture and additives as production variables.
6. Tooling/NRE, cavity count, change cost and lead time.
7. Alternate LVP routes: machining, AM, urethane/soft tooling where applicable.
8. Inspection, cosmetics, sealing and assembly interfaces.
9. DEV/LVP/SVP route transition and bridge-process expiration.

## Core framework — Polymer Route Review
`Function/material → geometry → flow/forming mechanism → tooling → expected defects/variation → inspection → volume → economics → evidence → route decision`.

## DEV / LVP / SVP
- DEV: prints/machining can prove packaging and selected functional claims.
- LVP: bridge molding/machining/AM may remain rational with explicit evidence limits.
- SVP: production tooling and process control become justified when volume, repeatability, lead time and economics support them.

## Worked example
Outdoor enclosure: CNC prototype proves fit/sealing geometry at one state. Injection-molded production introduces shrink/warp, gate/weld-line and cosmetic constraints. The design is revised with process-aware wall/rib/datum strategy rather than simply tightening every dimension.

## Listener tools
1. Polymer Process Candidate Table.
2. Moldability/Bridge Review: walls, draft, ejection, flow, shrink/warp, inserts, CTQs, measurement, tooling-change sensitivity.

## Visual asset plan
- Mold cross-section with gate, cavity, ejector and flow front.
- Good vs problematic wall/rib/boss concepts.
- Warp/sink/weld-line illustrations.
- Decision table comparing molding, machining, AM and soft-tool routes.

## Standards/source architecture
Verify exact sources before numerical design rules. Likely source families: ISO/ASTM polymer material/test standards, mold/process-specific guidance, material-supplier processing data and customer requirements. Numeric draft angles, wall limits, shrink values and process windows must remain material/tool/supplier specific unless sourced.

## Common mistakes
- using a generic “plastic” property instead of exact grade/state;
- assuming molded dimensions equal machined dimensions;
- using tighter tolerances to solve architecture problems;
- ignoring moisture/conditioning where material sensitive;
- ordering tooling before process-relevant DFM is stable;
- assuming injection molding wins at every commercial quantity.

## Closing handoff
Episode 13 applies the same route logic to metals, where material state, grain flow, residual stress and secondary operations become central.
