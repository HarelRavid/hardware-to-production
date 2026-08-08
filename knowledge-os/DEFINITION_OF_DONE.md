# Definition of Done

**Baseline: v1.0**

## 1. Purpose

This document defines when a Knowledge Object, Module, Domain or podcast section is mature enough to support production of the podcast without substantial new foundational research.

## 2. Object Readiness Checklist

A Knowledge Object may become `Podcast Ready` only when, where applicable:

- [ ] Definition is clear and terminology/aliases are resolved.
- [ ] Engineering Meaning and Decision Impact are explained.
- [ ] Lifecycle position is mapped.
- [ ] Typical owners/responsible roles are identified where meaningful.
- [ ] Inputs and outputs are documented.
- [ ] Decision criteria and tradeoffs are explained.
- [ ] Important limitations and failure conditions are captured.
- [ ] Common mistakes are documented.
- [ ] Relevant standards/regulations were searched and classified.
- [ ] Core academic/professional evidence was reviewed.
- [ ] Authoritative books/handbooks were checked where available.
- [ ] Useful industrial guidance was reviewed.
- [ ] At least one practical or case-study layer exists where meaningful.
- [ ] Relationships to upstream/downstream Objects are typed and justified.
- [ ] Important relationships include evidence/confidence/provenance.
- [ ] Major contradictory evidence is preserved through Claims/Knowledge Conflicts.
- [ ] Open Questions are explicitly listed.
- [ ] Material Engineering Assumptions are explicit.
- [ ] Questions Answered are mapped.
- [ ] Listener-facing tags are assigned.
- [ ] Important Claims have external evidence beyond GNR-only provenance.
- [ ] No substantial foundational research is expected to be needed merely to write the episode discussion.

## 3. Source Quantity Is Not a Gate by Itself

There is deliberately no universal minimum number of sources. Different topics have different evidence ecosystems.

A standard-defined method may require fewer but stronger sources. A contested manufacturing-selection topic may require many independent sources.

Evidence quality, independence, context and applicability matter more than raw source count.

## 4. Module Readiness

A Module may be considered mature when:

- its core Objects are mapped;
- episode-critical Objects meet Object Readiness;
- major Questions Answered have traceable answers;
- key Decisions are supported by Claims;
- important Failure Modes / common mistakes are represented;
- evidence gaps and Open Questions are visible;
- cross-Module dependencies are typed.

## 5. Domain Completion Criteria

Where applicable, a process/engineering Domain should cover:

- Fundamentals / terminology
- Relevant physics or process principles
- Materials
- Design rules / engineering constraints
- Tooling / equipment
- Process flow / operations
- Quality / inspection / measurement
- Failure modes
- Economics / cost and lead-time drivers
- Automation / scalability implications
- Lifecycle / prototype-to-production implications
- Standards and regulations
- Academic / professional literature
- Industrial guidance
- Engineering Claims
- Engineering Decisions
- Case Studies
- Why Projects Fail / common systemic mistakes
- Knowledge Conflicts / Open Questions
- Cross References
- Podcast / listener navigation layer

Not every Domain requires equal depth in every category. `Not applicable` should be explicit rather than silently omitted.

## 6. Knowledge Integrity Review

Before a major Domain or podcast section is declared complete, perform an integrity audit for:

- [ ] duplicate concepts / duplicate IDs;
- [ ] orphan Objects;
- [ ] unsupported or GNR-only episode-critical Claims;
- [ ] Decisions whose branches lack evidence or explicit heuristic labels;
- [ ] hidden Engineering Assumptions;
- [ ] unresolved Knowledge Conflicts not visible to the reader;
- [ ] numerical values missing context;
- [ ] manufacturer-specific rules represented as universal limits;
- [ ] missing lifecycle connections;
- [ ] missing Questions Answered;
- [ ] missing provenance;
- [ ] substantial foundational research gaps.

## 7. Podcast-Oriented Domain Review

Before episode architecture begins, each major Domain should contain a useful listener-facing set of:

- key Questions;
- common Decisions;
- common Mistakes / failure patterns;
- common Myths or misconceptions where relevant;
- Lessons Learned / Case Studies.

`20` is a useful target for broad Domains, not an artificial quota. Smaller Domains may require fewer; large Domains may require more. Coverage and usefulness are the gate.

## 8. Podcast Section Readiness

A podcast section (Prototype Workshop, Designing for Manufacturing, NPI & Industrialization) is ready for episode architecture only when:

- its major Domains/Modules are mapped;
- core Objects are at least `Verified` or `Referenced`;
- episode-critical Objects are `Podcast Ready`;
- major cross-domain dependencies are visible in the graph;
- evidence gaps are known rather than hidden;
- the Knowledge Integrity Review has been completed.

## 9. Episode Readiness

An episode may enter writing only when:

- the episode question/purpose can be answered from the Knowledge OS;
- key Claims have traceable external evidence;
- mandatory vs recommended practice is separable;
- listener tags point to mature Objects;
- prerequisites are identifiable;
- practical examples/case studies exist where needed;
- unresolved uncertainty is explicit;
- important assumptions and conflicts are visible;
- no major architecture or foundational research work is expected during writing.

## 10. Architecture Stability Rule

If writing an episode reveals that the Knowledge OS requires major restructuring, stop episode writing and treat the issue as an architecture/research gap. The podcast does not silently redefine the Knowledge OS.

Knowledge OS v1.0 is the stable architecture baseline; routine content development should extend the knowledge within it rather than modify the model.