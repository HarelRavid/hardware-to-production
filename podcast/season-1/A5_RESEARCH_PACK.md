# A5 Research Pack — Serious Mechanical Prototype: From Shape to Engineering Evidence

status: CLAIM SET STABLE
season: Season 1 — Build the Right Thing
primary_audience: A — founders/developers/early hardware teams
secondary_audience: mechanical engineers, NPI/industrialization engineers
lifecycle: DEV → early LVP bridge
technical_depth: foundation/practitioner

## Episode promise
Help a team move from a mechanical prototype that demonstrates shape/fit/motion into a prototype deliberately built to answer engineering questions about interfaces, loads, tolerances, materials, assembly, environment and future manufacturing.

## Hook
The enclosure looks right, the mechanism moves, and the demo succeeds. Then the first serious build arrives and holes do not align, the seal leaks, fasteners loosen, a printed feature cannot be molded, and the tolerance stack only worked because one engineer hand-fit every unit.

A more expensive prototype is not automatically a more informative prototype.

## Stable core claim set
A5-C01 — Mechanical prototype maturity should be judged by the claims it can support, not by visual fidelity, cost or build number.

A5-C02 — Geometry, material behavior, surface condition, tolerances, joining, loads and environment are separate evidence dimensions; representing one does not prove the others.

A5-C03 — Interfaces and tolerance stacks become increasingly important when moving from one hand-fit article to interchangeable parts and assemblies.

A5-C04 — Manual rescue operations are valid DEV learning tools only when they remain visible as evidence of design/process uncertainty rather than disappearing into craftsmanship.

A5-C05 — A serious prototype should be selected to expose and retire consequential failure modes/manufacturing uncertainties, not merely to make the demo more production-looking.

A5-C06 — Material/process substitution requires an explicit evidence-transfer decision: what remains representative, what changed and what must be retested.

A5-C07 — Mechanical CTQs should begin to emerge before LVP even if final production tolerances and process capability are not yet known.

A5-C08 — The next build should retire the highest-value uncertainty; production-intent fidelity should be introduced selectively where the claim depends on it.

## Audience contract
### DEV takeaway
Record what each mechanical prototype is intended to prove and which dimensions remain non-representative.

### Prototype shortcuts
Printed parts, manual machining, oversized fasteners, hand finishing, temporary brackets, soft tooling and selective assembly can be legitimate when they accelerate learning.

### Shortcut expiration
A shortcut expires when a decision depends on the dimension it does not represent — for example fatigue, sealing, creep, surface friction, production tolerance, molded geometry, thermal distortion, corrosion or assembly interchangeability.

### LVP change
At tens/hundreds of units the team needs controlled drawings/models, interfaces, CTQs, repeatable assembly intent, tolerance logic, material/process definition and explicit handling of deviations/rework.

### SVP evidence
Commercial production requires demonstrated process/product evidence inside the released configuration/process envelope; one carefully fitted prototype is not that evidence.

### Manufacturing-debt prevention
Capture every manual rescue operation and ask whether it belongs in the design, the process, a fixture/tool, an inspection step or nowhere in the future state.

### Listener action
Perform a Mechanical Prototype Evidence Review on the current build.

## Listener Tool 1 — Mechanical Prototype Evidence Review
For each critical feature/interface, record:
- function and failure if wrong;
- prototype fabrication method;
- intended production method if known;
- geometry/material/tolerance/surface/joint/load/environment representativeness;
- manual rescue used?;
- evidence currently supported;
- evidence not transferable;
- next experiment/build needed.

## Listener Tool 2 — Manual Rescue Log
Whenever the team modifies a part during assembly, record:
`Unit → Part/feature → intervention → why required → time → decision owner → temporary/permanent → suspected root cause → next design/process action`

Repeated rescue operations become engineering signals, not craftsmanship folklore.

## Worked example — Sentinel Node enclosure/interface
Illustrative only.

Prototype 1 uses an FDM enclosure with threaded heat-set inserts and a manually trimmed gasket. It can support package envelope, connector access and basic assembly-sequence learning.

It does not automatically support claims about injection-molded warpage, production datum/tolerance distribution, future gasket sealing, long-term insert behavior, serial assembly time, cosmetic capability or lot-to-lot interchangeability.

Next build decision: do not replace every part with production tooling. Build the minimum articles/fixtures needed to retire the highest-risk interface, sealing and tolerance questions.

## Evidence/standards boundary
Potential source families for later verification:
- ASME Y14.5 / ISO GPS for tolerancing language where actually used;
- ISO 8015 / ISO 1101 / ISO 5459 / ISO 14405 family where applicable;
- material/process-specific ASTM/ISO methods only when a claim requires them;
- authoritative verification guidance for test-article/configuration representativeness.

No exact normative GD&T/GPS requirement is necessary for the conceptual core. Any later statement that a named standard requires a specific practice becomes V1/P0 and must be edition/clause/applicability verified.

## Claim classes / P0 state
- C01/C02/C04/C05/C06/C08: V6 synthesis informed by backbone; P1 support can be added during evidence verification.
- C03/C07: V6 with P2.02/P2.03 linkage; P1.
- Open P0 for current conceptual core: 0.

## Common failure modes
- prototype looks production-like while critical material/process behavior is unrepresented;
- CAD nominal dimensions treated as a tolerance strategy;
- hand fitting hides interface error;
- one supplier's process quirks become accidental design requirements;
- production process selected before uncertainty is understood;
- tolerance tightening replaces datum/interface reasoning;
- test article differs from released configuration without impact assessment.

## Navigation
Prerequisite recap: A4 representativeness/shortcut-expiration concept in 60–90 seconds.
Can stand alone: yes.
Recommended next: A6 for electronics-heavy products; A7 for verification planning; Episode 1 for industrialization transition.

## Claim-set-stable result
PASS.
- Eight non-overlapping claims retained.
- A4 owns the general representativeness framework; A5 applies it to mechanical evidence.
- No assumption that the production process must be finalized in DEV.
- Listener tools map directly to DEV→LVP learning.
- Standards-specific statements remain behind the Source Verification gate.

Next maturity target: EVIDENCE VERIFIED after P1 support and any standards-specific content selected for the script are verified.
