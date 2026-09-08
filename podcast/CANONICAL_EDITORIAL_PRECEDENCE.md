# Canonical Podcast Editorial Precedence

status: CURRENT CANONICAL ROUTING CONTROL
purpose: Prevent historical/pilot season-navigation artifacts from overriding the current podcast map.

## Precedence

For any disagreement about episode IDs, titles, season placement, audience routing or production packaging, use this order:

1. `PODCAST_MAP.md` — canonical episode IDs, titles and WBS/topic mappings.
2. `podcast/PODCAST_SEASON_ARCHITECTURE.md` — canonical current six-season listener-facing architecture.
3. `podcast/EPISODE_PACKAGING_CONTRACT.md` — canonical production/evidence packaging rules.
4. `MASTER_WBS.md` and Knowledge Backbone V1 artifacts — canonical technical ownership/evidence architecture.
5. Current season production blueprints and current full-review documents.

## Current six seasons

1. Season 1 — Build the Right Hardware Before Production Finds Your Mistakes — A1–A8 + EP01–10.
2. Season 2 — How Hardware Is Actually Made — EP11–19.
3. Season 3 — Build the Factory Before You Need the Factory — EP20–31.
4. Season 4 — Quality, Suppliers and the Reality of Scale — EP32–40.
5. Season 5 — Automation, Data and the Connected Factory — EP41–52.
6. Season 6 — Manufacturing Atlas: Decision Playbooks and Case Studies — EP53–60.

## Historical/superseded navigation artifacts

Older navigation/season documents may remain in the repository for historical traceability. If any of them assign different season numbers/titles than the current list above, that routing is superseded and must not be used for new work.

Examples include older files named around:
- `PODCAST_SEASON_NAVIGATION_ARCHITECTURE*`
- `PODCAST_SEASONS_AND_NAVIGATION*`
- `SEASON_NAVIGATION_ARCHITECTURE*`

These historical artifacts may contain useful rationale, but they do not override the current canonical sources.

## Season 1 review precedence

Canonical full-series Season 1 review:
`podcast/season-1/SEASON_1_FULL_REVIEW_V2.md`

The older `SEASON_1_FULL_REVIEW.md` covers the earlier A1–A8-only framing and is historical.

## Legacy research-pack routing

Research packs can contain valid evidence even if their old `season:` metadata is obsolete. Folder/metadata location must therefore never override `PODCAST_MAP.md` or current season architecture.

In particular, historical EP02–EP10 research packs under `podcast/season-2/` belong editorially to canonical Season 1.

## Pilot folder

`podcast/pilot/` is a historical pilot/evidence workspace. Its artifacts may remain valid research inputs, but its season labels and routing are not current canonical editorial metadata.
