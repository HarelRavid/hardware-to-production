# Hardware-to-Production Podcast — Official Season-by-Season Delivery Roadmap

status: CANONICAL — ACTIVE
version: 2.0
effective_date: 2026-09-19
supersedes: podcast/PODCAST_COMPLETION_WORKPLAN.md
program_goal: Complete the podcast in canonical publication order, Season 1 through Season 6, without losing planning depth, evidence quality, technical rigor, reviews, or execution controls.
canonical_endpoint_for_preparation: CLAUDE HANDOFF READY
downstream_generation: Claude writes the final two-character dialogue script; NotebookLM is the intended audio-generation/execution environment.

---

## 1. Executive decision

From this point forward, work proceeds strictly in canonical publication order:

Season 1 → Season 2 → Season 3 → Season 4 → Season 5 → Season 6.

A later season may already contain mature research, scripts or evidence packages. That work is preserved, but it does not change execution priority.

We finish each season from its current maturity state until every canonical asset in that season reaches:

**CLAUDE HANDOFF READY**

Only then do we move to the next season.

This replaces the previous strategy of continuing source-lock waves across the whole series before finishing earlier seasons.

### Immediate effect

- Wave 06 process-family work is PAUSED after 06C.
- 06A / EP11, 06B / EP12 and 06C / EP13 remain PASS and frozen as completed work.
- 06D–06I resume only when Season 2 becomes the active season.
- The current critical path becomes Season 1.

No completed artifact is discarded or rewritten merely to fit the new order.

---

## 2. Why this is the new canonical strategy

The podcast is not a repository-completion exercise.

The actual delivery objective is:

> produce a deeply researched, technically correct, source-controlled, two-character episode package that can be handed to Claude with all required context so Claude can write the final dialogue without inventing technical content or losing the intended episode depth.

The new season-by-season model protects five things simultaneously:

1. **Narrative continuity** — each season is finished as one listener journey.
2. **Technical depth** — no episode is rushed just because adjacent episodes are already mature.
3. **Evidence integrity** — source locks and applicability gates remain mandatory.
4. **Editorial consistency** — tools, terminology, callbacks and two-speaker roles are reviewed across the whole season.
5. **Production velocity** — once one season is handoff-ready, Claude script generation and NotebookLM production can begin while preparation continues on the next season.

---

## 3. Canonical maturity ladder from now on

The previous publication pipeline remains valid, but the preparation endpoint changes.

### Preparation lane

Production Architecture Complete  
→ Research / Evidence Pack Complete  
→ Source / Claim Lock  
→ Applicability Lock  
→ Quantitative / Case Verification  
→ Internal Technical Review  
→ Script Outline Complete  
→ Season Continuity Review  
→ Episode Handoff Manifest  
→ Claude Writing Prompt  
→ **CLAUDE HANDOFF READY**

### Downstream writing / production lane

Claude Handoff Ready  
→ Claude Two-Character Dialogue Draft  
→ Claude Script Technical Review  
→ Claude Script Editorial Review  
→ Source / Current-Status Recheck  
→ Final Dialogue Freeze  
→ NotebookLM Production Package  
→ NotebookLM Audio Generation / Execution  
→ Audio QA / Corrections  
→ Show Notes / Visuals / Metadata  
→ PODCAST READY  
→ Publish

The first lane is the canonical preparation work performed before moving to the next season.

The second lane may begin as soon as a season reaches Claude Handoff Ready.

---

## 4. Important change: no mandatory internal Full Script before Claude

For episodes that do not yet have a full internal script:

**do not create a new Hardware-to-Production Full Script Draft merely as an intermediate step.**

The new efficient path is:

Verified Evidence  
→ Technical Review  
→ Script Outline  
→ Claude Handoff Prompt  
→ Claude Dialogue Script

Reason:
Claude is the intended writer of the final spoken dialogue.

Our responsibility before Claude is to eliminate ambiguity about:
- what the episode must teach;
- what it must not claim;
- which evidence is authoritative;
- which numbers are verified;
- what is our synthesis;
- the exact narrative arc;
- the exact listener tools;
- the DEV/LVP/SVP translation;
- adjacent episode boundaries;
- the two-character interaction.

