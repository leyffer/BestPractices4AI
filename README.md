# BestPractices4AI

A curated collection of best practices, notes, and links for working with AI, published as a documentation site built with [MkDocs](https://www.mkdocs.org/) and [Material for MkDocs](https://squidfunk.github.io/mkdocs-material/).

**Live site:** https://leyffer.github.io/BestPractices4AI/

## Local development

```bash
pip install -r requirements.txt
mkdocs serve
```

Then open <http://localhost:8000>. Pages live under `docs/`; site structure and theme are configured in `mkdocs.yml`.

To check the build the same way CI does:

```bash
mkdocs build --strict
```

## Deployment

Pushing to `main` triggers the GitHub Actions workflow (`.github/workflows/deploy.yml`), which runs `mkdocs gh-deploy` to publish the site to the `gh-pages` branch.

> **One-time setup:** after the first successful workflow run, go to **Settings → Pages** and set the source to the **`gh-pages` branch** so the site goes live.

## Claude integration

See [.claude](.claude/) contains the usual `CLAUDE.md` and other useful files for working with claude on this project,
