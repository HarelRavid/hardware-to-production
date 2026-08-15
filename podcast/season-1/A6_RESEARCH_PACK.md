# A6 Research Pack — Serious Electronics/Embedded Prototype: From Dev Board to Controlled Hardware

status: RESEARCH PACK OPEN
season: Season 1 — Build the Right Thing
primary_audience: A — founders/developers/early hardware teams
secondary_audience: electronics, embedded, test and NPI engineers
lifecycle: DEV → early LVP bridge
technical_depth: foundation/practitioner

## Episode promise
Show how to evolve an electronics/embedded prototype from a bench demonstration into controlled hardware that can support decisions about power, interfaces, components, firmware, testability, reliability, assembly and future production.

## Hook
The prototype works on a dev board with jumper wires and a laptop attached. The custom PCB arrives and suddenly the system resets under load, a component is unavailable, firmware depends on a debug cable, programming takes five minutes per unit, and nobody can reproduce which firmware/build actually passed the demo.

A working circuit is not yet a reproducible product configuration.

## Core claim set — draft
1. Electronics prototype maturity is multidimensional: functional behavior, electrical margins, interfaces, firmware/configuration, component lifecycle, assembly, testability and environment mature at different rates.
2. Dev boards and lab instruments are excellent learning tools but can hide power, timing, EMC, thermal, programming and production-test dependencies.
3. Hardware revision, BOM revision, firmware version, configuration/calibration data and test evidence must become traceably linked before repeated builds create ambiguity.
4. Component selection must evolve from “works electrically” toward availability, lifecycle, package/assembly compatibility, approved alternates and evidence for substitutions.
5. Design-for-test and programming strategy should begin before LVP because production cannot rely on engineering debug access as its normal verification method.
6. A passing bench test does not prove environmental, reliability, EMC, safety or serial-production performance outside the demonstrated test envelope.
7. Every bodge wire, jumper, manual calibration, firmware workaround and bench-only dependency should be treated as visible development debt with an owner/expiration condition.
8. The next electronics build should retire the most consequential uncertainty rather than merely produce a cleaner PCB.

Target final core claims: 6–8.

## Audience contract
### DEV takeaway
Create a minimal controlled build identity: hardware revision + BOM + firmware + configuration + test result.

### Prototype shortcuts
Dev kits, breadboards, jumper wires, external power supplies, manual flashing, bench calibration, debug consoles and engineering test scripts are legitimate DEV shortcuts.

### Shortcut expiration
They expire when decisions depend on product power architecture, timing/noise, EMC, thermal behavior, production programming/test, field update, component availability, assembly repeatability or released configuration.

### LVP change
At tens/hundreds of units, the team needs controlled BOM/AVL intent, repeatable programming, production test boundaries, traceability, configuration/calibration handling, defect/rework history and a disciplined substitute/change process.

### SVP evidence
Serial production requires evidence tied to released hardware/firmware/configuration and controlled manufacturing/test processes, plus applicable product qualification/compliance evidence.

### Manufacturing-debt prevention
Make bench-only dependencies and engineering interventions visible before they become undocumented factory instructions.

### Listener action
Run an Electronics Prototype Debt Scan on the current prototype.

## Listener Tool 1 — Electronics Prototype Debt Scan
Check each category:
- dev-board dependency;
- external lab supply/instrument dependency;
- bodge/jumper/manual wiring;
- untracked firmware build;
- untracked calibration/configuration;
- manual flashing/debug interface;
- unavailable/single-source component;
- unqualified alternate;
- thermal hot spot/margin unknown;
- power-up/brownout/reset behavior unknown;
- interface timing/noise margin unknown;
- production test access undefined;
- serial number/traceability undefined;
- rework not recorded;
- compliance/reliability evidence assumed from component datasheets.

For each item: `Accept now? → Owner → Expiration trigger → Next evidence`.

## Listener Tool 2 — Controlled Build Identity
Minimum record for a serious repeated build:
`Unit ID → PCB/HW revision → BOM revision → firmware/software version → configuration/calibration version → programmed by/method → test procedure/version → result → deviations/rework`

This can start in a spreadsheet; the principle matters before the software system.

## Worked example — Sentinel Node controller
Illustrative only.

DEV prototype:
- commercial MCU development board;
- USB-powered during debugging;
- sensor module on breakout board;
- manually flashed firmware;
- laptop script reads output;
- no persistent unit identity.

What it may prove: algorithm feasibility, sensor communication, basic user flow.

What it does not automatically prove:
- final power integrity/brownout behavior;
- PCB EMC behavior;
- thermal margins inside enclosure;
- production programming time;
- test coverage without debug console;
- field firmware/configuration control;
- component/substitute qualification;
- serial assembly yield/rework behavior.

Serious next build: introduce controlled custom hardware only where needed to retire these risks, and bind test evidence to HW/BOM/FW/configuration identity.

## Standards/evidence hooks
Later source verification may include, depending on actual episode claims:
- IPC-A-610 / J-STD-001 for assembly/acceptability context;
- IPC-2221 / IPC-6012 for PCB design/performance context;
- IPC/WHMA-A-620 where harnesses are material;
- J-STD-033 for moisture-sensitive device handling where applicable;
- JEDEC qualification/test methods for component/package reliability examples;
- product-specific IEC/EN/UL EMC/electrical-safety standards only with defined product scope/jurisdiction.

Guardrail: this episode must not imply IPC acceptance proves product reliability or that component certification proves system compliance.

## Initial claim classes
- Claims 1, 2, 3, 7, 8: V6 synthesis with P2.02/P2.03/P2.06 support.
- Claims 4, 5: V6/V2; authoritative electronics/manufacturing support desirable; P1.
- Claim 6: V6 general evidence-boundary principle; any named compliance requirement becomes V1/P0.

## P0 backlog
No exact normative requirement is needed for the conceptual episode core.
Any exact IPC/JEDEC/IEC/UL requirement, acceptance class, numeric criterion or compliance statement is P0 before final script.

## Common failure modes to teach
- firmware that passed test cannot be reconstructed;
- BOM substitute treated as electrically equivalent without impact assessment;
- dev-board regulator/debugger hides final power behavior;
- production depends on engineer-only debug tools;
- calibration stored on someone's laptop;
- test fixture created after design freezes access points;
- component datasheet qualification mistaken for assembled-product qualification;
- reworked unit passes final test and its failed history disappears.

## Navigation
Prerequisite recap: A3 interface ownership + A4 shortcut expiration, 60–90 seconds.
Can stand alone: yes, especially for electronics teams.
Recommended next: A7 verification planning, A8 configuration management, Episode 1 industrialization transition.

## Claim-set-stable exit criteria
- reduce to 6–8 non-overlapping core claims;
- verify terminology for BOM/AVL/programming/test/configuration without making industry-specific mandates;
- make electronics reliability/compliance boundaries explicit;
- map future IPC/JEDEC standards work into Source Verification Backlog;
- preserve a lightweight DEV implementation path rather than enterprise-tool assumptions.
