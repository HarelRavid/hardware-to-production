# A1 Script Outline — From an Idea to Engineering Requirements

status: SCRIPT OUTLINE COMPLETE — FULL SCRIPT DRAFT NEXT
season: Season 1 — Build the Right Hardware Before Production Finds Your Mistakes
primary_audience: founders / early hardware teams
lifecycle: Idea → Requirements → Architecture; DEV-FIRST
entry_point: PRIMARY SERIES ENTRY
production_blueprint: `podcast/season-1/A1_PRODUCTION_BLUEPRINT.md`
claim_basis: `podcast/pilot/A1_RESEARCH_PACK.md` (historical pilot location; claim content retained)
source_lock: `evidence/source-lock/wave-01/W1_A1_A7_A8_CLAIM_LOCK.md`
shared_sources: `evidence/source-lock/wave-01/W1_SHARED_SOURCE_REGISTER.md`
technical_review: `evidence/source-lock/wave-01/W1_INTERNAL_TECHNICAL_REVIEW.md`
outline_contract: `podcast/SCRIPT_OUTLINE_CONTRACT.md`

## 1. Episode job

Listener enters with:
> I have a product idea. I should probably start drawing/building.

Listener leaves with:
> I can write the minimum product truth that must be explicit before different engineers start solving different products, while keeping uncertainty visible instead of pretending everything is known.

Primary listener action:
Create a one-page **Minimum Useful Requirements Sheet** for the next prototype/build decision.

## 2. Cold open — competent engineering, wrong problem

### Narrative
[ILLUSTRATIVE]
A small hardware team spends six weeks producing a polished prototype. Mechanical work is good. PCB work is good. Firmware works.

At integration, five questions suddenly appear:
- What temperature must it operate at?
- What supply/power behavior is actually allowed?
- Which way must the connector face in the real installation?
- Does the customer expect cleaning with chemicals?
- Is the enclosure expected to survive rain or only an indoor splash?

Nobody made an obviously bad engineering decision.
They simply answered different unstated versions of the product.

### Core point
[SYNTHESIS — A1-C01]
An idea gives direction. It does not yet give a multidisciplinary team enough controlled engineering truth to coordinate detailed design.

### Wording guard
Do not claim this is a sourced real company failure.
Do not say requirements eliminate iteration.

### Transition
The solution is not a 200-page specification before prototype #1. The solution is the **minimum useful requirement baseline**.

---

## 3. Beat 1 — what changes when an idea becomes an engineering input?

### Narrative point
Move from adjectives and intent to observable constraints/outcomes.

Examples:
- `rugged` → under which load/environment?
- `portable` → mass/envelope/use expectation?
- `fast` → response time or throughput?
- `waterproof` → what exposure/use condition?

### Source ownership
[AUTH-GUIDANCE — A1-C01/A1-C02]
Source anchors:
- S-W1-01 NASA SEH §4.2 Technical Requirements Definition.
- S-W1-05 NASA Appendix C/D.

NASA supports the engineering premise that stakeholder expectations/constraints are translated into validated technical requirements and that requirements need enough definition to be verified.

### Synthesis
[SYNTHESIS]
For an early commercial hardware team, the useful threshold is not formal completeness. It is enough clarity that the next architecture/prototype decision is solving the intended problem.

### Technical guard
Do not tell listeners that every early requirement must use formal NASA `shall` syntax.

---

## 4. Beat 2 — Minimum Useful Requirements: seven buckets

Use a physical whiteboard/listener worksheet progression rather than terminology lecture.

### 4.1 Function / performance
What must the product do and how well where that matters now?

[AUTH-GUIDANCE]
NASA SEH §4.2 identifies functional/performance requirements as core technical requirement types.

### 4.2 Interfaces
What must connect/interact with what?
Examples: mounting, connectors, voltage/current, communication, fluid/thermal/human/service interfaces.

[AUTH-GUIDANCE]
NASA SEH §4.2 includes interface requirements and physical/functional interfaces.

### 4.3 Environment / operating context
Temperature, humidity, vibration, dust/water, chemicals, storage/transport, duty cycle — only what is relevant enough to affect current decisions.

[AUTH-GUIDANCE]
NASA SEH §4.2 identifies environmental/crosscutting constraints.

### 4.4 Safety / compliance watchlist
Known hazard/compliance boundaries that might materially constrain architecture.

