# A1 Production Blueprint — From an Idea to Engineering Requirements

status: PRODUCTION BLUEPRINT COMPLETE
season: Season 1 — Build the Right Thing

## Listener transformation
Before: “I have a product idea and want to start CAD/PCB immediately.”
After: “I can turn product intent into a small requirement baseline, expose assumptions and decide what the next prototype must learn.”

## Narrative hook
A team spends six weeks designing a polished prototype. At integration they discover that nobody agreed on operating temperature, battery life, allowable size, connector orientation, cleaning method or whether the product must survive outdoor rain. The engineering was competent; the problem was that the team started solving before agreeing what had to be true.

## Teaching flow
### Segment 1 — Why ideas are not engineering inputs
Explain the gap between user/problem statements and engineering requirements. Show why “small,” “robust,” “fast,” “portable” and “waterproof” are not yet useful engineering statements.

### Segment 2 — Minimum Useful Requirements
Introduce categories:
- function/performance;
- environment/load/duty cycle;
- interfaces;
- power/resources;
- physical envelope;
- safety/regulatory assumptions;
- manufacturing/service constraints;
- cost/volume assumptions;
- verification intent.

The goal is not completeness. The goal is enough control to prevent random engineering.

### Segment 3 — Requirement vs solution
Examples:
- requirement: user must replace module in X context;
- solution disguised as requirement: use four M3 screws.
Teach when a solution constraint is legitimate and when it prematurely freezes design space.

### Segment 4 — Unknowns are allowed; invisible unknowns are not
Introduce labels: CONFIRMED / TARGET / ASSUMPTION / TBD.
Every important TBD gets owner + learning action + expiration trigger.

### Segment 5 — Requirement quality
Use the Requirement Quality Check:
- clear subject;
- measurable/observable condition;
- operating conditions;
- rationale/source when important;
- verification path;
- no hidden contradiction;
- no unnecessary implementation constraint.

### Segment 6 — Sentinel Node example
Transform “small outdoor sensor node that sends data all day” into a minimum baseline: sensing function, update interval target, outdoor environment assumption, power target, enclosure/interface bounds, service concept and explicit unknowns.

### Segment 7 — DEV→LVP→SVP horizon
DEV: requirements can be ranges/targets.
LVP: supplier, inspection, test and interface requirements must harden.
SVP: CTQs, compliance and release criteria require controlled, traceable requirements.

## Listener tool
### Minimum Useful Requirements Sheet
Fields:
`Need → requirement → class → status → source/rationale → owner → verification idea → next learning action → expiration trigger`.

### 20-minute action
Take the current product idea and write only the 10–20 requirements that would make the next prototype materially different if they changed.

## Misconceptions to challenge
- “Requirements are bureaucracy.”
- “We can define everything later.”
- “A prototype will tell us what the requirements are.”
- “TBD means failure to decide.”
- “More requirements always means better engineering.”

## Evidence/source backlog
- ISO/IEC/IEEE 29148 exact terminology where used.
- NASA systems-engineering guidance for requirement quality/verification linkage.
- Any safety/regulatory requirement must remain product/jurisdiction specific.

## Closing handoff
The listener now knows what must be true. A2 asks the next unavoidable question: **who is capable and accountable for making each part of that truth real?**
