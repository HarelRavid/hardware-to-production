# EP52 Script Outline V1 — Manufacturing Data Engineers Can Actually Use

status: SCRIPT OUTLINE COMPLETE
season: Season 5 — Automation, Data and the Connected Factory
audience: manufacturing / data / automation / OT security / engineering leadership
lifecycle: LVP → SVP → FIELD
source_lock: Wave 05
technical_review: evidence/source-lock/wave-05/W5_INTERNAL_TECHNICAL_REVIEW.md

## Listener promise
Define a decision-grade manufacturing dataset and a secure data path that preserve production context, authority, provenance and recoverability.

## Cold open
[ILLUSTRATIVE] Data lake has millions of samples, but failed units cannot be compared because recipe, calibration and rework context are missing. An analytics connector then gains broad OT access.

## Beat 1 — Start from engineering decision, not tags
Claims EP52-C01/C02.

## Beat 2 — Minimum context
product/config → unit/lot → operation → equipment/fixture → recipe/software → value+unit+time → measurement context → quality/rework/disposition → material/supplier → maintenance/change → provenance.

## Beat 3 — Derived/AI outputs need lineage
Claim EP52-C09.

## Beat 4 — OT changes the consequence model
Claim EP52-C03.
Source NIST SP 800-82 Rev3.

## Beat 5 — Read-only vs write-back
Claim EP52-C04.
Guard: read-only is lower authority, not automatically safe.

## Beat 6 — IEC 62443 responsibility map
Claim EP52-C05.
asset owner 2-1; service provider 2-4; system risk 3-2; system requirements 3-3; product lifecycle 4-1; component 4-2.
Guard: roles can coexist.

## Beat 7 — zones/conduits
Claim EP52-C06.
Risk architecture, not universal network drawing.

## Beat 8 — secure data path
asset → trust boundary → direction → identity/access → segmentation → monitoring → change → backup → recovery → evidence impact.

## Beat 9 — recovery after cyber/config event
Claim EP52-C08.
Restart is not enough if configuration/WIP/genealogy/quality/release trust changed.

## Listener tools
Engineering Data Fitness Check + Secure Data Path Review.

## Misconceptions
- more data = better evidence;
- read-only connector = safe by definition;
- RBAC alone solves OT security;
- 62443 mandates one network topology;
- machine restart = recovery;
- AI feature table can replace raw evidence lineage.

## Publication recheck
IEC 62443-2-1:2024 status must be rechecked before final release due IEC stability date 2026.

## Closing action
Pick one analytics or cloud data path and draw what can flow in each direction, which production decisions depend on it, and what happens if it is wrong/unavailable/compromised.

## Season close
Season 5 ends with connected manufacturing whose data remains tied to physical production truth and whose connectivity does not silently weaken safety, availability or evidence integrity.
