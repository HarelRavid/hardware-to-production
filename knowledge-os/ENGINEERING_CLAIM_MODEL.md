# Engineering Claim Model

## Purpose

Engineering Claims are the atomic evidence-bearing units of the Hardware to Production Knowledge OS.

Knowledge Objects remain durable containers and graph nodes, but claims hold the specific statements that can be supported, limited, contradicted, refined, or used in engineering decisions.

## Core Rule

**Objects organize knowledge. Claims assert knowledge. Sources support claims. Decisions consume claims.**

A claim is never just copied text from a source. It is a concise engineering statement synthesized from evidence, with its applicability and limitations preserved.

## Claim ID

Format:

`H2P-CLM-XXXXXX`

Claim IDs are stable and must not be reused.

## Canonical Claim Schema

```yaml
id: H2P-CLM-XXXXXX
statement:
classification:
status: Draft
confidence:
evidence_level:
evidence_count: 0
applicable_context: []
limitations: []
exceptions: []
related_objects: []
supports_decisions: []
created:
last_reviewed:
```

## Claim Classification

Allowed primary classifications:

- Normative Requirement — required by a standard, law or regulation.
- Verified Fact — directly measurable or definitional fact supported by authoritative evidence.
- Academic Evidence — supported by one or more academic studies but not necessarily consensus.
- Academic Consensus — supported by a mature body of literature or authoritative review.
- Industrial Best Practice — widely used professional practice, not necessarily mandatory.
- Manufacturer-Specific Guidance — valid for a specified machine, material, process or supplier context.
- Expert Opinion — attributable professional judgment.
- Project Synthesis — conclusion synthesized by Hardware to Production from multiple sources.
- Project Heuristic — practical rule of thumb explicitly marked as non-normative.

## Confidence

- Very High — strong authoritative evidence with little meaningful contradiction in the stated scope.
- High — multiple strong sources or one highly authoritative source with good scope match.
- Medium — useful evidence exists but applicability, quantity or agreement is limited.
- Low — preliminary, weakly supported or highly context-dependent.
- Unknown — not yet evaluated.

Confidence is not the same as source authority. A high-authority source may support only a narrow claim.

## Evidence Level

Record the strongest evidence class supporting the claim and preserve all linked evidence.

Suggested levels:

1. Normative — standard/regulation directly states the requirement.
2. Authoritative — government laboratory, recognized handbook, formal institutional guidance.
3. Peer-reviewed — academic paper or review.
4. Industrial — technical literature, validated application note, industry association guidance.
5. Experiential — expert practice, case study, specialist professional experience.

## Required Claim Fields

Every validated claim must include:

1. Statement — one clear engineering assertion.
2. Classification.
3. Confidence.
4. Applicable Context — process, material, lifecycle, geometry, environment or industry boundary where relevant.
5. Limitations / Exceptions where known.
6. At least one related Knowledge Object.
7. Evidence links.
8. Engineering decision relevance when applicable.

## Claim Relationships

Claims may connect using controlled relations such as:

- SUPPORTED_BY → Source
- CONTRADICTED_BY → Source or Claim
- REFINES → Claim
- QUALIFIES → Claim
- LIMITS → Claim
- SUPERSEDES → Claim
- DERIVED_FROM → Claim(s)
- APPLIES_TO → Object
- DOES_NOT_APPLY_TO → Object / Context
- SUPPORTS_DECISION → Decision Object
- SUPPORTS_HEURISTIC → Heuristic
- SUPPORTS_PITFALL → Engineering Pitfall

Claim-to-claim contradictions must be preserved rather than silently resolved. The resolution, if one exists, should usually be encoded as a narrower context or a new synthesis claim.

## Atomicity Rule

Prefer one falsifiable or assessable statement per claim.

Bad:
`FDM is cheap, fast, inaccurate and weak in Z.`

Better:
- FDM can offer short in-house iteration lead time for suitable prototype geometries.
- Mechanical behavior of FDM parts can be build-orientation dependent.
- Dimensional accuracy cannot be inferred solely from nominal nozzle or layer resolution.

## Context Rule

Claims containing numerical values must preserve the context required to interpret the value, such as:

- material grade;
- machine / process family;
- build orientation;
- specimen geometry;
- conditioning;
- post-processing;
- test standard / method;
- environmental conditions.

Do not create universal numbers from manufacturer-specific or experiment-specific data.

## Claim Lifecycle

`Candidate → Extracted → Corroborating → Reviewed → Validated → Published → Superseded`

A claim may remain `Disputed` when credible evidence conflicts.

## Source Extraction Rule

For every meaningful source, ask:

1. Which engineering claims does this source support?
2. Which existing claims does it refine, limit or contradict?
3. What context is required for the claim to remain valid?
4. Which engineering decisions can use this claim?

The source itself is not the final knowledge product.
