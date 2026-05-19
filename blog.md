---
layout: page
title: Blog
permalink: /blog/
---

{%- assign posts = site.posts | where_exp: "p", "p.draft != true" -%}
{% include post-list.html posts=posts %}
