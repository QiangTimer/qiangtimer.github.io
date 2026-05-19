# Authoring guide

## Add a brief

Create `_writings/{series}/briefs/{slug}.md`

```yaml
---
title: Your title
date: 2026-05-20
series: firmware
type: brief
excerpt: One-line summary.
tags: [taxonomy]
---

Body (Markdown).
```

URL: `/series/firmware/briefs/{slug}/`

## Add an analysis

Create `_writings/{series}/analysis/{slug}.md`

```yaml
---
title: Your title
date: 2026-05-20
series: firmware
type: analysis
excerpt: One-line summary.
tags: [hk20, crypto]
---

## Context
## Observation
## Method
## Judgment
## Implication
```

URL: `/series/firmware/analysis/{slug}/`

## Series IDs

`agent` · `vulnerability` · `firmware` · `network-probing` · `offense-defense`

## Draft / hide

```yaml
published: false
```

## Disclosure

Create `_disclosure/{slug}.md` with `series`, `cve`, `status`, etc. See `example-advisory.md`.

## Local preview

```bash
bundle install && bundle exec jekyll serve
```
