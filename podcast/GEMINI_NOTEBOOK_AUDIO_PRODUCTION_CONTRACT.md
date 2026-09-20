# Google NotebookLM Audio Production Contract

status: CANONICAL — DOWNSTREAM AUDIO PRODUCTION CONTROL
version: 1.0
created: 2026-09-20
platform: Google NotebookLM / notebook.google.com
governed_by:
- podcast/OFFICIAL_PODCAST_DELIVERY_ROADMAP.md
- podcast/CLAUDE_EPISODE_HANDOFF_CONTRACT.md
- podcast/TWO_CHARACTER_DIALOGUE_STYLE_CONTRACT.md
- podcast/FULL_SERIES_DIALOGUE_PRODUCTION_BOARD.md

## 1. Purpose

Define how a technically reviewed and editorially frozen Hardware-to-Production episode is converted into a Google NotebookLM Audio Overview production package.

This contract exists because NotebookLM Audio Overview is a generative podcast-style synthesis layer over notebook sources.

It is not treated as a deterministic text-to-speech engine that is guaranteed to read a supplied dialogue line-by-line.

Therefore:
- Claude creates the canonical editorial dialogue;
- the project audits and freezes that dialogue;
- a dedicated NotebookLM source package is created from the frozen content;
- NotebookLM generates the audio discussion;
- the generated audio receives content and technical QA before publication.

## 2. Canonical recurring hosts

The podcast has two recurring named engineering hosts.

### OZ — Veteran Engineer / Systems Engineer
Oz is the experienced engineering voice:
- practical;
- technically rigorous;
- calm;
- experienced with product development, manufacturing, suppliers, testing, production and scale.

### RONA — Young Engineer / Practitioner / Challenger
Rona is a younger engineer:
- technically capable;
- sharp;
- curious;
- confident;
- willing to challenge assumptions, cost, process overhead and overgeneralization.

Rona is not a student and must never be portrayed as naive.

### Legacy aliases
Historical source files may use:
- Speaker A / Character A = Oz
- Speaker B / Character B = Rona

These aliases are not output names.

## 3. Production architecture

Canonical downstream sequence:

CLAUDE HANDOFF READY
→ CLAUDE CANONICAL DIALOGUE DRAFT
→ CLAIM / TECHNICAL AUDIT
→ QUANTITATIVE / CASE / LEGAL AUDIT where applicable
→ TWO-CHARACTER EDITORIAL REVIEW
→ SOURCE-CURRENTNESS RECHECK
→ FINAL DIALOGUE FREEZE
→ NOTEBOOKLM SOURCE PACKAGE
→ NOTEBOOKLM CUSTOM AUDIO PROMPT
→ AUDIO OVERVIEW GENERATION
→ AUDIO QA
→ CORRECTION / REGENERATION if required
→ PODCAST READY

NotebookLM never bypasses claim/source/editorial gates.

## 4. Required per-episode production artifacts

After final dialogue freeze, create:

1. `<ASSET>_FINAL_DIALOGUE.md`
2. `<ASSET>_NOTEBOOKLM_SOURCE.md`
3. `<ASSET>_NOTEBOOKLM_CUSTOM_PROMPT.md`

Optional:
4. `<ASSET>_AUDIO_QA.md`
5. final show notes / visuals / metadata.

### 4.1 FINAL_DIALOGUE
This is the canonical reviewed editorial dialogue.

It must:
- use `OZ:` and `RONA:`;
- preserve the approved technical narrative;
- preserve worked examples, applicability guards and listener action;
- remain the reference against which the generated audio is audited.

### 4.2 NOTEBOOKLM_SOURCE
This is the clean source document uploaded or added to Google NotebookLM.

It should contain the episode's approved content in a form optimized for grounded generative audio.

It is not required to preserve every line break or every turn from FINAL_DIALOGUE.

It must preserve:
- episode title and purpose;
- Oz and Rona character identities;
- canonical engineering narrative;
- required concepts;
- worked example;
- technical distinctions;
- source-vs-synthesis boundaries;
- important numbers and their assumptions;
- required caveats/applicability;
- practical action;
- next-episode conceptual handoff.

It must exclude material we do not want the Audio Overview to narrate as podcast content:
- repository URLs;
- file paths;
- citation syntax;
- internal claim IDs;
- editorial gate names;
- implementation instructions intended only for the production team;
- unresolved review flags;
- hidden/internal notes not meant for audio.

### 4.3 NOTEBOOKLM_CUSTOM_PROMPT
This is the customization instruction used when generating the Audio Overview.

It controls:
- audience;
- host identities;
- desired discussion style;
- what to emphasize;
- what not to invent;
- episode-specific must-cover points;
- tone/pacing;
- language;
- closing action and handoff.

The custom prompt does not replace the source package.

## 5. NotebookLM behavior assumption

Treat Audio Overview as generative synthesis.

Do not assume:
- that NotebookLM will read the supplied dialogue verbatim;
- that Markdown speaker labels guarantee exact voice assignment;
- that names or speaker identities will always remain perfectly stable;
- that the generated discussion will preserve every line of the canonical script;
- that production notes embedded in the source will remain non-spoken.

For this reason:
- speaker names in source/custom prompt are guidance;
- generated audio must be audited;
- role reversals, omissions, new factual claims or technical distortion require regeneration/correction.

## 6. Recommended source structure

A NotebookLM source should use clear plain Markdown structure.

Recommended order:

# Episode title

## Podcast identity
Hardware-to-Production podcast.

## Hosts
Oz — veteran engineer / systems engineer.
Rona — young engineer / practitioner / challenger.

