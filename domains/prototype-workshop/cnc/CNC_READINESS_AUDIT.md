# 2.2 CNC & Subtractive Prototyping — Readiness Audit

provenance: [GNR, SYN]
status: Reviewed

## 1. Scope
Audit against `knowledge-os/DEFINITION_OF_DONE.md` to determine whether the CNC cluster can support podcast writing without substantial new foundational research.

## 2. Coverage assessment

### 2.1 Definition / terminology
- Status: Strong
- Milling, turning, 3/4/5-axis, CAM, workholding, tooling, tolerance and inspection concepts are mapped.

### 2.2 Purpose / problem solved
- Status: Strong
- CNC is positioned as a rapid functional prototyping route when bulk-material fidelity, precision interfaces or production-grade stock matter.

### 2.3 Lifecycle position
- Status: Strong
- Prototype through Pilot coverage exists, with links to production representativeness.

### 2.4 Inputs / outputs
- Status: Moderate-Strong
- Core inputs are defined across CAD/CAM, material, datum, tooling, workholding and inspection. Some individual objects still need explicit owner/input/output metadata.

### 2.5 Decision criteria / tradeoffs
- Status: Strong
- CNC vs AM, 3/4/5-axis, hole/thread strategy, tolerance allocation and in-house/outsource decision trees exist.

### 2.6 Limitations / failure conditions
- Status: Strong
- Tool access, deep features, thin walls, clamping distortion, machine dynamics, material difficulty, burrs and metrology limitations are captured.

### 2.7 Common mistakes
- Status: Moderate-Strong
- Major pitfalls are embedded in claims and decision content; consolidate into a listener-facing pitfalls page before podcast publication.

### 2.8 Standards / normative sources
- Status: Moderate
- ASME Y14.5 is linked for GD&T; metrology and machining standards require one additional standards-focused pass. CNC itself is not governed by a single design standard.

### 2.9 Academic / government evidence
- Status: Strong
- NIST high-speed machining, path verification, on-machine metrology and uncertainty evidence provide strong anchors.

### 2.10 Books / handbooks
- Status: Moderate
- MIT course material and Seco reference-book ecosystem identified. Dedicated textbook bibliography should be strengthened before public release.

### 2.11 Industrial guidance
- Status: Strong
- Protolabs, Xometry, Kennametal, Seco and plastic-machining guidance are represented and explicitly treated as contextual/vendor guidance.

### 2.12 Case studies
- Status: Moderate-Strong
- NIST rapid CNC, Instrument Maker Shop, closed-loop inspection and difficult-material examples captured.

### 2.13 Relationships
- Status: Strong for core nodes
- Axis/CAM/workholding/material/tolerance/inspection/economics are linked. Relationship density should continue to grow as Sheet Metal and DFM domains are added.

### 2.14 Contradictions / uncertainty
- Status: Moderate
- Context dependence is preserved, especially supplier limits and machining parameters. Explicit contradiction objects are not yet necessary for most CNC fundamentals.

### 2.15 Listener-facing tags
- Status: Gap
- Final stable listener tag set should be assigned after Prototype Workshop domains are complete so naming remains consistent across CNC, AM and Sheet Metal.

### 2.16 Foundational research still required?
- Status: Low-Moderate
- No major foundational gap blocks podcast planning for CNC. Remaining work is strengthening references, adding standards/books and consolidating examples rather than discovering the basic structure.

## 3. Readiness score
Qualitative coverage estimate: **~82%**.

This is not a statistical score. It is a coverage judgment against the Definition of Done.

## 4. Current disposition
**Status: Reviewed / Near Podcast Ready**

Do not mark the entire CNC cluster `Podcast Ready` yet. Complete the following closing items first:
1. standards-focused pass for machining/metrology terminology and inspection;
2. curated books/handbooks bibliography;
3. listener-facing common-pitfalls summary;
4. final listener tags;
5. one cross-process case study comparing CNC, AM and Sheet Metal on the same prototype intent.

## 5. Decision
The cluster is mature enough to stop foundational expansion and proceed to the next Prototype Workshop cluster while keeping the five closing items in the CNC backlog.
