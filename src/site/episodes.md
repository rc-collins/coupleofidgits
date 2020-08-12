---
title: Episodes
layout: layouts/base.njk
subtitle: A full archive of episodes.
---

{%- for episode in collections.episodes -%}
<a href="{{ episode.url }}">{{ episode.data.title }}</a><br/>
{%- endfor -%}

