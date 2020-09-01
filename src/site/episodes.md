---
title: Episodes
layout: layouts/base.njk
subtitle: A full archive of episodes.
---

### Season 1

<ul class="listing">
{%- for page in collections.season1 -%}
  <li>
    <a href="{{ page.url }}">{{ page.data.title }}</a> -
    <time datetime="{{ page.date }}">{{ page.date | dateDisplay("LLLL d, y") }}</time>
    <br />
    {{ page.content | safe }}
  </li>
{%- endfor -%}
</ul>


### Bonus Content

<ul class="listing">
{%- for page in collections.season0 -%}
  <li>
    <a href="{{ page.url }}">{{ page.data.title }}</a> -
    <time datetime="{{ page.date }}">{{ page.date | dateDisplay("LLLL d, y") }}</time>
    <br />
    {{ page.content | safe }}
  </li>
{%- endfor -%}
</ul>
