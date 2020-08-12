---
title: Episodes
layout: layouts/base.njk
subtitle: A full archive of episodes.
---
{%- for page in collections.post -%}
<a href="{{ page.url }}">{{ page.data.title }}</a><br/>
{%- endfor -%}
