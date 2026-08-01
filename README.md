# INF 420: The Information Society — Online Textbook

Open online textbook for **INF 420 The Information Society** at Dominican University's School of Information Studies (Fall 2026), by Timothy D. Bowman, Ph.D.

**Live site:** https://tdbowman.github.io/420infosociety.github.io/

Companion to the [INF 110 Foundations of Informatics book](https://tdbowman.github.io/110informatics.github.io/), built with the same stack.

## Stack

- [MyST Markdown](https://mystmd.org/) content
- [Jupyter Book 2](https://jupyterbook.org/) (`jupyter-book` npm CLI) for building
- GitHub Actions → GitHub Pages for deployment (`.github/workflows/deploy.yml`)

## Local development

```bash
npm install -g jupyter-book
jupyter-book start        # live-reload dev server
jupyter-book build --html # production build to _build/html
```

## Deployment

Push to `main`; the GitHub Actions workflow builds and deploys to GitHub Pages automatically. In the repo settings, set **Pages → Source → GitHub Actions** the first time.

## Structure

- `myst.yml` — site config and table of contents
- `intro.md`, `about-this-book.md`, `how-to-use.md`, `assignments-and-timeline.md` — front matter
- `module-XX-*/` — one folder per course module: an overview page plus 2–3 section pages and an `images/` folder
- `module-09-review/` — midterm review week (peer-review workshop 1)
- `glossary.md`, `references.md`, `course-wrapup.md` — resources and wrap-up

## Status

Fall 2026 edition: all 14 modules complete. Reading list fully updated and link-verified July 2026.