### Existing full scripts

Existing FULL_SCRIPT_DRAFT_V1 files are retained.

They are:
- valuable editorial/reference material;
- eligible as linked inputs to Claude;
- not automatically the canonical final spoken script;
- not discarded or rewritten unless a review identifies a problem.

This preserves all prior work while eliminating an unnecessary step for unfinished episodes.

---

## 5. Final writing model — two characters

Every final episode is written for two recurring speaker roles.

Names may be assigned later; roles are canonical now.

### Character A — Lead Host / Systems Engineer

Role:
- owns the episode structure;
- frames the engineering decision;
- introduces definitions only when needed;
- explains the canonical framework;
- keeps source/applicability boundaries accurate;
- connects the episode to the broader hardware lifecycle.

Voice:
- clear;
- experienced;
- practical;
- technically disciplined;
- never sounds like a standards document.

### Character B — Practitioner / Challenger

Role:
- asks the question the listener would ask;
- challenges overgeneralization;
- asks “what does this change in practice?”;
- tests the framework on examples;
- surfaces common mistakes and shortcuts;
- asks about cost, supplier reality, operator reality, scale and failure;
- summarizes the decision in practical language.

Voice:
- technically capable;
- skeptical but constructive;
- conversational;
- does not exist merely to say “yes” or repeat Character A.

### Dialogue rules

The Claude prompt must enforce:
- genuine back-and-forth, not alternating monologues;
- both characters carry technical content;
- no fake conflict for entertainment;
- no invented real-world anecdotes;
- illustrative scenarios explicitly remain illustrative;
- no character may introduce an unsourced consequential claim;
- questions should advance the listener journey;
- long technical explanation is broken by challenge/example/application;
- final script must remain natural for two-voice NotebookLM production.

---

## 6. Canonical episode preparation package

Every episode must reach Claude with one complete linked package.

### Required episode artifacts

1. Production Blueprint
2. Research Pack / relevant foundation/domain packs
3. Source Register
4. Claim Lock
5. Applicability / standards status notes
6. Quantitative check record where relevant
7. Case Evidence Pack where relevant
8. Internal Technical Review
9. Script Outline
10. Source Notes or source-note skeleton
11. Adjacent episode boundary / handoff notes
12. Season continuity notes
13. Episode Handoff Manifest
14. Claude Episode Writing Prompt

Existing full-script drafts may be item 15 as optional reference.

### Handoff Manifest purpose

The Handoff Manifest is the single navigation file for Claude.

It must answer:

- What is this episode?
- What must it teach?
- Who is the listener?
- What stage of the lifecycle does it serve?
- Which files are authoritative?
- Which files are background only?
- Which claims are forbidden or gated?
- Which numbers are factual vs illustrative?
- Which examples/cases are real vs fictional?
- Which canonical frameworks must be reused?
- What did previous episodes already teach?
- What must this episode hand to the next episode?
- What visual material should not be overexplained in audio?
- What style and two-character behavior are required?

Claude should not need to discover the repo structure independently.

---

## 7. Claude Episode Writing Prompt — mandatory structure

Each final prompt must be self-contained and link to all relevant repo artifacts.

### Section A — Task

Write the final spoken dialogue for:
- episode ID/title;
- season;
- two characters;
- intended approximate duration/word class;
- target technical depth.

### Section B — Listener transformation

Before → After.

### Section C — Mandatory source hierarchy

Provide direct repository links to:
- blueprint;
- claim lock;
- source register;
- technical review;
- worked examples;
- case packs;
- quantitative checks;
- source notes;
- relevant canonical framework documents.

The prompt must label:
- MUST READ;
- SUPPORTING;
- DO NOT TREAT AS AUTHORITY.

### Section D — Technical truth constraints

List:
- P0 claims;
- applicability boundaries;
- current standard versions/status;
- exact numbers;
- prohibited overclaims;
- cross-industry transfer limits;
- internal synthesis ownership.

### Section E — Narrative architecture

