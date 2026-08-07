# CNC vs Polymer AM — Prototype Decision Matrix

Provenance: GNR + NIST/standards/industrial evidence.

| Decision criterion | CNC machining | Polymer AM |
|---|---|---|
| Stock-material fidelity | Strong | Variable; process/material-specific |
| Isotropic-like stock behavior | Generally strong | Often limited, especially FFF |
| Complex internal geometry | Limited by tool access | Strong for many AM processes |
| Fast one-off geometry iteration | Moderate | Often strong |
| Tight functional bores/fits | Strong | Often needs secondary finishing/validation |
| Surface finish | Strong and controllable | Process-specific; may require post-processing |
| Large flat metal parts | Strong if stock/fixture allow | Not applicable to polymer AM |
| Thin complex polymer geometry | Possible but workholding-sensitive | Often favorable depending on process |
| Enclosed channels | Usually difficult/impossible without split parts | Can be feasible, but powder/resin removal constraints apply |
| Early form/fit | Often overkill | Frequently favorable |
| Functional load testing in production-like stock material | Strong | Must verify printed-material representativeness |
| Production-process representativeness for molded parts | Low | Low to moderate; geometry may be representative but process-induced behavior is not |
| Fixture/jig iteration | Strong but slower | Often strong for fast iteration |
| Cost at quantity 1 | Setup-sensitive | Often favorable for small parts |
| Cost sensitivity to complexity | High where extra setups/tool access required | Often less sensitive to geometric complexity |

## Decision rules
1. If material fidelity and controlled interfaces dominate, CNC is often the better prototype route.
2. If iteration speed and geometric complexity dominate, polymer AM is often the better first route.
3. Hybrid workflows are common: print the body, machine critical bores/faces; or CNC the functional core and print covers/fixtures.
4. Neither route proves injection-molding process capability, molded warpage, weld lines, sink or production variation.
5. The prototype objective controls the decision.

## Relationships
- USES: H2P-PW-173 Prototype Manufacturing Process Selection
- USES: H2P-PW-174 Prototype Production Representativeness
- COMPARES: H2P-PW-049 CNC Milling
- COMPARES: H2P-PW-021 FDM/FFF
- COMPARES: H2P-PW-022 SLA
- COMPARES: H2P-PW-024 SLS
- COMPARES: H2P-PW-025 MJF