[AUTH-GUIDANCE + SYNTHESIS — A1-C06]
NASA supports safety/environmental/standards constraints as engineering inputs.
The podcast's `watchlist` is our lightweight implementation.

Guard:
Do not imply the watchlist determines legal compliance or that one generic standard applies.

### 4.5 Reliability / service
Useful life, duty cycle, maintenance/service assumptions when already architecture-relevant.

[SYNTHESIS]
No generic lifetime requirement is invented.

### 4.6 Manufacturing / supply horizon
Expected near-term quantity, likely process/supplier constraints and test/calibration needs where they alter design now.

[SYNTHESIS]
Do not turn speculative future mass production into premature design lock.

### 4.7 Assumptions / TBDs
Capture uncertainty as an explicit object.

[SYNTHESIS — A1-C05]
`assumption/TBD → why unknown → learning action → owner → expiration condition`.

### Transition
Once the buckets exist, the next challenge is avoiding the opposite mistake: writing the chosen solution as if it were the need.

---

## 5. Beat 3 — requirement vs design solution

### Example 1
Need/outcome:
The service technician must replace a module under the defined service conditions.

Premature solution:
The module shall use four M3 screws.

### Teaching point
[SYNTHESIS]
A design solution can legitimately become a constraint when there is a real reason: common platform, mandated interface, approved supplier/component, regulatory/customer constraint, service compatibility, etc.

The error is not `specifying a screw`. The error is freezing a solution while forgetting the reason it exists.

### Tool field
Add `source/rationale` to the Minimum Useful Requirements Sheet.

### Source support
[AUTH-GUIDANCE]
S-W1-02 NASA requirements traceability/source rationale premise.

---

## 6. Beat 4 — unknowns are allowed; invisible unknowns are not

### Story
[ILLUSTRATIVE]
A sensor accuracy value is not known yet.
Two possible behaviors:
1. write a confident number because the spreadsheet has a cell;
2. record a target range/TBD and define the test that will resolve it.

### Claim
[SYNTHESIS — A1-C05/A1-C10]
Early DEV can carry explicit uncertainty. The control is that uncertainty has identity, owner and a point at which it can no longer safely remain unresolved.

### Expiration examples
A TBD stops being harmless when it begins to control:
- an interface;
- a safety/compliance decision;
- supplier selection;
- irreversible tooling;
- customer claim;
- verification acceptance;
- production test/control.

[SYNTHESIS + A1-C08 premise]

### Source anchor
[AUTH-GUIDANCE]
S-W1-02 supports controlled baselines/change impact once requirements are managed/baselined.

### Wording guard
Do not claim NASA/ISO defines our `expiration trigger` concept.

---

## 7. Beat 5 — Requirement Quality Check

Run the listener's own example through eight questions:

1. WHY — what need/hazard/interface/business constraint drives it?
2. WHAT — what observable outcome is required?
3. HOW MUCH — value/range/unit needed?
4. WHERE/WHEN — operating conditions?
5. INTERFACE — who/what depends on it?
6. VERIFY — how could we know it is satisfied?
7. MATURITY — confirmed / target / assumption / TBD?
8. CHANGE IMPACT — who must know if it changes?

### Ownership
[SYNTHESIS]
This is the Hardware-to-Production listener tool.

### External premise
[AUTH-GUIDANCE — A1-C02/C03]
NASA source family supports verifiability, source/traceability and managed change.

### Technical guard
Do not imply this eight-question list is copied from NASA or ISO 29148.

---

## 8. Beat 6 — Sentinel Node worked pass

[ILLUSTRATIVE / CANONICAL SENTINEL]

Start:
`small outdoor sensor node that monitors rotating machinery`.

Build only a minimal early baseline:

### Product function
Detect/measure vibration and temperature sufficiently to support the target condition-monitoring use case.

### Interfaces
- machine mounting interface;
- 24 VDC supply candidate;
- wired communications candidate;
- service/programming access in DEV.

### Environment
- industrial location;
- dust/wet exposure assumption to be resolved;
- temperature/vibration envelope under definition.

### Unknowns/TBD
- final sensor accuracy;
- final enclosure ingress target;
- final connector family;
- final production calibration method.

### Learning actions
- sensor characterization;
- installation/mount transfer study;
- environmental exposure tests;
- connector/service investigation.

