# Script Outline Contract — Hardware-to-Production Podcast

status: CANONICAL PUBLICATION-PACKAGING CONTROL
version: 1.0
created: 2026-09-10
backbone_change: NO — editorial/publication layer over frozen Knowledge Backbone V1

## 1. Purpose

Define the minimum structure required before an episode moves from verified research/technical review into full narration/script drafting.

A script outline is not a shorter Production Blueprint. It is the **claim-by-claim narrative execution plan** that determines:
- what is said;
- in what order;
- which source supports each consequential statement;
- which language is external fact/guidance versus our synthesis;
- which examples are real, fictional or illustrative;
- what the listener should decide/do at the end.

## 2. Entry gate

Do not open a script outline until:
1. Production Blueprint is complete;
2. consequential claim set is stable;
3. P0 source/claim blockers for the intended script scope are locked or explicitly excluded;
4. applicability boundaries are defined;
5. a technical review has identified wording/technical guards.

If the script introduces a new consequential claim not present in the locked claim set, return that claim to Source Verification before drafting it as fact/guidance.

## 3. Required outline metadata

Every outline must state:
- Episode ID/title;
- canonical season;
- audience;
- lifecycle position;
- source-lock record(s);
- technical-review record;
- Production Blueprint source;
- outline status;
- whether the episode can stand alone / recap burden.

## 4. Required narrative objects

### A. Cold open / hook
Must be one of:
- real sourced case;
- explicitly fictional/composite scenario;
- Sentinel Node;
- practical decision/failure scenario.

Never present a composite as a real company/event.

### B. Listener promise
State what the listener will be able to understand, inspect, calculate, decide or create after the episode.

### C. Prerequisite recap
Include only concepts necessary to understand this episode.
Do not hide another full episode inside the recap.

### D. Teaching beats
For every major beat record:
- narrative point;
- claim ID(s);
- source anchor(s) or `V6 SYNTHESIS`;
- applicability/wording guard;
- example/tool used;
- transition to next beat.

### E. Listener tool execution
The episode must **use** its tool on an example rather than merely list the tool fields.

### F. DEV/LVP/SVP or lifecycle translation
Where relevant, explicitly show how the decision changes by maturity rather than repeating generic stage definitions.

### G. Closing action
Give one practical action/check/decision the listener can execute.

### H. Handoff
State why the next episode/deep dive logically follows.

## 5. Source language tags

Use these internal outline tags:

- `[FACT]` — sourced factual statement.
- `[AUTH-GUIDANCE]` — authoritative technical guidance with owner/applicability visible.
- `[NORMATIVE]` — exact standard/regulatory requirement; requires V1 lock.
- `[SYNTHESIS]` — Hardware-to-Production conclusion/framework.
- `[ILLUSTRATIVE]` — invented example/number/scenario.
- `[CASE-ATTRIBUTED]` — claim reported by a company/regulator/investigation where attribution matters.

These tags are production controls. They do not need to be spoken to the listener.

## 6. Source anchor rule

Every consequential `[FACT]`, `[AUTH-GUIDANCE]`, `[NORMATIVE]` or `[CASE-ATTRIBUTED]` beat must point to a source-lock ID or exact source record.

Do not rely on:
- memory;
- a Production Blueprint alone;
- a secondary blog when primary evidence was already locked;
- a standard name without edition/current status/applicability.

## 7. Normative-language rule

If the outline contains language equivalent to:
- `must because the standard requires`;
- `ISO/IEC/AIAG/FAA/FDA requires`;
- a mandated threshold/criterion;

then the beat must reference a V1 source lock with exact edition/status/applicability and location.

If that evidence is not available, rewrite as:
- our engineering recommendation;
- source-informed guidance;
- or remove the statement.

Do not soften an unsupported normative claim with vague words and leave the implication intact.

## 8. Quantitative rule

Every engineering-significant number in an outline must be tagged as one of:
- sourced measured/reported data;
- calculated from sourced inputs;
- illustrative assumption.

Calculated items require formula/units and independent arithmetic check before full script lock.

## 9. Case-study rule

For real cases preserve:
`FACT → SOURCE INTERPRETATION/ATTRIBUTION → OUR FRAMEWORK LESSON`.

The outline must identify where causation is established, attributed, uncertain or merely our synthesis.

## 10. Internal-framework rule

Canonical V6 tools/frameworks may be used freely when mapped correctly, but must not be described as external standards.

Examples:
- Hardware Evolution Ladder;
- DEV/LVP/SVP Lens;
- QUALITY CHAIN 8;
- CHANGE 9;
- RAMP 10;
- AUTOMATE 10;
- CASE 12;
- listener tools created for individual episodes.

## 11. Editorial density rule

An outline should prefer:
`recognizable problem → explanation → concrete example → decision/tool → consequence`

over long blocks of terminology.

Named standards should enter the spoken narrative only when they materially help the listener make a decision. Otherwise they belong in show notes/source pack.

## 12. Misconception guard

Each outline must include 3–8 misconceptions/overclaims that the full script must avoid or explicitly correct.

## 13. Script-ready gate

An outline may be marked `SCRIPT OUTLINE COMPLETE` when:
1. every narrative beat has claim/source/synthesis ownership;
2. technical-review guards are embedded;
3. no unresolved P0 claim appears in the planned narration;
4. examples are labeled real vs illustrative;
5. listener tool is executed, not only named;
6. episode boundaries with adjacent topics are respected;
7. source-note skeleton can be generated directly from the outline.

This does not equal PODCAST READY.

Next:
`SCRIPT OUTLINE COMPLETE → FULL SCRIPT DRAFT → EDITORIAL/TECHNICAL SCRIPT REVIEW → SOURCE NOTES → PODCAST READY GATE`.
