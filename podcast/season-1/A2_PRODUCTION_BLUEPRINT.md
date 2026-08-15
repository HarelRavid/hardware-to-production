# A2 Production Blueprint — Hardware Team Map: Who Owns What?

status: PRODUCTION BLUEPRINT COMPLETE
season: Season 1 — Build the Right Thing

## Listener transformation
Before: “We need a mechanical engineer, electronics engineer and maybe firmware.”
After: “I can map engineering responsibilities independently of job titles, see which risks have no owner and decide what can be combined, outsourced or must receive specialist review.”

## Narrative hook
A five-person startup has smart engineers and fast prototypes, yet the product repeatedly fails at thermal limits, connector integration and testability. Nobody was incompetent; those responsibilities simply never existed on the org chart or in anyone’s explicit scope.

## Teaching flow
### Segment 1 — Responsibilities before titles
Explain why startups should first map work and decision rights, not copy a large-company org chart.

### Segment 2 — Hardware discipline map
Cover the practical responsibility families:
- product/systems;
- mechanical/structures;
- electronics/power/PCB;
- embedded/firmware/software boundary;
- thermal;
- materials/chemistry where relevant;
- test/verification;
- manufacturing/NPI;
- quality/reliability;
- supply chain/supplier engineering;
- compliance/safety;
- service/field support.

### Segment 3 — One person can wear many hats
Distinguish role coverage from headcount. A founder may own systems + electronics + test early, but must know when competence/review is insufficient.

### Segment 4 — Decision criticality
Introduce escalation triggers:
- safety/compliance impact;
- architecture lock-in;
- irreversible NRE/tooling;
- supplier transfer;
- high-cost qualification;
- hidden cross-discipline interaction;
- production release consequences.

### Segment 5 — Ownership interfaces
Show the difference between “everyone owns quality” and a usable owner for CTQ definition, measurement, disposition and change.

### Segment 6 — Sentinel Node example
Map who owns sensor performance, enclosure sealing, PCB power, firmware, calibration, supplier change, production test and final product integration. Expose missing ownership before hiring decisions.

### Segment 7 — DEV→LVP→SVP horizon
DEV: generalists + targeted experts.
LVP: explicit NPI/quality/supply/test ownership emerges.
SVP: release, change, supplier, production and field authority must be clear and durable.

## Listener tool
### Hardware Discipline Map
Columns:
`Responsibility → decisions → current owner → competence/confidence → review needed → dependency → escalation trigger → future role`.

### Ownership Gap Review
Ask:
1. Which consequential decision currently has no named owner?
2. Which owner is acting outside competence without review?
3. Which decision is shared so broadly that nobody can close it?
4. Which contractor knowledge would disappear if the relationship ended?
5. Which production responsibility is being postponed because “we are still prototyping”?

## Misconceptions to challenge
- “One engineer can’t cover multiple disciplines.”
- “A startup needs a full corporate org chart.”
- “Everyone owns integration.”
- “Quality/manufacturing only matter after design freeze.”
- “Using a consultant means the responsibility is outsourced too.”

## Evidence/source backlog
Mostly V6 synthesis. Add authoritative systems/project responsibility examples only where useful. Any regulated competence/independence requirement must be source- and industry-specific.

## Closing handoff
A2 gives every responsibility an owner. A3 asks where those owners must agree: **the interfaces between subsystems, where locally correct decisions can create a globally broken product.**
