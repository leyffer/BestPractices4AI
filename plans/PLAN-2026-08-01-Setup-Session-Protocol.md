# PLAN 2026-08-01 — Set up CLAUDE.md and Session Protocol

## Context

`BestPractices4AI` is a MkDocs (Material theme) documentation site published to GitHub Pages. It had
no repo-scoped `CLAUDE.md` (the only `CLAUDE.md` in the tree belonged to an unrelated parent project,
`QuasiNewtonMixed`). Goal: add a `CLAUDE.md` that documents the project and establishes a lightweight
session logbook/status protocol so decisions and state persist across sessions.

## Changes

Created at the repo root:

1. **`CLAUDE.md`** — project overview, repository structure, common workflows (local preview, build,
   add-a-page, deploy), plus the file-structure and session-protocol sections.
2. **`LOGBOOK.md`** — header + first session entry (this change), linking to this plan.
3. **`STATUS.md`** — initial current-state snapshot.
4. **`plans/PLAN-2026-08-01-Setup-Session-Protocol.md`** — this file.

## Notes / Decisions

- The parent `../CLAUDE.md` (QuasiNewtonMixed) is unrelated and was not touched.
- Root bookkeeping files live outside `docs/`, so they do not affect the site build or nav.

## Verification

1. `ls` repo root: confirm `CLAUDE.md`, `LOGBOOK.md`, `STATUS.md`, `plans/` exist.
2. Confirm `LOGBOOK.md` links to this plan.
3. (Optional) `mkdocs build` still succeeds.
