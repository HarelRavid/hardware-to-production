# A1 Claude Launch & Return Packet

status: READY FOR EXTERNAL CLAUDE EXECUTION
asset: A1 — From an Idea to Engineering Requirements
production_board: podcast/FULL_SERIES_DIALOGUE_PRODUCTION_BOARD.md

## 1. Send to Claude

Use exactly this prompt as the execution entry point:

podcast/season-1/claude-handoff/A1/A1_CLAUDE_WRITING_PROMPT.md

The prompt itself links the Handoff Manifest and every MUST READ source.

Do not prepend a new technical summary.
Do not paste older scripts as higher-priority authority.
Do not ask Claude to research beyond the package.

## 2. Expected Claude return

Claude should return:

1. complete two-character dialogue;
2. labels only:
   - OZ:
   - RONA:
3. optional:
   - PRODUCTION NOTES — NOT SPOKEN
4. optional:
   - REVIEW FLAG — NOT FOR AUDIO

Claude must not return:
- invented citations;
- URLs inside dialogue;
- new standards rules;
- unverified numbers;
- renamed canonical frameworks.

## 3. Save returned draft

Target path after receiving Claude output:

podcast/season-1/dialogue-production/A1/A1_CLAUDE_DIALOGUE_DRAFT_V1.md

Initial status:

CLAUDE DRAFT RECEIVED — TECHNICAL REVIEW NEXT

## 4. Immediate review sequence after return

### D1 — Dialogue format
Check:
- Oz/Rona labels;
- both technically substantive;
- no naive-student Rona;
- no URLs/claim IDs in speech;
- production notes separated.

### D2 — Claim audit
Compare against:
- W1_A1_A7_A8_CLAIM_LOCK.md
- W1_SHARED_SOURCE_REGISTER.md
- W1_INTERNAL_TECHNICAL_REVIEW.md

Every consequential statement must map to the locked claim scope.

### D3 — Quantitative audit
A1 contains no evidence-derived engineering threshold.
Illustrative quantities must remain obviously illustrative.

### D4 — Editorial audit
Check:
- hook;
- Minimum Useful Requirements Sheet;
- Requirement Quality Check;
- Sentinel example;
- uncertainty/TBD logic;
- no A7/A8 duplication;
- correct A2 handoff.

### D5 — Source-note finalization
Update A1_SOURCE_NOTES_V1.md only if the Claude dialogue materially changes which locked sources are actually spoken/attributed.

### D6 — Final dialogue freeze
Create:

podcast/season-1/dialogue-production/A1/A1_FINAL_DIALOGUE_V1.md

Status:
FINAL DIALOGUE FROZEN — NOTEBOOKLM PACKAGE NEXT

## 5. NotebookLM downstream

After final dialogue freeze, use:

podcast/GEMINI_NOTEBOOK_AUDIO_PRODUCTION_CONTRACT.md

Then create:
- A1_NOTEBOOKLM_SOURCE.md
- A1_NOTEBOOKLM_CUSTOM_PROMPT.md
- A1_AUDIO_QA.md after audio generation.

## 6. Current blocker

The only remaining dependency before A1 technical/editorial review is the external Claude dialogue output.

No additional research or architecture work is needed for A1 before sending it to Claude.
