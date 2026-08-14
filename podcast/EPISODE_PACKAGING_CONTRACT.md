# Episode Packaging Contract — Hardware-to-Production Podcast

status: FINAL QA — FREEZE GATE
version: 1.0
purpose: Define the minimum evidence/editorial package required for any episode to progress from Knowledge Backbone coverage to PODCAST READY.

## 1. Principle

An episode is not a narrated summary of the Data Hub.
It is a controlled publication package built from verified claims, scoped applicability, worked evidence and an explicit audience/lifecycle objective.

Canonical pipeline:

Backbone topic → Episode claim set → Source verification → Applicability → Worked example / case evidence → Audience framing → Technical review → Script/outline → Show notes/source pack → PODCAST READY

## 2. Required episode metadata

Every episode pack must contain:

- Episode ID / title
- Season / part
- Primary audience: A / B / both
- Secondary audience
- Lifecycle position: DEV / LVP / SVP / cross-stage
- MASTER_WBS mappings
- P2 canonical package mappings
- Prerequisites / recommended prior episodes
- Entry-point note: whether episode can stand alone
- Estimated technical depth: foundation / practitioner / advanced
- Publication status

## 3. Audience contract — mandatory

Every technical episode must answer, where relevant:

1. DEV takeaway — what should an early team understand or do now?
2. Prototype shortcut — what temporary solution may be acceptable?
3. Shortcut expiration — what signal/condition means the shortcut must stop?
4. LVP change — what becomes necessary at tens/hundreds of units?
5. SVP evidence — what must be demonstrated before commercial serial production?
6. Manufacturing-debt prevention — what should be designed/documented now?
7. Listener action — what can the listener inspect, calculate, decide or create after the episode?

If a field is not applicable, the pack must state why rather than silently omit it.

## 4. Episode claim register

Each consequential statement in the episode must exist in a claim register.

Minimum fields:

| Field | Requirement |
|---|---|
| Claim ID | required |
| Claim text | required |
| Claim class | V1–V6 per SOURCE_VERIFICATION_BACKLOG |
| Priority | P0/P1/P2 |
| Source status | UNVERIFIED / SOURCE LOCATED / VERIFIED / TECHNICALLY REVIEWED / PACKAGED |
| Source | required for V1–V5 |
| Exact support location | required for P0 normative/critical claims |
| Applicability | required |
| Source says | required for interpretive claims |
| We conclude | required when synthesis/inference is present |
| Episode use | core / supporting / optional |

P0 claims cannot appear in a final script as authoritative guidance until VERIFIED + TECHNICALLY REVIEWED.

## 5. Standards / normative claims gate

Any statement of the form:
- “ISO/IEC/ISA/ASTM/ASME/AIAG requires…”
- “the standard defines…”
- “you must…” because of a named standard/regulation

must contain:

- exact standard designation;
- edition/year/status;
- applicability/jurisdiction;
- clause/table/figure or equivalent exact location when available/required;
- distinction between normative requirement and guidance;
- no unsupported transfer of a requirement between industries/applications.

Secondary summaries may aid discovery but cannot silently replace the authoritative source for a P0 normative claim.

## 6. Quantitative gate

For every number that affects an engineering conclusion:

- units must be explicit;
- equations/formulas must be recorded;
- assumptions must be listed;
- input evidence class must be known;
- arithmetic must be independently checked;
- sensitivity must be shown when one uncertain variable can reverse the recommendation;
- pedagogical/Sentinel numbers must be labeled as illustrative, not field data.

Examples include:
- takt/capacity;
- OEE;
- FPY/yield/rework;
- capability indices;
- NPV/IRR/break-even;
- sample-size or acceptance thresholds;
- reliability/qualification numbers.

## 7. Applicability Statement — mandatory for standards-heavy episodes

Each standards-heavy episode must include at least one explicit applicability statement:

- product/process/system covered;
- lifecycle stage;
- configuration/process envelope;
- jurisdiction/industry if relevant;
- assumptions;
- exclusions;
- what change would force reassessment.

Example structure:

> This requirement/guidance is applied here to [system/process] under [conditions]. It is not being generalized to [excluded scope]. A change in [key dependency] requires applicability/evidence reassessment.

## 8. Worked example requirement

Every practitioner/advanced technical episode should include at least one of:

- Sentinel Node worked example;
- numerical example;
- process decision example;
- failure/reaction scenario;
- supplier/change scenario;
- manufacturing-data reconstruction;
- real-world case study.

The example must demonstrate the framework rather than merely restate it.

## 9. Case-study packaging rules

A case study must separate:

FACT
SOURCE INTERPRETATION
OUR FRAMEWORK LESSON

Required:
- primary/official evidence where available;
- exact dates/population/configuration where material;
- no causal claim stronger than source support;
- no blame language where system/process analysis is sufficient;
- explicit domain-transfer limitation;
- distinction between what was known at the time and hindsight.

## 10. Canonical frameworks reuse rule

Episodes must reuse canonical frameworks rather than invent synonymous alternatives.

Current reusable framework family includes, where relevant:
- Hardware Evolution Ladder
- DEV / LVP / SVP Lens
- Hardware Manufacturing Readiness Matrix
- QUALITY CHAIN 8
- RATE 8
- RAMP 10
- ECON 10
- SUPPLIER 10
- CHANGE 9
- AUTOMATE 10
- LOSS 8
- RELEASE 12
- TRACE 10
- RECONSTRUCT 8
- ATLAS 10
- SECURITY 12
- SECURE RELEASE 12
- CASE 12

