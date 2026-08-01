# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

**BestPractices4AI** is a [MkDocs](https://www.mkdocs.org/) documentation site using the
[Material](https://squidfunk.github.io/mkdocs-material/) theme: "A curated collection of best
practices, notes, and links for working with AI."

- Published to GitHub Pages: <https://leyffer.github.io/BestPractices4AI/>
- Repo: `leyffer/BestPractices4AI`
- Auto-deployed on push to `main` via `.github/workflows/deploy.yml` (runs `mkdocs gh-deploy --force`).

## Repository Structure

- `mkdocs.yml` — site config: theme, palette, plugins, and the `nav` tree.
- `requirements.txt` — `mkdocs-material`, `mkdocs-git-revision-date-localized-plugin`.
- `docs/` — all site content, organized to match the `nav` block in `mkdocs.yml`:
  - `index.md` — Home (includes Argonne-specific, login-required resources).
  - `prompt-eng/system-prompts.md`, `prompt-eng/few-shot-guides.md`
  - `development/agent-design.md`, `development/evaluation.md`
  - `security/data-privacy.md`
  - `resources/links.md`
- `.github/workflows/deploy.yml` — CI deploy to GitHub Pages.

## Common Workflows

- **Local preview:** `pip install -r requirements.txt` then `mkdocs serve` (view at
  <http://127.0.0.1:8000>).
- **Build:** `mkdocs build`.
- **Add a page:** create the `.md` under `docs/<section>/`, then add it to the `nav:` block in
  `mkdocs.yml`. The nav is manual — pages not listed there won't appear in navigation.
- **Deploy:** happens automatically on push to `main`; no manual step needed.

## File Structure (session bookkeeping)

Maintain the following file structure:

- `CLAUDE.md`: this file, as an overview.
- `LOGBOOK.md`: a short summary of each session, with links to `plans/`.
- `plans/`: collects all detailed plans.
- `STATUS.md`: written at the end of each session to document the current state.

## Session Protocol

- **Always at session start:** read `LOGBOOK.md` (historical decisions) and `STATUS.md` (current
  project state).
- **Always after a plan has been approved:** create a new `plans/PLAN-YYYY-MM-DD-ShortTitle.md` file
  and add an entry to `LOGBOOK.md` with a link to the plan.
- **Always at session end:** update `LOGBOOK.md` with a short summary of the session and replace
  `STATUS.md` with the new current (detailed) status.
