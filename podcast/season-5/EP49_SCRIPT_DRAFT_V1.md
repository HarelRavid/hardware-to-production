# EP49 Full Script Draft V1 — Standards, Claims and Evidence as a Manufacturing Knowledge Graph

status: FULL SCRIPT DRAFT V1 — SCRIPT REVIEW NEXT
season: Season 5 — Automation, Data and the Connected Factory
source_outline: EP49_SCRIPT_OUTLINE_V1.md
source_lock: evidence/source-lock/wave-05/
spoken_normative_standard_claims: NONE

## Production note — not spoken

"Knowledge graph" describes linked engineering objects/relationships. This episode does not require or prescribe a graph database. Protected standards content is never reproduced; citation metadata and applicability are controlled separately.

# SPOKEN SCRIPT

## Opening

An engineer opens a folder and finds the document everybody has been looking for.

A test report.

The material passed.

Problem solved.

Then someone asks:

Which requirement did this test address?

Which product revision?

Which supplier?

Which process?

Was the sample production representative?

Did a later material change invalidate it?

Nobody knows.

The PDF exists.

The engineering claim has lost its context.

That is the problem for this episode.

Search can find documents.

Engineering has to know:

**What claim does this evidence support, under which conditions, and why should we still trust it now?**

---

## 1. A document is a container

A standard.

Test report.

Supplier certificate.

FMEA.

Lab notebook.

Email.

Inspection report.

These are containers of information.

The engineering object we care about may be:

A requirement.

A claim.

An assumption.

An evidence record.

An applicability statement.

A decision.

A change dependency.

If we store only documents, later users have to reconstruct those relationships from memory.

That reconstruction is expensive.

And sometimes impossible.

So the knowledge architecture should preserve the relationship, not only the file.

---

## 2. Start with the question and claim

Suppose the question is:

Can this enclosure material survive the intended chemical exposure?

The claim might be:

Material X in configuration Rev C meets the defined exposure requirement under condition Y.

Now evidence can attach to that claim.

Test report.

Material certificate.

Supplier data.

Field evidence.

Each piece has a role.

The source and evidence do not become the claim automatically.

Engineering makes the conclusion.

That distinction matters because a source can say something narrower than the conclusion someone wants to draw.

So preserve:

Source says.

Evidence shows.

We conclude.

Those are different objects.

---

## 3. Applicability is not optional context

A test passes.

For what configuration?

Which material lot?

Which temperature?

Which process route?

Which supplier?

Which sample preparation?

Which firmware?

Which test method?

Evidence is not infinitely reusable.

It supports a claim inside an envelope.

That is one of the frozen invariants of this project.

If the context changes, we do not automatically delete the evidence.

We ask whether the change touched the dependency that made the evidence valid.

That is evidence impact analysis.

---

## 4. One evidence item can support many claims—and one claim can need many evidence items

A sealing test might support:

Ingress requirement.

Assembly torque decision.

Gasket-material approval.

Supplier qualification.

But not necessarily all of them to the same strength.

And one release claim may need:

Dimensional evidence.

Material evidence.

Functional test.

Process validation.

Supplier status.

So the graph is many-to-many.

That is why a folder tree eventually becomes weak.

A file lives in one folder.

Engineering evidence lives in multiple relationships.

---

## 5. Standards need more than a name

A standard citation is not:

“ISO says so.”

For a consequential normative claim, you need the right designation, edition/status, applicability and exact support location when required.

And licensing still matters.

A knowledge system should not casually copy protected standards text into every database.

It can preserve:

Standard identity.

Edition.

Scope.

Clause/location metadata.

Applicability statement.

Controlled access to the source.

That gives engineers a traceable path without turning the repository into an unauthorized standards mirror.

---

## 6. Change should trigger dependency review

A supplier changes.

Do we invalidate every test ever performed?

No.

Do we keep every test because the part number did not change?

Also no.

Ask:

Which claims depended on the supplier/process/material attribute that changed?

Which evidence assumed the old state?

Which evidence remains applicable?

This is where a claim/evidence graph becomes operational.

It lets change control ask:

**What depends on this?**

That is much more useful than reopening every qualification document indiscriminately.

---

## 7. Contradictions and uncertainty should remain visible

Two sources disagree.

One test fails.

One passes.

Supplier data says one thing.

Field data says another.

Do not force the knowledge base to choose a clean answer too early.

Record the contradiction.

Record uncertainty.

Record evidence maturity.

Record reviewer status.

A manufacturing knowledge system should know what it does **not** know.

Otherwise GNR—good narrative reasoning—quietly becomes “fact.”

---

## 8. AI makes this boundary more important, not less

AI can retrieve.

Summarize.

Compare.

Suggest a synthesis.

That is useful.

But model confidence is not evidence maturity.

Search relevance is not source authority.

A fluent answer is not a verified engineering claim.

So derived AI output should retain:

Sources.

Scope.

Assumptions.

Model/version where consequence warrants it.

Review status.

The AI layer can help navigate the graph.

It should not silently become the graph's authority.

---

## 9. The Claim Evidence Card

Here is the listener tool.

Write:

Question.

Decision.

Claim.

Applicability or configuration envelope.

Evidence.

Source and exact location where needed.

Evidence maturity.

Reviewer.

Related requirements or objects.

Change dependencies.

Decision use.

Try this on one consequential engineering claim.

If half the card is blank, the document archive may be strong while the evidence architecture is weak.

---

## 10. Knowledge graph does not mean graph database

This is worth saying explicitly.

You can implement these relationships in:

A graph database.

Relational database.

PLM links.

Structured files.

A lightweight knowledge platform.

The engineering requirement is the relationship.

Not the database technology.

Choose implementation based on scale, query needs, integration and governance.

Do not buy graph technology because the architecture uses the phrase “knowledge graph.”

---

## 11. DEV to LVP to SVP

In DEV, a lightweight claim/evidence note may be enough.

In LVP, supplier, process and test evidence starts multiplying.

Link it to configuration before reconstruction debt becomes painful.

In SVP, governance matters.

Reviewer maturity.

Access.

Change impact.

Standards status.

Retention.

The same conceptual graph grows in rigor.

---

## 12. Six traps to avoid

PDF repository equals knowledge base.

Search rank equals evidence strength.

Standard name without edition or applicability.

Source and conclusion merged.

AI synthesis stored as verified fact.

Change means either invalidate everything or invalidate nothing.

---

## 13. The action after this episode

Pick one important test report.

Do not summarize it.

Write the exact engineering claim it supports.

Then write:

For which configuration?

Under which conditions?

Which decision uses it?

What change would make you reassess it?

That turns the document into engineering knowledge.

---

## Closing

EP49 tells us how to preserve claims and evidence.

Now we can ask a more useful question.

Can this knowledge system help engineers make decisions?

Not retrieve facts.

Decide between alternatives.

That is Episode 50:

**The Manufacturing Atlas: Turning Knowledge into Decisions.**

# End spoken script

## Draft source anchors — not spoken

- Wave 01 — source/claim/applicability and change-impact discipline.
- W5-S04/S05/S06 — digital thread, durable identity and provenance context.
- claim/evidence graph structure is Hardware-to-Production synthesis.
