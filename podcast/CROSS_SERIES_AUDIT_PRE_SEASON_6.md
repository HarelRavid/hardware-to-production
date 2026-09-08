# Cross-Series Audit Before Season 6

status: COMPLETE — CONTINUE WITH CANONICAL HYGIENE REPAIRS
scope: Opening Arc A1–A8 + Episodes 1–52 + editorial/navigation architecture
purpose: Verify continuity, duplicate ownership, lifecycle logic, adherence to the original plan, and repository canonical clarity before producing Season 6.

## 1. Executive decision

The technical/editorial program remains coherent and aligned with the intended Hardware-to-Production journey.

Decision: **PASS WITH CANONICAL HYGIENE REPAIRS REQUIRED BEFORE SEASON 6 PRODUCTION.**

No redesign of Seasons 1–5 is required. The main technical arc is continuous and the recurring themes are mostly intentional reinforcement rather than duplicate episode ownership.

The principal issue is repository/editorial hygiene: several historical navigation/season documents and research-pack locations still describe superseded season structures. They can confuse future editors/agents even though the current production blueprints follow the correct canonical architecture.

## 2. Canonical precedence — effective immediately

Use this precedence for all future podcast work:

1. `PODCAST_MAP.md` — canonical episode IDs, titles and topic mappings.
2. `podcast/PODCAST_SEASON_ARCHITECTURE.md` — canonical current six-season listener architecture.
3. `podcast/EPISODE_PACKAGING_CONTRACT.md` — canonical episode packaging/evidence rules.
4. `MASTER_WBS.md` + frozen Knowledge Backbone/evidence packages — canonical technical knowledge ownership.
5. Current season production blueprints/full reviews.

Any older season/navigation artifact that conflicts with items 1–3 above is historical/superseded and must not drive new production decisions.

## 3. Current canonical six-season journey

### Season 1 — Build the Right Hardware Before Production Finds Your Mistakes
A1–A8 + EP01–10.
Journey: idea → requirements → architecture → controlled prototypes → production intent → DFX/test/variation/reliability.

### Season 2 — How Hardware Is Actually Made
EP11–19.
Journey: production intent → manufacturing-process and process-chain selection.

### Season 3 — Build the Factory Before You Need the Factory
EP20–31.
Journey: LVP → production system → pilot → validation → ramp/change.

### Season 4 — Quality, Suppliers and the Reality of Scale
EP32–40.
Journey: stable production → quality/evidence system → supplier industrialization/resilience.

### Season 5 — Automation, Data and the Connected Factory
EP41–52.
Journey: scalable production → automation → digital thread/data/OT context.

### Season 6 — Manufacturing Atlas: Decision Playbooks and Case Studies
EP53–60.
Journey: cross-domain application, case reconstruction and full decision synthesis.

This is fully consistent with the current `PODCAST_MAP.md` and `podcast/PODCAST_SEASON_ARCHITECTURE.md`.

## 4. End-to-end continuity audit

### Opening Arc → EP01–10
PASS.
The Opening Arc builds the early-team mental model; EP01–10 convert that foundation into manufacturability/industrialization decisions. The Season 1 V2 review correctly treats A1–A8 + EP01–10 as one listener journey.

### EP10 → EP11
PASS.
EP10 closes product-architecture/reliability/service design thinking. EP11 begins manufacturing-route selection. The transition is logical: define what the product must survive/become, then choose how it will actually be made.

### EP19 → EP20
PASS.
EP19 owns manufacturing process-chain design; EP20 owns translation of the released product definition into MBOM/routing/process execution. This is a clean product/process → production-system handoff.

### EP31 → EP32
PASS.
EP31 closes ramp change/effectivity; EP32 asks whether the resulting production process is statistically stable/capable. This is the correct ramp → sustained quality transition.

### EP40 → EP41
PASS.
EP40 closes supplier resilience; EP41 asks whether automation is justified in the now-scalable production system. Automation does not arrive before supplier/process maturity.

### EP46 → EP47
STRONG PASS.
The physical process is stabilized/scaled before the information architecture is layered over it. This avoids the common mistake of digitizing unstable manufacturing.

