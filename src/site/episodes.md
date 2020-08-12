---
title: Episodes
layout: layouts/base.njk
subtitle: A full archive of episodes.
---
{%- for episode in collections.episodes -%}
<a href="{{ episode.url }}">{{ episode.data.title }}</a><br/>
{%- endfor -%}

<ul>
{%- for episode in collections.all -%}
  <li><a href="{{ post.url }}">{{ post.url }}</a></li>
{%- endfor -%}
</ul>
