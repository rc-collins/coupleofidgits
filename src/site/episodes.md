---
title: Episodes
layout: layouts/base.njk
subtitle: A full archive of episodes.
---

{%- if collections.season0 -%}
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
{%- endif -%}

{%- if collections.season1 -%}

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
{%- endif -%}

{%- if collections.season2 -%}

### Season 2

<ul class="listing">
{%- for page in collections.season2 -%}
  <li>
    <a href="{{ page.url }}">{{ page.data.title }}</a> -
    <time datetime="{{ page.date }}">{{ page.date | dateDisplay("LLLL d, y") }}</time>
    <br />
    {{ page.content | safe }}
  </li>
{%- endfor -%}
</ul>
{%- endif -%}

{%- if collections.season3 -%}

### Season 3

<ul class="listing">
{%- for page in collections.season3 -%}
  <li>
    <a href="{{ page.url }}">{{ page.data.title }}</a> -
    <time datetime="{{ page.date }}">{{ page.date | dateDisplay("LLLL d, y") }}</time>
    <br />
    {{ page.content | safe }}
  </li>
{%- endfor -%}
</ul>
{%- endif -%}

{%- if collections.season4 -%}

### Season 4

<ul class="listing">
{%- for page in collections.season4 -%}
  <li>
    <a href="{{ page.url }}">{{ page.data.title }}</a> -
    <time datetime="{{ page.date }}">{{ page.date | dateDisplay("LLLL d, y") }}</time>
    <br />
    {{ page.content | safe }}
  </li>
{%- endfor -%}
</ul>
{%- endif -%}