### EP52 → EP53
PASS, with one Season 6 requirement.
EP52 closes the engineering-grade data/connected-factory layer. EP53 should deliberately switch mode from teaching new architecture to applying the accumulated system through real cases. Season 6 must not reopen fundamentals as if they were new topics.

## 5. Duplicate-content audit — high-risk pairs

### EP10 vs EP34 — reliability
CONTROLLED, KEEP BOTH.
- EP10 owns design-for-reliability/service/repair and field-learning architecture before launch.
- EP34 owns reliability validation under real production variation, configuration, supplier and field exposure.

Script rule: EP34 should open by explicitly saying it assumes the design-for-reliability principles of EP10 and now asks whether production evidence supports the reliability claim.

### EP08 vs EP24 vs EP44 — test/measurement
CONTROLLED, KEEP ALL THREE.
- EP08 owns design-for-test/calibration/traceability as a product design concern.
- EP24 owns production test architecture plus measurement-system capability and trustworthy decisions.
- EP44 owns automation of inspection/EOL test and qualification of the automated decision path.

Script rule: always distinguish testability → measurement adequacy → automation of test.

### EP09 vs EP32 — variation/capability
CONTROLLED, KEEP BOTH.
- EP09 owns tolerances/GD&T/GPS and product/process variation as a design/release problem.
- EP32 owns time-ordered process stability, SPC and capability interpretation in sustained production.

Script rule: EP32 should not re-teach tolerance-stack fundamentals.

### EP31 vs EP35/EP48 — configuration/effectivity/genealogy
CONTROLLED, KEEP.
- EP31 owns engineering-change effectivity during ramp.
- EP35 owns traceability/genealogy as quality/affected-population evidence.
- EP48 owns the digital implementation of as-built/as-processed genealogy, recipes, parameters and measurements.

### EP35 vs EP48 — genealogy
CONTROLLED, KEEP BOTH.
EP35 owns the quality principle and investigation need; EP48 owns connected digital-thread implementation. No merge needed.

### EP36 vs EP49 — standards/evidence
CONTROLLED, KEEP BOTH.
EP36 owns applicability/compliance operations. EP49 owns graph representation of standards, claims, sources, evidence and provenance.

### EP29 vs EP42/EP45 — capacity/economics/OEE
CONTROLLED.
- EP29 owns physical capacity, takt, constraint and accepted throughput.
- EP42 owns investment economics for automation.
- EP45 owns automated-system losses/OEE/maintenance and sustained equipment performance.

OEE must remain a loss lens, not a substitute for EP29 system capacity analysis.

### EP37–40 vs Season 6 industry case episodes
RISK TO CONTROL DURING SEASON 6.
Season 6 must use supplier/quality/approval frameworks as lenses in cases, not re-teach supplier qualification, RFQ, CAPA or dual sourcing from scratch.

## 6. Repetition that is intentionally canonical

These themes repeat across many episodes and should continue to do so because they are global invariants:
- Claim → Evidence → Applicability;
- configuration identity and effectivity;
- DEV / LVP / SVP;
- product evidence ≠ manufacturing evidence;
- measurement adequacy before capability/quality conclusions;
- rework adds history rather than erasing failure;
- accepted sustainable throughput over isolated peak speed;
- approval valid only inside the demonstrated envelope;
- change invalidates only affected evidence dependencies;
- recovery requires restored configuration, quality, genealogy and release trust.

The repetition becomes a problem only if a later episode re-explains the full concept instead of applying it at a new decision layer.

## 7. Plan adherence audit

PASS.

The project still follows the intended product order:
Knowledge OS/Data Hub → podcast → toolkit/learning paths → Manufacturing Atlas/interactive decision support.

The podcast still uses the Knowledge OS as the source of truth rather than reshaping engineering truth to fit episode narratives.

The current editorial map remains 68 listener assets: Opening A1–A8 + core EP01–60. The current six-season packaging is a navigation layer over that unchanged technical roadmap.