### Lesson
[SYNTHESIS]
The sheet does not make Sentinel production ready. It makes the next engineering decisions **traceably intentional**.

---

## 9. Beat 7 — verification begins inside requirements thinking

### Point
Do not fully teach A7 here.
Ask one question for each important requirement:
> If this mattered enough to write down, what kind of evidence could eventually tell us whether it is true?

### Source anchor
[AUTH-GUIDANCE — A1-C02/C03]
S-W1-03 + S-W1-05.
NASA's requirements/verification guidance supports linking requirements to verification approach/source records.

### Guard
Do not introduce full verification hierarchy, qualification planning or formal V&V bureaucracy.

### Transition
A7 will later teach how to turn this `verification idea` into defensible evidence.

---

## 10. Beat 8 — what hardens from DEV → LVP → SVP?

### DEV
[SYNTHESIS]
- ranges/TBDs may remain;
- objective is controlled learning;
- lightweight tool is enough.

### LVP
[SYNTHESIS]
Requirements that drive supplier specs, interfaces, inspection/test, process controls and release decisions become more controlled and traceable.

### SVP
[SYNTHESIS]
Critical requirements/evidence/change relationships need to scale across released configurations, larger populations and field feedback.

### Guard
Do not imply DEV/LVP/SVP is an external standard lifecycle.
Do not imply requirements become absolutely frozen in SVP.

---

## 11. Misconceptions to explicitly challenge

1. `Requirements are paperwork before engineering.`
Correction: the minimum baseline is coordination infrastructure for engineering decisions.

2. `We should define everything before prototyping.`
Correction: uncertainty is legitimate when visible and paired with learning.

3. `The prototype will tell us the requirements.`
Correction: prototypes can refine requirements, but without an initial intended claim/context you cannot tell what was learned.

4. `TBD means failure.`
Correction: invisible or ownerless TBD is the problem.

5. `More requirements = more mature.`
Correction: unnecessary/premature constraints can reduce learning and lock poor solutions.

6. `Safety/regulatory can be checked near launch.`
Correction: potential constraints should be identified early enough to avoid late architecture conflicts; exact obligations are product/jurisdiction specific.

7. `ISO 29148 is the startup checklist.`
Correction: the standard is a formal requirements-engineering reference; this episode's lightweight tool is our synthesis and does not claim universal ISO applicability.

---

## 12. Closing listener action

### 20-minute exercise
Take the product you are building now.
Do not write the whole specification.
Write only the 10–20 requirements/constraints that would materially change the next prototype or architecture decision if they changed.

For each, add:
`status → rationale/source → verification idea → owner → unresolved learning → expiration trigger`.

Then circle every field where two disciplines could currently be assuming different answers.

That becomes tomorrow's engineering conversation.

---

## 13. Closing handoff to A2

Closing idea:
> Once the team agrees what must be true, the next failure mode is equally predictable: everyone assumes somebody else owns making it true.

A2 moves from **product truth** to **discipline/ownership truth**.

---

## 14. Source-note skeleton generated from this outline

### Spoken/source-worthy external anchors
1. NASA SEH §4.1/§4.2 — stakeholder constraints and technical requirements categories.
2. NASA SEH §6.2 — traceability and managed requirement change.
3. NASA SEH §5.3 + Appendix D — verification linkage/records.

### Show-notes-only standards context unless narration needs it
4. ISO/IEC/IEEE 29148:2018 — current published requirements-engineering standard identity/scope/status as checked 2026-09-10.
5. ISO/IEC/IEEE DIS 29148 Edition 3 — revision-watch only; not current normative edition.

### Internal tools to label as ours
- Minimum Useful Requirements Sheet.
- Requirement Quality Check.
- assumption/TBD expiration logic.
- DEV/LVP/SVP implementation framing.

---

## 15. P0 check before full script draft

Planned unsupported normative claims: 0.
Planned consequential sourced claims without source-lock anchors: 0.
Planned quantitative claims requiring arithmetic lock: 0.
Product-specific compliance claims: 0.
Real-world factual case claims: 0 — cold open is explicitly illustrative.

## 16. Gate

Technical content architecture: PASS.
Source ownership: PASS.
Applicability: PASS.
Episode-boundary discipline: PASS.
Narrative flow: PASS.

**A1 SCRIPT OUTLINE: COMPLETE — READY FOR FULL SCRIPT DRAFT**
