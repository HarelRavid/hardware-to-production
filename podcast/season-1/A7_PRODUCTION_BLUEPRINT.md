# A7 Production Blueprint — Verification Planning Before DVT/PVT Thinking

status: PRODUCTION BLUEPRINT COMPLETE
season: Season 1 — Build the Right Thing

## Listener transformation
Before: “We need to run tests and see if the product passes.”
After: “I can define the claim, configuration, conditions, method, measurement and decision before the test begins, and I know what evidence will survive later review.”

## Narrative hook
A team spends weeks on environmental tests. Months later a design review asks: which hardware revision was tested? Which firmware? Was the gasket final? What was the acceptance criterion before the data were seen? Nobody can answer cleanly, so expensive test activity produced weak reusable evidence.

## Teaching flow
### Segment 1 — Testing is activity; verification is evidence
Differentiate exploration/debug from evidence used for release, supplier/process qualification or customer/compliance claims.

### Segment 2 — The verification chain
`Requirement/risk/interface → verification question → article/configuration → conditions → method → measurement → criterion → result → applicability → decision → retest trigger`.

### Segment 3 — Verification starts early
Ask how important requirements will be demonstrated while architecture is still flexible. This exposes untestable requirements and inaccessible interfaces before late-stage redesign.

### Segment 4 — Representativeness is claim-specific
Reuse A4: a test article can be representative for one claim and weak for another. Explain geometry/material/process/configuration/environment dependencies.

### Segment 5 — Measurement adequacy
Introduce the principle only: a crisp PASS number is weak if the measurement method cannot resolve the decision. Detailed MSA comes later.

### Segment 6 — Acceptance before results
Where a true pass/fail decision is intended, define criterion and decision logic before seeing the data. Exploratory tests may intentionally use learning outcomes instead.

### Segment 7 — Change and re-verification
A change does not require retesting everything. Identify which evidence depends on the changed attribute.

### Segment 8 — Sentinel Node environmental example
Compare exploratory printed-enclosure exposure with later production-intent enclosure/connector verification. Show what the early test taught and why it cannot silently become final qualification evidence.

### Segment 9 — DEV→LVP→SVP horizon
DEV: rapid, instrumented learning.
LVP: controlled articles/procedures/results and traceability.
SVP: release/qualification evidence tied to released configuration/process and controlled changes.

## Listener tools
### Verification Intent Sheet
`Claim → decision → article → configuration → representativeness → conditions → method → measurement → criterion/learning objective → result location → applicability → retest trigger`.

### Evidence-to-Claim Review
Ask whether the conclusion exceeds the actual test configuration, conditions or method.

## Misconceptions to challenge
- “More testing means more confidence.”
- “DVT/PVT is when verification starts.”
- “A pass proves the whole product.”
- “Every change means full retest.”
- “Exploratory data are useless for later engineering.”
- “The acceptance limit can be chosen after seeing results.”

## Standards/source backlog
NASA verification guidance; ISO/IEC/IEEE 29148 when exact requirements-verification language is used; product-specific qualification standards only with scope/edition verification.

## Closing handoff
A7 creates meaningful evidence. A8 ensures the evidence remains usable by answering: **which exact product, firmware, material, supplier and rework state did that result actually belong to?**
