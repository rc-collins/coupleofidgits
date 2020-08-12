---
title: Episodes
layout: layouts/base.njk
subtitle: A full archive of episodes.
---

{%- for episode in collections.episode -%}
<a href="{{ episode.url }}">{{ episode.data.title }}</a><br/>
{%- endfor -%}

<hr>

<ul class="listing">
{%- for page in collections.episode -%}
  <li>
    <a href="{{ page.url }}">{{ page.data.title }}</a> -
    <time datetime="{{ page.date }}">{{ page.date | dateDisplay("LLLL d, y") }}</time>
  </li>
{%- endfor -%}
</ul>

