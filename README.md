# qiangtimer.github.io

Jekyll blog for [https://qiangtimer.github.io/](https://qiangtimer.github.io/). You write Markdown; GitHub Pages builds the site.

## Content folders

| Folder | Purpose | URL |
|--------|---------|-----|
| `_posts/` | Long articles | `/blog/YYYY/MM/DD/title/` |
| `_briefs/` | Short research notes | `/briefs/name/` |
| `_papers/` | Paper index (PDF/DOI links) | `/papers/name/` |
| `_series/` | Series landing pages | `/series/name/` |
| `_disclosure/` | Sanitized advisories | `/disclosure/name/` |

Edit site title and meta in `_config.yml`. Edit homepage intro in `index.md`, bio in `about.md`.

## Add a blog post

Create `_posts/2026-05-20-my-title.md`:

```yaml
---
title: Your title
date: 2026-05-20
categories: [firmware]
tags: [ipc, analysis]
series: my-series        # optional, matches _series/*.md series_id
series_order: 1        # optional
excerpt: One-line summary for lists.
---

Your Markdown content.
```

Filename must be `YYYY-MM-DD-slug.md`.

## Add a brief / paper / series / disclosure

Copy the matching `example-*` file in `_briefs/`, `_papers/`, `_series/`, or `_disclosure/`, rename, set `published: true` (or remove `published: false`), fill front matter and body.

**Series:** `_series/foo.md` uses `series_id: foo`. Posts/briefs use `series: foo` to link and auto-list on the series page.

## Hide without deleting

```yaml
published: false
```

## Local preview

```bash
bundle install
bundle exec jekyll serve
```

Open http://127.0.0.1:4000

## Deploy

Push to `main` on GitHub. Enable **Settings → Pages → Source: Deploy from branch → main / (root)** if not already.