## Episode question
One concise engineering decision/question.

## Listener transformation
Before → After.

## Canonical discussion arc
The required narrative in sequence.

## Worked example
Only approved facts/numbers.

## Important technical boundaries
Applicability, caveats, source-vs-synthesis distinctions and prohibited overclaims.

## Practical action
The listener's concrete action.

## Handoff to next episode
The exact conceptual bridge.

This structure is production guidance, not a claim that Google requires these exact Markdown headings.

## 7. Canonical Audio Overview custom prompt template

Use this as the common base and append episode-specific requirements.

---

Create a podcast-style Audio Overview based only on the selected episode source.

The Hardware-to-Production podcast has two recurring engineering hosts:

OZ — a veteran engineer / systems engineer. He is highly experienced, practical, technically rigorous, calm, and familiar with product development, manufacturing, suppliers, testing, production and scale.

RONA — a young engineer / practitioner / challenger. She is technically capable, sharp, curious and confident. She challenges assumptions, asks why a method is necessary, tests ideas against practical constraints, and asks the questions a strong engineer earlier in her career would genuinely ask. She is not a student and must never sound naive.

Preserve these identities consistently:
Oz = veteran engineer.
Rona = young engineer.

The conversation should feel like two engineers working through a real engineering problem together.

Use natural back-and-forth discussion rather than alternating lectures.

Preserve the technical meaning, narrative order, worked example, engineering distinctions and practical takeaway contained in the selected source.

Do not introduce technical facts, standards requirements, numerical thresholds, real-world cases, statistics or engineering recommendations that are not supported by the selected source.

Do not mention:
- source files;
- repository paths;
- citations;
- URLs;
- claim IDs;
- production instructions;
- internal editorial notes.

Do not describe the episode as a summary of a document.

Present it as the Hardware-to-Production podcast.

Use technical language appropriate for practicing engineers, founders, NPI engineers, production engineers and hardware product teams.

Keep external guidance distinct from the podcast's own frameworks.

Never present an internal Hardware-to-Production framework as an ISO, NASA, NIST or other external requirement unless the source explicitly establishes that attribution.

Use the worked example actively rather than merely listing its components.

Preserve uncertainty and applicability boundaries.

Never convert “guidance,” “could,” “may,” or “depends on context” into a universal requirement.

Finish with:
1. one concrete practical action for the listener; and
2. the defined conceptual handoff to the next episode, when one exists.

Do not add a generic AI closing that changes the intended ending.

---

## 8. Episode-specific custom prompt extension

Every episode-specific NotebookLM custom prompt must append:
- episode ID and title;
- target audience level;
- exact must-cover engineering decision;
- the primary listener tool;
- the approved worked example;
- must-preserve quantitative assumptions where applicable;
- prohibited overclaims;
- exact next-episode handoff;
- output language;
- any pronunciation guidance that matters.

Do not place source citations or repository URLs in the custom audio prompt unless needed for production setup outside the generated audio.

## 9. Audio QA gate

Generated audio must be checked against the FINAL_DIALOGUE and source package.

At minimum verify:

### Host identity
- Oz and Rona identities are not reversed.
- Rona is not reduced to a naive student.
- Oz does not monopolize the technical content.

### Technical content
- no consequential claim was invented;
- no approved technical distinction was lost;
- no guidance was upgraded into a requirement;
- no real case was invented;
- no quantitative assumption changed;
- no applicability boundary disappeared.

### Narrative
- episode question remains clear;
- worked example is used;
- listener tool is executed;
- practical action survives;
- next-episode handoff is correct.

### Audio
- pronunciation is acceptable;
- acronyms are understandable;
- no obvious speaker-switch or third-voice artifact materially damages the episode;
- no source metadata or production note is spoken unexpectedly.

## 10. Regeneration rule

Regenerate or revise the source/custom prompt when:
- host identity is reversed or materially inconsistent;
- a critical concept is omitted;
- NotebookLM introduces an unsupported claim;
- a standard/guidance statement is strengthened;
- a numerical value or assumption changes;
- the audio states internal production notes;
- technical meaning is distorted.

A stylistic paraphrase alone is not a failure if technical meaning and the intended listener transformation remain intact.

## 11. Source-currentness rule

If a source-currentness gate is required for the episode, perform it before final NotebookLM package approval.

For current regulatory, standards or public-case content, a materially changed source can require:
- targeted source update;
- dialogue/source-package patch;
- regeneration.

## 12. Platform references

Implementation references checked 2026-09-20:

- Google describes NotebookLM Audio Overviews as podcast-style conversations generated from notebook sources.
- Google supports customization of Audio Overviews and allows users to specify focus, audience/learning goals and other guidance.
- Google supports multilingual Audio Overviews and provides an output-language setting.
- Audio Overviews are generative AI outputs and remain subject to generation variability.

Official Google references:
- https://blog.google/innovation-and-ai/products/developing-notebooklm/
- https://blog.google/innovation-and-ai/models-and-research/google-labs/notebooklm-video-overviews-studio-upgrades/
- https://blog.google/innovation-and-ai/models-and-research/google-labs/notebook-lm-audio-video-overviews-more-languages-longer-content/
- https://blog.google/innovation-and-ai/models-and-research/google-labs/notebooklm-audio-overviews-50-languages/

## 13. Final rule

Claude controls the canonical reviewed dialogue.

Google NotebookLM controls the generative audio realization.

The generated audio is accepted only after QA demonstrates that it preserves the approved engineering meaning, Oz/Rona character intent and episode narrative.
