# Source-Lock Wave 02 — Quality Chain + Supplier Approval Evidence

status: COMPLETE — PUBLICATION WORKFLOW PASS FOR CURRENT GENERIC SCRIPT SCOPE
opened: 2026-09-19
closed: 2026-09-19
scope_type: shared-source-family wave
baseline_head_at_open: 14e0c1ca96fc67e18c6d5691389c1bee326747d2

## 1. Purpose

Scale the validated Wave 01 publication workflow to the quality/supplier evidence family while preserving a stricter boundary around protected industry manuals and customer-specific requirements.

Pipeline:
`Shared Source Lock → Episode Claim Lock → Internal Technical Review → Script Outline → Full Draft → Script Review → Source Notes → Publication Gate`.

## 2. Direct episode scope

- EP23 — DFMEA, PFMEA, Control Plans and Quality Gates
- EP24 — Production Testing and Measurement-System Capability
- EP32 — Process Capability, SPC and Knowing Whether Production Is Stable
- EP39 — Building the RFQ Technical Package and Approving First Production
- EP40 — Supplier Quality, Dual Sourcing and Resilience

Backbone:
- P2.03 — Quality Chain
- P2.06 — Supplier Industrialization / Approval / Change / Requalification

## 3. Canonical shared register

`evidence/source-lock/SOURCE_LOCK_WAVE_02_QUALITY_SUPPLIER_REGISTER.md`

## 4. Source strategy

Open/public authoritative sources carry generic engineering claims:
- NIST measurement-process characterization;
- NIST repeatability/reproducibility terminology;
- NIST process-capability guidance;
- NIST MEP supply-chain management;
- IAQG public 9102 scope/current Rev C resources;
- AIAG public catalog/overview pages for publication identity, high-level purpose and current-edition status.

Protected manuals remain method-detail gates:
- AIAG & VDA FMEA;
- AIAG Control Plan;
- AIAG MSA;
- AIAG & VDA SPC;
- AIAG PPAP;
- customer-specific requirements.

No protected manual content is reproduced in this repository.

## 5. Current edition/status controls checked 2026-09-19

AIAG:
- APQP: 3rd Edition, published Mar 2024.
- Control Plan: 1st Edition, published Mar 2024.
- MSA: Version 4/current catalog listing.
- PPAP: 4th Edition, 2nd Printing/current catalog listing.
- AIAG & VDA SPC: 1st Edition, released Jul 2026; supersedes the legacy AIAG-only SPC reference as the current AIAG/VDA harmonized publication.

IAQG:
- 9102 Rev C is the current public FAI resource/form family.

## 6. Quantitative control

Sentinel capability example independently recalculated:
- LSL 4.80, USL 5.20, sigma 0.04, mean 5.00:
  - Cp = 1.6667
  - Cpk = 1.6667
- same limits/sigma, mean 5.10:
  - Cp = 1.6667
  - Cpk = 0.8333

These are illustrative pedagogical numbers.
They are not field measurements and do not establish a universal acceptance threshold.

## 7. Wave-wide guardrails

1. Do not say an AIAG manual requires an exact step/field/threshold unless licensed/current text is reviewed.
2. Do not use a universal GR&R percentage or Cpk threshold.
3. Do not treat stability, capability and conformance as synonyms.
4. Do not treat FAI, PPAP-style approval and sustained process capability as synonyms.
5. Do not treat a supplier name as a permanent evidence object independent of process/site/configuration/change.
6. Do not convert NIST MEP supplier-management guidance into mandatory contractual supplier controls.
7. Customer-specific requirements remain customer-specific.
8. Automotive/aerospace methods may be compared by evidence question, not generalized as universal law.

## 8. Wave completion criterion

Wave 02 closes when all five episodes have:
- claim lock;
- internal technical review;
- source-safe script outline;
- full draft;
- script review;
- source notes;
- explicit remaining licensed/manual/customer-specific gates;
- publication gate record.

PODCAST READY remains a separate final gate.