Provide:
- hook;
- teaching beats;
- worked example;
- listener tool execution;
- DEV/LVP/SVP translation;
- misconceptions;
- closing action;
- handoff to next episode.

### Section F — Two-character dialogue instructions

Specify Character A / Character B behavior and dialogue balance.

### Section G — Spoken-source rules

Claude must:
- attribute regulator/company/investigator claims naturally where needed;
- avoid reading citations/URLs aloud;
- avoid standards-title overload in spoken audio;
- move dense standard metadata to show notes unless decision-critical;
- never convert guidance into a requirement.

### Section H — Output format

Require:
- dialogue only, labeled consistently by speaker;
- optional production notes separated clearly from spoken text;
- no markdown tables inside spoken dialogue;
- no fabricated citations;
- no claims outside the source/claim set unless marked for review.

### Section I — Self-check before answer

Claude must verify:
- no unresolved P0 statement;
- no invented number;
- no duplicated episode owned elsewhere;
- no framework renaming;
- no real case presented without attribution;
- every example is correctly labeled;
- both speakers contribute meaningfully.

---

## 8. Season completion definition

A season is complete for preparation only when **every canonical asset in that season is Claude Handoff Ready**.

Season completion is not based on:
- number of research files;
- number of source links;
- existence of a blueprint;
- existence of an old script draft.

### Season exit gate

Before moving to the next season:

1. every episode package is complete;
2. every episode has a technical review;
3. every episode has a final Script Outline;
4. all P0 blockers for intended Claude narration are resolved or excluded;
5. season-wide duplicate-content review passes;
6. definitions/framework names are consistent;
7. callbacks and handoffs are mapped;
8. episode depth is balanced across the season;
9. no episode silently assumes content that has not yet been taught;
10. every episode has a Handoff Manifest;
11. every episode has a final Claude Writing Prompt;
12. season status is marked CLAUDE HANDOFF READY.

Only then does preparation move to the next season.

---

# 9. Season-by-season official roadmap

## SEASON 1 — Build the Right Hardware Before Production Finds Your Mistakes

Status: **CLAUDE HANDOFF READY — PASS (18/18)**

Exit audit:
`podcast/season-1/SEASON_1_CLAUDE_HANDOFF_EXIT_AUDIT.md`

Canonical scope:
A1–A8 + EP01–EP10
Total assets: 18

### Current mature publication packages

- A1 — complete package; one small wording patch previously noted
- A7 — complete package
- A8 — complete package

### Remaining preparation scope

A2–A6  
EP01–EP10

### Season 1 workstreams

#### S1-A — Foundation / roles / architecture / prototype evidence
Primary:
A2, A3, A4, A5, A6

Required work:
- verify current research/source packs;
- close source/claim locks;
- technical review;
- normalize Hardware Evolution Ladder references;
- preserve prototype pedigree/representativeness;
- build final outlines;
- generate Handoff Manifests + Claude prompts.

#### S1-B — NPI / readiness / DFX
Primary:
EP01–EP06

Required shared families:
- product vs manufacturing readiness;
- NPI ownership;
- lifecycle gates;
- DFM/DFA;
- prototype-to-production debt;
- process-selection handoff into Season 2.

#### S1-C — Test / tolerance / reliability / service
Primary:
EP07–EP10 plus A7/A8 callbacks

Required shared families:
- verification/testability;
- tolerance/variation;
- reliability/service;
- configuration identity.

### Season 1 season-wide review

Must confirm:
- A1–A8 feels like one opening arc;
- EP01 does not restart the series;
- readiness terms do not fork;
- A7/EP08 and A8/later change-control ownership remain distinct;
- DFX does not pre-teach Season 2 process families;
- listener reaches EP10 ready to choose manufacturing routes.

### Season 1 exit

18/18 assets:
CLAUDE HANDOFF READY.

Then and only then preparation moves to Season 2.

---

## SEASON 2 — How Hardware Is Actually Made

Status: **CLAUDE HANDOFF READY — PASS (9/9)**

Canonical scope:
EP11–EP19
Total assets: 9

