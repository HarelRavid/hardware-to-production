# Knowledge OS Research Workflow

## 1. Objective

Research exists to mature predefined Knowledge Objects, create defensible Engineering Claims and Relationships, and support explicit Engineering Decisions. The goal is not to accumulate links.

## 2. Step 1 — Map the Research Space

Before searching, define:

- target Domain and Subdomain;
- candidate Knowledge Objects;
- Engineering Questions the domain must eventually answer;
- candidate Engineering Decisions;
- key research questions;
- expected lifecycle relevance;
- likely standards bodies and source families;
- known neighboring Objects.

## 3. Step 2 — Create / Confirm Object IDs

Each candidate Object receives a stable ID and status `Mapped` before significant research is attached to it.

If research reveals a genuinely separate concept, create a new Object instead of overloading an existing one.

## 4. Step 3 — Search by Evidence Layer

Recommended sequence:

1. standards and regulations;
2. government and research institutes;
3. universities and academic literature;
4. books and handbooks;
5. industry associations and high-quality manufacturer literature;
6. courses, conferences and expert lectures;
7. professional practice sources.

Search in both English and Hebrew when meaningful. Do not force Hebrew sources when stronger authoritative material exists only in English.

## 5. Step 4 — Register Sources

Each source should be entered into the source index with:

- source ID;
- title;
- author / organization;
- publication date/version;
- source type;
- authority tier;
- language;
- URL / locator;
- access status;
- Objects / Claims supported;
- read status;
- last verification date.

## 6. Step 5 — Extract Engineering Claims

The source itself is not the final knowledge product.

For every meaningful source ask:

1. Which Engineering Claims does this source support?
2. Which existing Claims does it refine, qualify, limit or contradict?
3. Under what material/process/lifecycle/environmental context is each Claim valid?
4. Which Engineering Decisions can use the Claim?

Extract, when relevant:

- explicit definitions;
- normative requirements;
- quantitative limits;
- decision criteria;
- process sequences;
- advantages / limitations;
- causal statements;
- lifecycle implications;
- terminology differences;
- failure mechanisms;
- exceptions;
- unresolved questions.

Claims follow `ENGINEERING_CLAIM_MODEL.md`.

## 7. Step 6 — Preserve Context for Numerical Claims

Never store a numerical engineering value without enough context to interpret it.

Capture as applicable:

- material / grade;
- machine / process family;
- parameter set;
- orientation;
- specimen / feature geometry;
- conditioning;
- post-processing;
- test method / standard;
- temperature / humidity / environment;
- sample size and uncertainty where available.

Do not convert a narrow datasheet or experiment into a universal process capability.

## 8. Step 7 — Build Relationships During Research

Whenever research demonstrates a logical connection between Objects, Claims, Decisions or Sources, create the typed relationship immediately.

Every meaningful relationship includes:

- type;
- direction;
- inverse where defined;
- reason;
- strength;
- confidence;
- evidence.

Do not postpone graph creation until the end of research.

## 9. Step 8 — Triangulate Important Claims

Seek multiple independent sources for Claims that materially affect engineering decisions, especially:

- safety;
- regulatory requirements;
- process capability;
- material compatibility;
- manufacturing selection;
- reliability;
- dimensional / mechanical performance;
- cost/scaling rules;
- causal failure claims.

Manufacturer-specific data may remain single-source when the Claim is explicitly limited to that manufacturer's material/machine/process context.

## 10. Step 9 — Preserve Disagreement

When credible sources disagree:

- retain both Claims or evidence positions;
- identify scope/context differences;
- create contradiction/qualification relationships where appropriate;
- seek a narrower context that may reconcile them;
- avoid premature Project Recommendations.

## 11. Step 10 — Build Engineering Decisions

Once enough Claims exist, convert recurring engineering questions into Decision Objects.

For each decision define:

- input variables;
- constraints/disqualifiers;
- candidate options;
- Claims that discriminate between options;
- tradeoffs;
- exceptions;
- escalation path when evidence is insufficient.

Decision branches must be traceable to Claims or explicitly marked Project Heuristics.

## 12. Step 11 — Capture Pitfalls and Heuristics

During research, record recurrent reasoning or execution mistakes as Engineering Pitfalls.

Record useful non-normative shortcuts as Engineering Heuristics.

Never mix Pitfalls/Heuristics with normative requirements or Verified Facts.

## 13. Step 12 — Synthesize

Only after evidence collection should the project produce a synthesis or recommendation.

Project Synthesis must be visibly distinguishable from normative requirements, Academic Consensus, Industrial Best Practice or manufacturer guidance.

## 14. Step 13 — Review for Graph Completeness

Before marking an Object `Reviewed`, verify:

- it has appropriate upstream/downstream links;
- important assertions exist as Claims rather than unsupported prose;
- no important referenced concept lacks an Object;
- vague `related to` links have been replaced by typed relationships;
- lifecycle tags are correct;
- major standards and evidence families have been checked;
- key Engineering Questions have a path toward Decision Objects.

## 15. Step 14 — Validate Podcast Coverage

Before `Podcast Ready`, confirm that the Object cluster can support the expected discussion without requiring new foundational research.

The expected path should exist:

`Listener Question → Decision → Claims → Objects → Sources`

The podcast should be able to explain both the knowledge and the practical decision consequences.

## 16. Source Status

Recommended source state progression:

Found → Accessed → Read → Claim-Extracted → Cross-checked → Linked → Cited

## 17. Claim Status

Candidate → Extracted → Corroborating → Reviewed → Validated → Published

Alternative terminal/intermediate states:

- Disputed
- Superseded

## 18. Research Quality Rule

A large number of sources does not equal maturity. Prefer a smaller set of authoritative, complementary sources over repetitive low-authority material.

Likewise, a large number of Claims does not equal maturity. Prefer atomic, useful, correctly scoped Claims over fragmented trivia.

## 19. Link Maintenance

Public listener-facing sources should be periodically checked for broken links or superseded editions. Standards should include edition/year information wherever possible.
