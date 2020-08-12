---
title: Episodes
layout: layouts/base.njk
subtitle: A full archive of episodes.
---

{%- for episode in collections.episodes -%}
<a href="{{ episode.url }}">{{ episode.data.title }}</a><br/>
{%- endfor -%}


<ul class="listing">
{%- for page in collections.episodes -%}
  <li>
    <a href="{{ page.url }}">{{ page.data.title }}</a> -
    <time datetime="{{ page.date }}">{{ page.date | dateDisplay("LLLL d, y") }}</time>
  </li>
{%- endfor -%}
</ul>