### Current completed packages

- EP11 / Wave 06A — PASS
- EP12 / Wave 06B — PASS
- EP13 / Wave 06C — PASS

### Paused work to resume when Season 2 becomes active

- 06D EP14 Joining
- 06E EP15 Composites
- 06F EP16 Ceramics / Powder / Sintering
- 06G EP17 Additive
- 06H EP18 Surface / Cleaning / Heat Treatment
- 06I EP19 Process Chains

### Season 2 rule

Each process family keeps its own:
- material state;
- process physics;
- defect mechanisms;
- source family;
- standards/applicability;
- supplier capability;
- inspection;
- economics.

No generic numeric DFM folklore.

### Season 2 audio/editorial rule

Avoid encyclopedic process lectures.

Each episode should follow:

mechanism → failure/variation → design tradeoff → production evidence → decision.

Dense spatial/process material belongs in companion visuals/show notes.

### Season 2 exit

EP11–19:
CLAUDE HANDOFF READY.

Then move to Season 3.

---

## SEASON 3 — Build the Factory Before You Need the Factory

Status: **ACTIVE**

Canonical scope:
EP20–EP31
Total assets: 12

### Existing complete publication packages

EP23, EP24, EP26, EP27, EP28, EP29, EP30, EP31

### Remaining packages

EP20 — EBOM/MBOM/routing  
EP21 — tooling/fixtures/equipment  
EP22 — standard work/operator qualification  
EP25 — layout/material flow

### Season 3 completion wave

Create one shared source family:

**Production System Engineering**

Cover:
- MBOM/routing/execution definition;
- tooling/fixture intent and control;
- work instruction/operator qualification;
- layout/material flow/WIP/ergonomics;
- interfaces to quality/test/capacity already locked.

Then:
- complete missing episode packs;
- perform season continuity review;
- create 12 Handoff Manifests;
- create 12 Claude prompts.

### Season 3 exit

12/12:
CLAUDE HANDOFF READY.

---

## SEASON 4 — Quality, Suppliers and the Reality of Scale

Status: **ACTIVE**

Canonical scope:
EP32–EP40
Total assets: 9

### Existing complete packages

EP32, EP39, EP40

### Remaining

EP33–EP38

### Workstream 4A — Quality / reliability / traceability / compliance

EP33 — NCR / CAPA / effectiveness  
EP34 — reliability validation / field evidence  
EP35 — genealogy / affected-population reconstruction  
EP36 — standards / applicability / compliance

### Workstream 4B — sourcing / supplier industrialization

EP37 — make/buy / sourcing strategy  
EP38 — supplier capability / qualification

Then integrate existing EP39/40.

### Season-wide review

Check:
- CAPA does not duplicate field evidence;
- EP35 physical genealogy vs Season 5 digital genealogy distinction;
- compliance terminology remains jurisdiction/sector scoped;
- supplier industrialization arc EP37→40 is continuous.

### Season 4 exit

9/9:
CLAUDE HANDOFF READY.

---

## SEASON 5 — Automation, Data and the Connected Factory

Canonical scope:
EP41–EP52
Total assets: 12

### Current status

12/12 Publication Packages Complete.

No major source-pack construction remains.

### Required season preparation work

Because the new endpoint is Claude handoff rather than our own full script, existing full drafts become high-value reference inputs.

Required:
1. season-wide editorial/duplicate review;
2. confirm current-standard revision watches;
3. update EP52 IEC 62443-2-1 status before final prompt if needed;
4. normalize terminology across automation/data/security;
5. prepare Handoff Manifest for each EP41–52;
6. prepare Claude Writing Prompt for each EP41–52.

### Important Claude instruction

Existing script drafts are reference material only.

Claude must use:
claim/source lock + technical review + outline as authority.

### Season 5 exit

12/12:
CLAUDE HANDOFF READY.

---

## SEASON 6 — Manufacturing Atlas: Decision Playbooks and Case Studies

Canonical scope:
EP53–EP60
Total assets: 8

### Existing maturity

