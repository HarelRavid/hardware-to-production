# Two-Character Dialogue Writing Style Contract

status: CANONICAL — CLAUDE WRITING CONTROL
version: 1.0
created: 2026-09-19
governed_by:
- podcast/OFFICIAL_PODCAST_DELIVERY_ROADMAP.md
- podcast/CLAUDE_EPISODE_HANDOFF_CONTRACT.md

## 1. Purpose

Control how Claude converts a verified episode package into the final two-character spoken dialogue intended for downstream NotebookLM production.

This contract controls writing style only.
It does not override Claim Locks, Technical Reviews, Source Registers or canonical episode ownership.

## 2. Speaker roles

### Speaker A — Lead Host / Systems Engineer
A should:
- frame the engineering decision;
- introduce concepts only when needed;
- explain causal/mechanism logic;
- preserve applicability and source-vs-synthesis boundaries;
- execute canonical frameworks accurately;
- connect DEV/LVP/SVP and adjacent episodes.

A should not:
- lecture for long uninterrupted blocks;
- sound like a standard or compliance auditor;
- answer every question before B can challenge it.

### Speaker B — Practitioner / Challenger
B should:
- be technically competent;
- challenge cost, practicality, necessity and overgeneralization;
- ask the listener's likely question;
- test concepts on a concrete example;
- expose hidden assumptions and common shortcuts;
- summarize what changes in practice.

B should not:
- be a naive student;
- exist only to say “right” / “exactly”;
- manufacture fake disagreement;
- introduce unsourced factual claims.

## 3. Dialogue rhythm

Preferred rhythm:
problem → challenge → mechanism → example → challenge → listener tool → practical consequence.

Avoid:
A monologue → B says “yes” → A monologue.

As a default, neither speaker should dominate more than roughly 65% of the spoken content.

This is an editorial balance, not a mathematical publication requirement.

## 4. Episode length class

Foundation/opening assets:
target approximately 18–25 minutes of spoken dialogue.

Practitioner technical episodes:
target approximately 22–32 minutes.

Case/synthesis episodes:
target approximately 25–35 minutes.

These are editorial targets, not hard limits.

Never remove a required technical distinction, applicability guard, calculation assumption or worked example merely to meet a duration target.

If the episode is too dense:
- move secondary standards metadata to show notes;
- compress repeated definitions into callbacks;
- keep the engineering decision/mechanism intact.

## 5. Spoken technical style

Use:
- natural technical language;
- short paragraphs/turns;
- physical examples;
- explicit cause/effect;
- concrete questions;
- occasional recap after dense material.

Avoid:
- long enumerations read mechanically;
- academic-paper prose;
- repeated “according to standard X” phrasing;
- unexplained acronyms;
- hype or marketing language.

## 6. Source attribution in audio

Natural attribution is required when ownership matters.

Examples:
- “NASA’s systems-engineering guidance treats…”
- “NIST’s reliability handbook warns that…”
- “The regulator’s report states…”

Do not read:
- URLs;
- claim IDs;
- file paths;
- citation syntax.

Standards should be named in audio only when the name materially helps the listener make the decision.

Edition/year detail normally belongs in source notes unless:
- current edition is itself important to the lesson;
- two editions/standards could change interpretation;
- a correction/update is part of the episode's warning.

## 7. Source vs synthesis language

External fact/guidance:
attribute naturally where useful.

Internal framework:
say “we’ll use…” / “our working tool is…” / “for this series…”

Never present:
- Hardware-to-Production frameworks;
- DEV/LVP/SVP;
- Atlas tools;
- readiness matrices;
- listener checklists

as external standards unless explicitly documented otherwise.

## 8. Illustrative examples

Invented/Sentinel scenarios are allowed and encouraged.

They must:
- remain obviously illustrative;
- never be described as a real company incident;
- use numbers only when already checked/approved;
- support the framework rather than distract from it.

## 9. Standards and normative language

Claude must never upgrade:
- “guidance suggests”
into
- “the standard requires”

unless the Claim Lock explicitly authorizes normative language.

If exact clause text is not locked:
- keep discussion conceptual;
- place exact standard identity in production/source notes.

## 10. Calculations and numbers

Every engineering-significant number must come from:
- a sourced factual record; or
- an approved illustrative example in the episode package.

For calculations:
- preserve units;
- preserve assumptions;
- explain what the calculation does NOT prove.

Do not invent “typical” thresholds.

## 11. Listener tools

Every episode's primary listener tool must be USED, not merely listed.

Dialogue should:
1. explain the tool's decision job;
2. run it on a concrete example;
3. show what decision changes as a result.

Avoid reading every field as a checklist unless that field is needed in the example.

## 12. DEV / LVP / SVP

Use the lifecycle lens only when it changes the decision.

Do not repeat the full definitions of DEV/LVP/SVP every episode.

Use callbacks such as:
- “At DEV, that shortcut can be reasonable…”
- “Once you enter repeated LVP builds…”
- “At SVP, the evidence burden changes because…”

## 13. Callbacks and adjacent episodes

Do not re-teach a prior episode.

Use a concise callback:
“As we established in A4…”

Then add only the new decision layer.

The handoff at the end should explain why the next episode is the next question, not act as an advertisement.

## 14. Production notes

Claude may include a separate section after the dialogue:

PRODUCTION NOTES — NOT SPOKEN

Allowed:
- pronunciation notes;
- optional diagram cue;
- source attribution reminder;
- edit risk;
- proposed show-note item.

These notes must never be mixed into spoken lines.

## 15. Output format

Use consistent labels:

SPEAKER A:
...

SPEAKER B:
...

Do not use:
- tables inside dialogue;
- markdown bullets as spoken content unless the speakers naturally enumerate;
- citations/URLs in speech;
- stage directions that NotebookLM would read as dialogue.

## 16. Final writing self-check

Before returning a draft, Claude must check:

1. Did both speakers contribute technical value?
2. Is every consequential claim inside the locked scope?
3. Did I invent any number, standard rule, real case or causal statement?
4. Did I preserve all applicability guards?
5. Did I distinguish source/guidance from Hardware-to-Production synthesis?
6. Did I execute the listener tool?
7. Did I duplicate a neighboring episode?
8. Are callbacks concise?
9. Does the episode end with one practical action?
10. Is the next-episode handoff correct?
11. Did I keep illustrative stories clearly illustrative?
12. Would a technically competent listener understand what to do differently?

If any answer is no, revise before output.
