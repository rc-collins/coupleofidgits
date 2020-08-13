---
title: Couple of Idjits
subtitle: Watching Supernatural and talking about it everyday. 
layout: layouts/base.njk
---

## Latest Episodes
<ul class="listing">
{%- for page in collections.episode -%}
  <li>
    <a href="{{ page.url }}">{{ page.data.title }}</a> -
    <time datetime="{{ page.date }}">{{ page.date | dateDisplay("LLLL d, y") }}</time>
  </li>
{%- endfor -%}
</ul>

## Find Us Online

- Penny Samuelson - [Facebook](https://www.facebook.com/penny.samuelsonconderman)
- Daniel Conderman - [YouTube](https://www.youtube.com/danconderman), [Facebook](https://www.facebook.com/conderman)

