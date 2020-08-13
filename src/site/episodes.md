---
title: Episodes
layout: layouts/base.njk
subtitle: A full archive of episodes.
---
<ul class="listing">
{%- for page in collections.episode -%}
  <li>
    <a href="{{ page.url }}">{{ page.data.title }}</a> -
    <time datetime="{{ page.date }}">{{ page.date | dateDisplay("LLLL d, y") }}</time><br />
    {{ content | safe }}
  </li>
{%- endfor -%}
</ul>

