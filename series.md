---
layout: page
title: Research Series
permalink: /series/
---

Continuous research threads. Each series publishes **Briefs** (short insight) and **Analysis** (observation + method + judgment).

<div class="series-grid">
{% for s in site.series_list %}
<article class="series-card">
  <h3><a href="{{ '/series/' | append: s.id | append: '/' | relative_url }}">{{ s.title }}</a></h3>
  <p class="series-card__subtitle">{{ s.subtitle }}</p>
</article>
{% endfor %}
</div>
