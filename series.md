---
layout: page
title: Series
permalink: /series/
---

{% for s in site.series %}
- [{{ s.title }}]({{ s.url | relative_url }}){%- if s.description -%} — {{ s.description }}{%- endif -%}
{% endfor %}