These are internal synthesis frameworks unless explicitly documented otherwise.

## 11. Global-invariant gate

No episode may contradict the V1 global invariants:

1. Evidence supports a defined claim inside a defined applicability/configuration envelope.
2. Change invalidates only the evidence dependencies it actually affects.
3. Definition, execution/as-built state and evidence are distinct but traceably linked.
4. Rework adds history; it does not erase failed history.
5. Measurement adequacy precedes confidence in capability/quality conclusions.
6. Accepted sustainable throughput matters more than isolated machine speed/short peak rate.
7. OEE is a loss lens, not root-cause or system-capacity proof.
8. Approval is valid only inside the demonstrated envelope.
9. Cyber/configuration events that alter manufacturing can invalidate manufacturing evidence.
10. “Running again” is not full recovery until configuration, quality, WIP/genealogy and release evidence are trustworthy.

If an episode appears to require an exception, that is a backbone change request, not an editorial shortcut.

## 12. Case-study repair visibility

Episode packs must use the following cross-domain repairs where relevant:

- FIELD EVIDENCE LOOP
- MINIMUM CONTROLLED PRODUCTION MODE
- INTERACTION CLAIM
- MOVING CONSTRAINT LOOP
- STAGED CAPEX OPTION
- INDUSTRIALIZATION SUPPLIER
- EFFECTIVENESS EVIDENCE
- SIGNAL AGGREGATION
- FIELD EVENT

If a repair is renamed editorially, the canonical object mapping must remain explicit.

## 13. Required episode structure

Default technical episode structure:

1. Hook / failure or decision the listener recognizes
2. Why the problem changes from DEV → LVP → SVP
3. Core concept/framework
4. What teams commonly get wrong
5. Worked example / Sentinel / case
6. Decision method / checklist
7. Standards/evidence/applicability where relevant
8. What to do now
9. What will be required next at higher maturity
10. Summary of listener tool / takeaway

Episodes may vary narratively, but all contract elements must remain represented in the research pack.

## 14. Required source pack

Before PODCAST READY each episode must have:

- claim register;
- source list;
- P0 verification complete;
- exact clause/page references for critical normative claims where applicable;
- quantitative check sheet;
- case-study fact sheet if applicable;
- unresolved-claim list;
- standards/applicability notes;
- licensing/citation note for any controlled standards content;
- proposed show-note references.

## 15. Technical review gate

Technical review must explicitly check:

- factual correctness;
- normative accuracy;
- applicability;
- units/calculations;
- source-vs-synthesis separation;
- DEV/LVP/SVP distinctions;
- failure-mode realism;
- no hidden assumption that a prototype result equals production capability;
- no hidden assumption that process capability equals product performance;
- no hidden assumption that component compliance proves system compliance;
- no cross-industry requirement transfer without explanation.

## 16. Editorial review gate

Editorial review must check:

- audience entry point is clear;
- prerequisite burden is controlled;
- jargon is defined before use;
- episode teaches decisions, not just vocabulary;
- at least one actionable listener tool exists;
- story/example supports the engineering lesson;
- repetition with other episodes is intentional and framed;
- the listener understands what comes next in the lifecycle.

## 17. Episode maturity states

### BACKBONE COVERED
Topic exists in Data Hub / P2 packages.

### RESEARCH PACK OPEN
Episode-specific claims and sources are being assembled.

### EVIDENCE VERIFIED
P0 claims are verified; applicability and calculations are controlled.

### TECHNICALLY REVIEWED
Engineering review complete; critical comments closed or explicitly accepted.

### SCRIPT READY
Narrative/script can be written without inventing technical truth.

### PODCAST READY
Technical + editorial + source-note + show-note package passes.

### PUBLISHED
Final released episode and source notes archived with version/date.

## 18. Freeze boundary

Knowledge Backbone V1 freeze does NOT freeze:
- exact scripts;
- episode order refinements that do not alter technical truth;
- future case additions;
- new source evidence;
- standards edition updates;
- improved examples;
- listener wording.

V1 freeze DOES baseline:
- domain architecture;
- canonical backbone chain;
- global invariants;
- P2.01–P2.10 canonical concepts;
- audience mission and DEV/LVP/SVP model;
- claim/evidence/applicability model;
- Source Verification Backlog method;
- this Episode Packaging Contract.

Post-freeze structural changes require a documented gap and controlled change decision.

## 19. Freeze-gate checklist contributed by this contract

Knowledge Backbone V1 may be frozen when:

1. P2.01–P2.10 are NEAR PODCAST READY at backbone level;
2. cross-framework contradiction audit passes;
3. global invariants are explicit;
4. Source Verification Backlog exists;
5. audience/stage re-audit passes;
6. Episode Packaging Contract exists;
7. controlled gaps are visible and do not require architecture redesign;
8. no known normative/source gap is being disguised as COMPLETE/PODCAST READY.

## 20. Result

This contract closes the final methodological gap between a technically rich knowledge base and a repeatable, reviewable podcast-production system.

Recommended next action:

Run the formal Knowledge Backbone V1 Freeze Decision and publish a baseline record containing:
- freeze scope;
- included canonical artifacts;
- known controlled gaps;
- post-freeze change rule;
- baseline commit SHA.
