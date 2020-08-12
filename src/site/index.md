---
title: Couple of Idjits
subtitle: Watching Supernatural and talking about it everyday. 
layout: layouts/base.njk
---


## Hosts

- Penny Sam
- Dan Collins


## Post pages

The pages found in in the posts

<ul class="listing">
{%- for page in collections.post -%}
  <li>
    <a href="{{ page.url }}">{{ page.data.title }}</a> -
    <time datetime="{{ page.date }}">{{ page.date | dateDisplay("LLLL d, y") }}</time>
  </li>
{%- endfor -%}
</ul>
