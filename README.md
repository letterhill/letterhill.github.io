# Quarto Portfolio Starter

A minimal Quarto + GitHub Pages starter focused on **Jupyter notebooks** organized by **folders**.

## Quick Start

1) Create a new GitHub repository named **USERNAME.github.io** (replace USERNAME).
2) Download this starter and extract it.
3) Initialize Git and push:

```bash
git init
git add .
git commit -m "init portfolio"
git branch -M main
git remote add origin https://github.com/USERNAME/USERNAME.github.io.git
git push -u origin main
```

4) Enable GitHub Pages (Settings → Pages). Set **Branch** to `gh-pages`. (The workflow below will create and update `gh-pages` automatically.)
5) Push changes—GitHub Actions will build & publish your site.

## Add a new notebook

- Save your notebook under `notebooks/<topic>/<name>.ipynb`
- Add a top Markdown cell with a YAML header:

```markdown
---
title: "Week 1 — Linear Regression"
date: 2025-08-14
categories: [ML, Study]
description: "From hypothesis to gradient descent"
---
```

- Commit and push. After the workflow finishes, your notebook appears on **Study Notes**.

## Local preview (optional)

Install Quarto from https://quarto.org, then run:

```bash
quarto preview
```

## Notes

- The GitHub Action uses `quarto-dev/quarto-actions` to render this site and publish to `gh-pages`.
- Customize `_quarto.yml` for theme, navbar, etc.