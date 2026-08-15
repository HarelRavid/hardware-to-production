# A5 Research Pack — Serious Mechanical Prototype: From Shape to Engineering Evidence

status: RESEARCH PACK OPEN
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

## Core claim set — draft
1. Mechanical prototype maturity should be judged by the claims it can support, not by visual fidelity or fabrication cost.
2. Geometry, material behavior, surface condition, tolerances, joining, loads and environment are different evidence dimensions; representing one does not prove the others.
3. Interfaces and tolerance stacks often become more important as a product moves from one hand-built unit to interchangeable parts and assemblies.
4. Hand fitting, drilling, sanding, shimming, adhesive improvisation and selective assembly are valuable DEV tools only if they are recorded rather than allowed to hide design/process debt.
5. A serious prototype should deliberately expose likely failure modes and manufacturing constraints rather than optimize only for a successful demonstration.
6. Material/process substitution requires an explicit evidence-transfer decision: what remains representative and what must be retested.
7. Mechanical CTQs should begin to emerge before LVP even if final production tolerances/process capability are not yet known.
8. The next build should be selected to retire the highest-value uncertainty, not simply to increase prototype fidelity everywhere.

Target final core claims: 6–8.

## Audience contract
### DEV takeaway
Record what each mechanical prototype is intended to prove and which dimensions remain non-representative.

### Prototype shortcuts
Acceptable examples may include printed parts, manual machining, oversized fasteners, hand finishing, temporary brackets, soft tooling and selective assembly when they accelerate learning.

### Shortcut expiration
A shortcut expires when a decision depends on the dimension it does not represent — e.g. fatigue, sealing, creep, surface friction, production tolerance, molded geometry, thermal distortion, corrosion or assembly interchangeability.

### LVP change
At tens/hundreds of units the team needs controlled drawings/models, interfaces, CTQs, repeatable assembly intent, tolerance logic, material/process definition and explicit handling of deviations/rework.

### SVP evidence
Commercial production requires demonstrated process capability and product performance inside the released configuration/process envelope; one carefully fitted prototype is not that evidence.

### Manufacturing-debt prevention
Capture every manual rescue operation and ask whether it belongs in the design, the process, a fixture/tool, an inspection step or nowhere in the future state.

### Listener action
Perform a Mechanical Prototype Evidence Review on the current build.

## Listener Tool 1 — Mechanical Prototype Evidence Review
For each critical feature/interface, record:
- function;
- failure if wrong;
- prototype fabrication method;
- intended production method if known;
- geometry representativeness;
- material representativeness;
- tolerance representativeness;
- surface/finish representativeness;
- joint/fastener representativeness;
- load/environment representativeness;
- manual rescue used?;
- evidence currently supported;
- evidence not transferable;
- next experiment/build needed.

## Listener Tool 2 — Manual Rescue Log
Whenever the team modifies a part during assembly, record:
`Unit → Part/feature → intervention → why required → time → who decided → temporary/permanent → suspected root cause → next design/process action`

Repeated rescue operations become engineering signals, not craftsmanship folklore.

## Worked example — Sentinel Node enclosure/interface
Illustrative only.

Prototype 1 uses an FDM enclosure with threaded heat-set inserts and a manually trimmed gasket. It proves package envelope, connector access and basic assembly sequence.

It does NOT automatically prove:
- injection-molded warpage;
- production datum/tolerance stack;
- sealing performance of the future gasket geometry;
- long-term insert pull-out/creep behavior;
- cosmetic surface acceptance;
- serial assembly time;
- interchangeability across independently produced lots.

Next build decision: do not replace every part with production tooling. Build only the articles/fixtures needed to retire the highest-risk interface, sealing and tolerance questions.

## Standards/evidence hooks
Potential source families for later verification:
- ASME Y14.5 / ISO GPS for tolerancing language where used;
- ISO 8015 / ISO 1101 / ISO 5459 / ISO 14405 family where applicable;
- material/process-specific ASTM/ISO test methods only when a claim actually requires them;
- NASA/system-engineering verification guidance for configuration/test-article representativeness concepts.

Guardrail: this episode is not a GD&T training episode and must not imply that one tolerancing standard is universally mandated.

## Initial claim classes
- Claims 1, 2, 4, 5, 6, 8: V6 synthesis informed by backbone + later authoritative support.
- Claim 3: V2/V5 support desirable; P1.
- Claim 7: V6 with P2.03/P2.02 linkage; P1.
- Any exact normative GD&T/GPS statement: V1/P0 before script use.

## P0 backlog
- None required for the conceptual core if standards are discussed descriptively.
- Any sentence saying a named standard requires a specific drawing/tolerance practice becomes P0 and must be clause/edition verified.

## Common failure modes to teach
- prototype looks production-like but critical material/process behavior is unrepresented;
- CAD nominal dimensions used as if tolerance strategy exists;
- hand fitting hides interface error;
- one supplier's process quirks become accidental design requirements;
- production process selected before uncertainty is understood;
- tolerance tightening used instead of datum/interface reasoning;
- test article differs from released configuration without impact assessment.

## Navigation
Prerequisite recap: A4 representativeness/shortcut-expiration concept in 60–90 seconds.
Can stand alone: yes.
Recommended next: A6 for electronics-heavy products; A7 for verification planning; Episode 1 for industrialization transition.

## Claim-set-stable exit criteria
- reduce draft claims to 6–8 non-overlapping claims;
- verify terminology around tolerance/interface evidence;
- ensure no hidden assumption that production process must be chosen in DEV;
- map every listener tool to DEV/LVP/SVP;
- record all standards-specific statements in Source Verification Backlog.