Season progression is still logically aligned to the Hardware Evolution Ladder:
`Idea → requirements → prototype → production intent → process selection → production system → pilot/validation/ramp → stable quality/suppliers → automation/data → cross-domain synthesis`.

No season currently jumps forward and then requires a hidden technical prerequisite from a later season.

## 8. Repository/canonical hygiene findings

### Finding H1 — multiple historical navigation architectures
SEVERITY: HIGH FOR FUTURE EDITORIAL CONFUSION; LOW FOR CURRENT CONTENT.

Several files still declare old season/navigation structures, including variants where automation/digital factory is called Season 6. These conflict with the current six-season architecture where automation/data is Season 5 and case studies/synthesis is Season 6.

Required repair:
- keep `PODCAST_MAP.md` and `podcast/PODCAST_SEASON_ARCHITECTURE.md` as current canonical authorities;
- mark older navigation files explicitly SUPERSEDED/HISTORICAL or archive them;
- future agents must not infer season structure from legacy files.

### Finding H2 — Season 1 has two full reviews
SEVERITY: MEDIUM.

`SEASON_1_FULL_REVIEW.md` covers only A1–A8 under the old Season 1 framing.
`SEASON_1_FULL_REVIEW_V2.md` covers canonical A1–A8 + EP01–10 and is the correct current review.

Required repair:
- V2 is canonical;
- older review should be marked superseded/historical.

### Finding H3 — misplaced Season 2 research packs EP02–EP10
SEVERITY: MEDIUM.

The production blueprints are correctly in Season 1, but research packs EP02–EP10 remain under `podcast/season-2/` and contain old season labels such as “Turn the Prototype into a Product.”

Required repair:
- do not treat their folder/season metadata as canonical;
- migrate or archive these research packs before final source-pack/script production;
- preserve their research content rather than deleting it blindly.

### Finding H4 — pilot artifacts still use old season naming
SEVERITY: LOW–MEDIUM.

`podcast/pilot/` contains valuable historical research/source-verification artifacts with pre-freeze/old season labels.

Required repair:
- retain them as historical evidence/pilot material;
- explicitly mark the folder non-canonical for current season routing.

### Finding H5 — Season 6 case evidence is the remaining known content-depth dependency
SEVERITY: EXPECTED/CONTROLLED.

The evidence campaign already identifies case-study evidence for EP53–60 as a controlled gap. Season 6 therefore must be case-source driven and must not be produced as generic commentary without primary/official evidence where available.

## 9. Season 6 guardrails produced by this audit

1. EP53–59 are application/case episodes, not a seventh pass over foundational teaching.
2. Every case separates FACT / SOURCE INTERPRETATION / OUR FRAMEWORK LESSON.
3. Do not claim one industry's method is universally required.
4. Each case must explicitly show which earlier episode/framework is being applied.
5. EP54 successful-pattern claims need evidence and domain-transfer limits; avoid survivorship-bias storytelling.
6. EP55 startup shortcuts must use the existing prototype-shortcut + expiration logic rather than invent a new maturity model.
7. EP56 automotive: APQP/PPAP/FMEA/SPC/MSA are industry/customer-context methods, not universal laws.
8. EP57 medical: regulatory/QMS claims need exact jurisdiction/product applicability.
9. EP58 aerospace: FAI/special-process/configuration controls require exact applicability and must not be generalized.
10. EP59 industrial equipment should own long-life service/configuration/retrofit lessons without duplicating EP10 reliability/service design.
11. EP60 must explicitly replay the Hardware Evolution Ladder and show the same product treated differently in DEV, LVP and SVP.
12. EP60 should use the existing canonical frameworks; do not invent a new final mega-framework that competes with the Knowledge Backbone.

## 10. Overall conclusion

The content architecture is sound.

There is no reason to redesign, reorder or merge the current Seasons 1–5.

The most important pre-Season-6 action is editorial governance cleanup: make the current canonical documents unmistakable and quarantine legacy season-routing metadata. After that, Season 6 can proceed safely as an application/synthesis season.

Final audit status: **PASS — CONTINUE AFTER CANONICAL HYGIENE REPAIR.**
