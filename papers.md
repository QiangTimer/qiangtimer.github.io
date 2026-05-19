---
layout: page
title: Papers
permalink: /papers/
---

{% for paper in site.papers %}
<div class="paper-card">
  <a href="{{ paper.url | relative_url }}"><strong>{{ paper.title }}</strong></a>
  {%- if paper.venue -%}<br>{{ paper.venue }}{%- endif -%}
  {%- if paper.year -%} · {{ paper.year }}{%- endif -%}
</div>
{% endfor %}
