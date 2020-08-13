---
title: Couple of Idjits
subtitle: Watching Supernatural and talking about it everyday, episode by episode. 
layout: layouts/base.njk
---

## Latest Episodes
<ul class="listing">
{%- for page in collections.episode | reverse -%}
  <li>
    <a href="{{ page.url }}">{{ page.data.title }}</a> -
    <time datetime="{{ page.date }}">{{ page.date | dateDisplay("LLLL d, y") }}</time>
  </li>
{%- endfor -%}
</ul>

## Subscribe

- [Stitcher](https://www.stitcher.com/podcast/couple-of-idjits)
- [XML Feed](http://cast.rocks/hosting/27557/feeds/CAURZ.jpg?e=0df284f)

## Find Us Online

- Facebook Group - [Armchair Hunters](https://www.facebook.com/groups/437248500580788/)
- Email - [coupleofidjits.podcast@gmail.com](mailto:coupleofidjits.podcast@gmail.com)
- Penny Samuelson - [Facebook](https://www.facebook.com/penny.samuelsonconderman)
- Daniel Conderman - [YouTube](https://www.youtube.com/danconderman), [Facebook](https://www.facebook.com/conderman)

