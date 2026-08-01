# Status

_Last updated: 2026-08-01_

## Current State

- MkDocs Material documentation site, deployed to GitHub Pages on push to `main`.
- Session bookkeeping scaffolding lives in `.claude/`: `CLAUDE.md`, `LOGBOOK.md`, `STATUS.md`,
  `plans/`. `.claude/CLAUDE.md` is auto-loaded as project memory in new sessions (per official docs).

### Site content present (per `mkdocs.yml` nav)

- **Home:** `docs/index.md`
- **Prompt Engineering:** `docs/prompt-eng/system-prompts.md`, `docs/prompt-eng/few-shot-guides.md`
- **Development:** `docs/development/agent-design.md`, `docs/development/evaluation.md`
- **Security:** `docs/security/data-privacy.md`
- **Resources:** `docs/resources/links.md`

## Verified

- **Maintenance files do not affect the site build (2026-08-01):** `mkdocs build` generates only the
  6 real docs pages (+ `index.html`, `404.html`). The bookkeeping files now live in `.claude/`, well
  outside `docs_dir` (`docs/`), so MkDocs never picks them up — they produce no pages, no
  `sitemap.xml` entries, and no search-index entries. They are git-maintenance artifacts only.

## Pending / Next Steps

- None currently. Flesh out content pages as needed.
