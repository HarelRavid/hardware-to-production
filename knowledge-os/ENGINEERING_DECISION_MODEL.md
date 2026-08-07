# Engineering Decision Model

## Purpose

The Knowledge OS must help engineers answer not only `What is X?` but also `Given my constraints, what should I do?`

Engineering Decisions sit above claims and objects. They consume validated claims and turn them into explicit decision logic.

## Decision ID

Format:

`H2P-DEC-XXXXXX`

## Canonical Decision Schema

```yaml
id: H2P-DEC-XXXXXX
title:
question:
domain:
lifecycle: []
status: Draft
inputs: []
constraints: []
candidate_options: []
required_claims: []
related_objects: []
outputs: []
last_reviewed:
```

## Decision Structure

Every decision should define:

1. Engineering question.
2. Required input information.
3. Constraints and disqualifiers.
4. Candidate options.
5. Claims used to discriminate between options.
6. Tradeoffs.
7. Recommendation logic.
8. Escalation path when information is insufficient.
9. Exceptions.
10. Links to detailed Knowledge Objects.

## Decision Output Types

- Select one option.
- Rank alternatives.
- Eliminate unsuitable options.
- Request additional test/data.
- Escalate to specialist review.
- Defer the decision until lifecycle maturity increases.

## Decision Tree Rule

Decision trees must not encode unsupported folklore as deterministic truth.

Each branch should be traceable to one or more Engineering Claims or clearly marked Project Heuristics.

Example:

```text
Need plastic prototype
  ↓
Is production-material behavior part of the learning objective?
  ├─ No → rapid polymer AM may be suitable
  └─ Yes
       ↓
Is the intended production material/process reproducible by the prototype process?
       ├─ Yes → evaluate process-specific route
       └─ No → consider CNC, soft tooling or production-representative prototype
```

## Engineering Pitfalls

Pitfalls describe recurrent failure modes in engineering reasoning or execution.

Schema:

```yaml
id: H2P-PIT-XXXXXX
statement:
why_it_fails:
applicable_context: []
related_claims: []
related_objects: []
prevention:
confidence:
```

Examples include:

- treating feedstock datasheet properties as printed-part properties;
- using printer pixel/nozzle resolution as dimensional accuracy;
- testing an XY-oriented coupon while the real load acts through Z interfaces;
- using a visually representative prototype to validate production-process behavior.

## Engineering Heuristics

Heuristics are useful shortcuts, explicitly non-normative.

Schema:

```yaml
id: H2P-HEU-XXXXXX
statement:
context:
rationale:
related_claims: []
exceptions: []
confidence:
```

Heuristics must never be presented as standards or facts.

## Engineering Questions

Questions are listener- and engineer-facing entry points into the graph.

Format:

`H2P-Q-XXXXXX`

A question should connect to one or more Decision Objects.

Examples:

- Which prototyping process should I use for this part?
- Should I build this prototype in-house or outsource it?
- When is a prototype sufficiently production-representative for DVT?
- Do I need an insert, printed thread or tapped hole?
- Which measurement method is adequate for this feature?

## System Stack

The intended reasoning path is:

`Engineering Question → Decision → Claims → Knowledge Objects → Sources`

The inverse path also exists:

`Source → Extracted Claims → Objects / Relationships → Decisions → Podcast explanation`

## Recommendation Rule

Project recommendations must state whether they are:

- directly required by evidence;
- a strong synthesis of evidence;
- a conservative engineering recommendation;
- a Project Heuristic.

Do not hide judgment behind citations.
