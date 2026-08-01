# Status

_Last updated: 2026-08-01_

## Current State

- MkDocs Material documentation site, deployed to GitHub Pages on push to `main`.
- Session bookkeeping scaffolding is in place: `CLAUDE.md`, `LOGBOOK.md`, `STATUS.md`, `plans/`.

### Site content present (per `mkdocs.yml` nav)

- **Home:** `docs/index.md`
- **Prompt Engineering:** `docs/prompt-eng/system-prompts.md`, `docs/prompt-eng/few-shot-guides.md`
- **Development:** `docs/development/agent-design.md`, `docs/development/evaluation.md`
- **Security:** `docs/security/data-privacy.md`
- **Resources:** `docs/resources/links.md`

## Verified

- **Maintenance files do not affect the site build (2026-08-01):** `mkdocs build` generates only the
  6 real docs pages (+ `index.html`, `404.html`). `CLAUDE.md`, `LOGBOOK.md`, `STATUS.md`, and
  `plans/` live outside `docs_dir` (`docs/`), so MkDocs never picks them up — they produce no pages,
  no `sitemap.xml` entries, and no search-index entries. They are git-maintenance artifacts only.

## Pending / Next Steps

- None currently. Flesh out content pages as needed.
