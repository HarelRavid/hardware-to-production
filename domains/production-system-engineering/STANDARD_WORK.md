# 4.5 Standard Work

status: Researching
provenance: [GNR]

## Scope
Definition and maintenance of the best current repeatable production method for a specific product/process context, including sequence, timing, work content, WIP and abnormal-condition handling.

## Core objects
- takt time
- cycle time
- operator work content
- machine automatic time
- walking/motion
- work sequence
- standard WIP
- handoff
- waiting
- changeover boundary
- workstation layout
- standard condition
- abnormal condition

## Engineering principle
Standard Work is not merely documentation of current behavior. It is the controlled baseline from which deviation, improvement and capacity assumptions can be recognized and measured.

## Questions
1. Is cycle time measured under a stable standard condition?
2. Which work is value-adding, necessary non-value-adding or avoidable?
3. What is the minimum safe/robust standard WIP?
4. Which steps can overlap with machine automatic time?
5. Does the standard work preserve required inspection and traceability?
6. Are ergonomic and fatigue effects included in repeatability?
7. Does the method still work across expected product mix/variants?

## Decision objects
### D-PSE-SW-001 — Define standard sequence
### D-PSE-WIP-001 — Standard WIP strategy
### D-PSE-CT-001 — Valid cycle-time basis
### D-PSE-BAL-001 — Work allocation/operator balance boundary

## Improvement loop
Observe -> measure -> identify waste/variation -> trial improvement -> validate quality/safety/time -> update standard -> train -> monitor.

## Cross-links
Standard Work <-> takt/line balance
Standard Work <-> WI
Standard Work <-> ergonomics
Standard Work <-> training
Standard Work <-> OEE/capacity
Standard Work <-> PFMEA/control plan

## Integrity rule
Best observed cycle time is not automatically sustainable standard cycle time.