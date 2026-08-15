# A6 Research Pack — Serious Electronics/Embedded Prototype: From Dev Board to Controlled Hardware

status: CLAIM SET STABLE
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

## Stable core claim set
A6-C01 — Electronics prototype maturity is multidimensional: function, electrical margins, interfaces, firmware/configuration, components, assembly, testability and environment mature at different rates.

A6-C02 — Dev boards and lab instruments can accelerate learning while hiding dependencies in power, timing/noise, thermal behavior, EMC, programming and production test.

A6-C03 — Hardware revision, BOM revision, firmware version, configuration/calibration identity and test evidence must become traceably linked before repeated builds create ambiguity.

A6-C04 — Component selection must evolve from “works electrically” toward availability/lifecycle, package/assembly compatibility, alternate strategy and evidence-based substitution.

A6-C05 — Design-for-test and programming strategy should begin before LVP because normal production verification cannot depend indefinitely on engineering-only debug access.

A6-C06 — A passing bench test supports only the demonstrated configuration/test envelope; it does not automatically prove environmental, reliability, EMC, safety or serial-production performance.

A6-C07 — Bodge wires, jumpers, manual calibration, firmware workarounds and bench-only dependencies should remain visible development debt with owners and expiration conditions.

A6-C08 — The next electronics build should retire the most consequential uncertainty rather than merely produce a cleaner PCB.

## Audience contract
### DEV takeaway
Create a minimal controlled build identity: hardware revision + BOM + firmware + configuration + test result.

### Prototype shortcuts
Dev kits, breadboards, jumper wires, external power supplies, manual flashing, bench calibration, debug consoles and engineering test scripts are legitimate DEV shortcuts.

### Shortcut expiration
They expire when decisions depend on product power architecture, timing/noise, EMC, thermal behavior, production programming/test, field update, component availability, assembly repeatability or released configuration.

### LVP change
At tens/hundreds of units, the team needs controlled BOM/AVL intent, repeatable programming, production-test boundaries, traceability, configuration/calibration handling, defect/rework history and a disciplined substitute/change process.

### SVP evidence
Serial production requires evidence tied to released hardware/firmware/configuration and controlled manufacturing/test processes, plus applicable product qualification/compliance evidence.

### Manufacturing-debt prevention
Make bench-only dependencies and engineering interventions visible before they become undocumented factory instructions.

### Listener action
Run an Electronics Prototype Debt Scan on the current prototype.

## Listener Tool 1 — Electronics Prototype Debt Scan
Check:
- dev-board/lab-instrument dependency;
- bodge/jumper/manual wiring;
- untracked firmware or calibration/configuration;
- manual flashing/debug dependency;
- unavailable/single-source component or unqualified alternate;
- thermal/power/reset/timing/noise margin unknown;
- production-test access undefined;
- serial identity/traceability undefined;
- rework not recorded;
- compliance/reliability assumed from component evidence.

For each: `Accept now? → Owner → Expiration trigger → Next evidence`.

## Listener Tool 2 — Controlled Build Identity
Minimum serious repeated-build record:
`Unit ID → PCB/HW revision → BOM revision → firmware/software version → configuration/calibration version → programming method → test procedure/version → result → deviations/rework`

This can begin in a spreadsheet; enterprise tooling is not a prerequisite.

## Worked example — Sentinel Node controller
Illustrative only.

DEV article uses a commercial MCU board, USB/debug power, breakout sensor, manually flashed firmware and laptop script with no persistent unit identity.

It may support algorithm feasibility, sensor communication and basic user-flow learning.

It does not automatically support final power integrity, PCB EMC, enclosure thermal margin, production programming/test time, field configuration control, component/substitute qualification or serial assembly yield/rework claims.

Serious next build: introduce controlled custom hardware only where required to retire these risks and bind resulting evidence to HW/BOM/FW/configuration identity.

## Evidence/standards boundary
Possible later source families, depending on script claims:
- IPC-A-610 / J-STD-001 for assembly/acceptability context;
- IPC-2221 / IPC-6012 for PCB design/performance context;
- IPC/WHMA-A-620 for harnesses;
- J-STD-033 for moisture-sensitive device handling;
- JEDEC test methods for component/package reliability examples;
- product-specific IEC/EN/UL EMC/electrical-safety standards only after scope/jurisdiction is defined.

Guardrails:
- IPC acceptance is not product reliability proof.
- Component certification/qualification is not automatically system compliance.
- No IPC/JEDEC class, threshold or requirement enters the final script without edition/applicability verification.

## Claim classes / P0 state
- C01/C02/C03/C07/C08: V6 synthesis with P2.02/P2.03/P2.06 support.
- C04/C05: V6/V2; authoritative electronics/manufacturing support desirable; P1.
- C06: V6 evidence-envelope principle; any named compliance requirement becomes V1/P0.
- Open P0 for current conceptual core: 0.

## Common failure modes
- tested firmware/build cannot be reconstructed;
- BOM substitute treated as electrically equivalent without impact assessment;
- dev-board regulator/debugger hides final power behavior;
- production depends on engineer-only debug tools;
- calibration stored on someone's laptop;
- test fixture arrives after access points are frozen;
- component datasheet qualification mistaken for assembled-product qualification;
- reworked unit passes final test and failed history disappears.

## Navigation
Prerequisite recap: A3 interface ownership + A4 shortcut expiration in 60–90 seconds.
Can stand alone: yes, especially for electronics teams.
Recommended next: A7 verification planning, A8 configuration management, Episode 1 industrialization transition.

## Claim-set-stable result
PASS.
- Eight non-overlapping claims retained.
- Lightweight DEV implementation path preserved.
- Configuration/evidence identity explicitly links to frozen backbone rather than introducing a new model.
- Reliability/compliance boundary is explicit.
- Electronics standards remain in the Source Verification gate.

Next maturity target: EVIDENCE VERIFIED after P1 source support and any selected IPC/JEDEC/IEC claims are verified.
