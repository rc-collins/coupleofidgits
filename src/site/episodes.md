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

<h2>Season 1</h2>

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

<h2>Season 2</h2>

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

<h2>Season 3</h2>

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

<h2>Season 4</h2>

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


{%- if collections.season5 -%}

<h2>Season 5</h2>

<ul class="listing">
{%- for page in collections.season5 -%}
  <li>
    <a href="{{ page.url }}">{{ page.data.title }}</a> -
    <time datetime="{{ page.date }}">{{ page.date | dateDisplay("LLLL d, y") }}</time>
    <br />
    {{ page.content | safe }}
  </li>
{%- endfor -%}
</ul>
{%- endif -%}



{%- if collections.season6 -%}

<h2>Season 6</h2>

<ul class="listing">
{%- for page in collections.season6 -%}
  <li>
    <a href="{{ page.url }}">{{ page.data.title }}</a> -
    <time datetime="{{ page.date }}">{{ page.date | dateDisplay("LLLL d, y") }}</time>
    <br />
    {{ page.content | safe }}
  </li>
{%- endfor -%}
</ul>
{%- endif -%}



{%- if collections.season7 -%}

<h2>Season 7</h2>

<ul class="listing">
{%- for page in collections.season7 -%}
  <li>
    <a href="{{ page.url }}">{{ page.data.title }}</a> -
    <time datetime="{{ page.date }}">{{ page.date | dateDisplay("LLLL d, y") }}</time>
    <br />
    {{ page.content | safe }}
  </li>
{%- endfor -%}
</ul>
{%- endif -%}