- EP53–59 dedicated Case Evidence Packs
- EP53–60 Production Blueprints
- Season 6 production/evidence reviews PASS
- strong FACT → SOURCE INTERPRETATION → OUR FRAMEWORK LESSON discipline

### Remaining work

Because Season 6 depends on public/current cases:
- recheck dates/populations/configurations;
- current regulator/investigation status;
- current standards/manual status;
- legal/settlement wording;
- company-reported vs independently established claims;
- current FDA/IATF/IAQG/OSHA/EU machinery applicability as actually used;
- technical domain review;
- final outlines;
- source notes;
- Handoff Manifests;
- Claude prompts.

### EP60 special rule

EP60 is synthesis.

Claude prompt must:
- use callbacks;
- not re-teach the entire series;
- preserve Sentinel Node as fictional worked example;
- replay decisions across lifecycle transitions.

### Season 6 exit

8/8:
CLAUDE HANDOFF READY.

At this point the full 68-asset preparation program is complete.

---

# 10. Claude script generation lane

Once a season is Claude Handoff Ready, Claude may generate its scripts while preparation moves to the next season.

But each generated script is not accepted automatically.

Required post-Claude gates:

1. dialogue-format compliance;
2. technical claim audit against Claim Lock;
3. quantitative audit;
4. source/applicability audit;
5. season continuity/edit audit;
6. duplicate-content audit;
7. two-character quality review;
8. word-count/duration review;
9. final source-currentness check;
10. final spoken-script freeze.

Any new consequential claim introduced by Claude goes back to source verification.

Claude is a writer, not a new evidence source.

---

# 11. NotebookLM production lane

NotebookLM is downstream of final dialogue approval.

Each approved episode should receive a NotebookLM Production Package containing:

- final two-character dialogue script;
- speaker-role definitions;
- pronunciation/acronym notes;
- episode summary;
- any non-spoken visual/show-note references;
- final source notes for factual grounding;
- forbidden paraphrase/overclaim notes where needed;
- target tone and pacing;
- episode title and sequence.

Audio output must then receive:
- content/omission check;
- pronunciation check;
- speaker-role consistency check;
- no fabricated claims check;
- technical meaning check;
- correction/rerender if needed.

NotebookLM output does not bypass editorial/technical QA.

---

# 12. Official current priority

CURRENT ACTIVE SEASON:

**Season 4 — Quality, Suppliers and the Reality of Scale**

COMPLETED PREPARATION:

- Season 1 — 18/18 CLAUDE HANDOFF READY
- Season 2 — 9/9 CLAUDE HANDOFF READY
- Season 3 — 12/12 CLAUDE HANDOFF READY

CURRENT PREPARATION GOAL:

EP32–EP40 → 9/9 CLAUDE HANDOFF READY.


---

# 13. Canonical progress metrics

Track four metrics separately:

### A. Production Architecture
68 / 68 complete.

### B. Publication Package Complete
Current baseline at roadmap activation: 29 / 68.

### C. Claude Handoff Ready
New primary preparation metric.

### D. Final Dialogue / NotebookLM Ready
Downstream production metric.

Do not use one blended percentage to hide where work actually remains.

---

# 14. Repository governance

This roadmap is now the canonical delivery roadmap.

Precedence for delivery planning:

1. podcast/OFFICIAL_PODCAST_DELIVERY_ROADMAP.md
2. podcast/EPISODE_PACKAGING_CONTRACT.md
3. podcast/SCRIPT_OUTLINE_CONTRACT.md
4. podcast/SOURCE_NOTES_CONTRACT.md
5. podcast/PODCAST_COMPLETION_WORKPLAN.md — historical/superseded
6. season-specific production/review documents

Knowledge Backbone / PODCAST_MAP still retain technical/content authority.

This roadmap controls **delivery order and completion gates**, not technical truth.

---

# 15. Final program rule

**One season at a time.**
**Publication order equals preparation order.**
**No loss of evidence depth or review rigor.**
**Claude receives a complete, linked, constrained writing package.**
**Claude writes the two-character dialogue.**
**NotebookLM performs the downstream audio-generation/execution step.**
