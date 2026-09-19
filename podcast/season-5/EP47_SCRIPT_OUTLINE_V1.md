# EP47 Script Outline V1 — What PLM, ERP, MES, QMS, SCADA and Historians Actually Do

status: SCRIPT OUTLINE COMPLETE
season: Season 5 — Automation, Data and the Connected Factory
audience: manufacturing / systems / data / quality / engineering leadership
lifecycle: LVP → SVP
source_lock: evidence/source-lock/wave-05/W5_EP47_EP48_EP49_EP50_EP51_EP52_CLAIM_LOCK.md
technical_review: evidence/source-lock/wave-05/W5_INTERNAL_TECHNICAL_REVIEW.md
blueprint: podcast/season-5/EP47_PRODUCTION_BLUEPRINT.md

## Listener promise
Map manufacturing information objects to authoritative ownership and consuming systems without assuming one vendor category should own everything.

## Cold open
[ILLUSTRATIVE] PLM has one BOM, ERP another, recipes live in machines and quality disposition lives in email. Every system is locally correct; no one can reconstruct what actually built a serial.

## Beat 1 — Start from information objects, not software brands
Claim: EP47-C01.
Objects: product definition, material transaction, execution, quality event, machine state, maintenance state.

## Beat 2 — ISA-95 as integration reference
Claims: EP47-C02.
Source: W5-S01/S02.
Guard: reference model, not mandatory software stack or cyber tiers.

## Beat 3 — Practitioner system roles
Claim: EP47-C03.
PLM/PDM, ERP/MRP, MES/MOM, QMS, SCADA/HMI, historian.
Tag: [SYNTHESIS].
Guard: roles vary by implementation.

## Beat 4 — Authoritative owner vs copy/cache
Claim: EP47-C04.
A replica can be valid; ambiguity occurs when authority/effectivity is unclear.

## Beat 5 — Competing truth audit
Use product revision, routing, recipe, quality status, material lot, genealogy and machine configuration.

## Beat 6 — Minimal viable digital thread by maturity
Claim: EP47-C05.
DEV: lightweight tools with identity.
LVP: explicit SoR boundaries.
SVP: governed interfaces/access/recovery.

## Listener tool — System-of-Record Map
Information object → authoritative owner → consumers → identifier → revision/effectivity → interface → evidence → fallback/recovery.

## Misconceptions
- ERP is master of everything;
- MES is always required;
- ISA-95 defines my vendor stack;
- duplicated data is always wrong;
- integration fixes unclear ownership.

## Closing action
Choose seven critical information objects and name the authoritative source and conflict-resolution rule for each.

## Handoff
EP48 uses those boundaries to reconstruct the actual unit history.
