# A2 Final Script Outline — Hardware Team Map: Who Owns What?

status: FINAL SCRIPT OUTLINE COMPLETE — SEASON CONTINUITY PENDING
season: Season 1
audience: founders / early hardware teams / engineering leads
lifecycle: DEV-first / cross-stage
source_lock: evidence/source-lock/season-1/S1A_A2_CLAIM_LOCK.md
technical_review: evidence/source-lock/season-1/S1A_INTERNAL_TECHNICAL_REVIEW.md
blueprint: podcast/season-1/A2_PRODUCTION_BLUEPRINT.md
research: podcast/season-1/A2_RESEARCH_PACK.md

## Listener transformation
Before:
“We need a mechanical engineer, electronics engineer and maybe firmware.”

After:
“I can map consequential engineering responsibilities independently of job titles, see ownership gaps, and decide what can be combined, outsourced or requires specialist review.”

## Two-character opportunity
Speaker A frames responsibilities before titles.
Speaker B challenges:
“Are you telling a five-person startup to hire twelve specialists?”
The answer must distinguish responsibility coverage from headcount.

## Cold open
[ILLUSTRATIVE]
A small startup has strong engineers but repeatedly misses thermal limits, connector integration and testability because those responsibilities are nobody’s explicit job.

## Beat 1 — Multidisciplinary does not mean large team
Claims: A2-C01/A2-C04.
Sources: S1A-S01/S02/S03.
Guard:
NASA supports multidisciplinary/role visibility; our startup implementation is internal synthesis.

## Beat 2 — Responsibilities before job titles
Claim: A2-C02.
Tool:
Hardware Discipline Map.
Use practical responsibility families without declaring them mandatory job roles.

## Beat 3 — Where ownership gaps become expensive
Claim: A2-C03.
Bridge to interfaces, integration and verification.
Use one connector/thermal/test example.

## Beat 4 — One person can wear many hats
Claim: A2-C04.
Explain competence/review boundary.

## Beat 5 — Escalation triggers
Architecture lock-in, safety/compliance impact, irreversible NRE/tooling, supplier transfer, expensive qualification, release consequences.
Guard:
not universal legal triggers; engineering decision triggers.

## Beat 6 — Manufacturing/quality/test cannot wait until “design is done”
Claim: A2-C05.
Source: NIST early process-planning premise + Product Readiness backbone.

## Beat 7 — Outsourcing work vs outsourcing ownership
Claim: A2-C07.
Use contractor example.

## Beat 8 — DEV / LVP / SVP
Claim: A2-C08.
DEV: generalists + targeted expert review.
LVP: explicit NPI/test/quality/supplier ownership.
SVP: durable release/change/field authority.

## Listener tool execution
Run Hardware Discipline Map on Sentinel Node:
sensor performance / sealing / PCB power / firmware / calibration / supplier change / production test / system integration.

## Misconceptions to correct
- every discipline requires a separate employee;
- one strong generalist can absorb everything indefinitely;
- consultants own integration because they designed a subsystem;
- quality/manufacturing begin after prototype completion;
- “everyone owns integration” is sufficient ownership.

## Closing action
List the ten most consequential technical decisions in the current project and name one owner/reviewer for each.

## Handoff
A2 names the owners.
A3 defines where those owners must agree: interfaces.
