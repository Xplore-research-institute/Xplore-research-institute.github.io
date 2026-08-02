# Xplore Research Institute — GitHub Pages Website

A dark, responsive Jekyll website for publishing scientific articles and research content.

## 1. Create the correct repository

For an organization website, create a repository named:

```text
YOUR-ORGANIZATION-USERNAME.github.io
```

The repository name must use the exact GitHub organization username in lowercase where applicable.

## 2. Upload the website

Upload all files and folders from this package to the root of the repository and commit them to the `main` branch.

## 3. Enable GitHub Pages

Open the repository and go to:

```text
Settings → Pages → Build and deployment → Source
```

Choose **Deploy from a branch**, select **main** and **/(root)**, then save.

## Adding a new article

Duplicate one of the files in `_posts` and rename it using:

```text
YYYY-MM-DD-your-article-title.md
```

Each article begins with YAML metadata:

```yaml
---
title: "Article Title"
description: "One-sentence summary."
author: "Author Name"
category: "Physics"
tags: [Gravity, Experiment]
read_time: 6
---
```

Write the article below that section using Markdown.

## Editing publications

Open:

```text
publications/index.html
```

Duplicate a `<article class="publication-item">...</article>` block and replace the sample information.

## Important customizations

- Email: `contact/index.html`
- GitHub and ORCID links: `contact/index.html` and `publications/index.html`
- Research areas: `research/index.html`
- Institute description: `about/index.html`
- Main homepage content: `index.html`
- Logo: `assets/images/xplore-logo.jpg`

## Local preview (optional)

If Ruby and Bundler are installed:

```bash
bundle install
bundle exec jekyll serve
```

Then open `http://localhost:4000`.
