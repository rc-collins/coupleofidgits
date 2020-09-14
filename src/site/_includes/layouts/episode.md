---
layout: layouts/base.njk
pageClass: episode
templateEngineOverride: njk, md
---

<p class="date">
  <time datetime="{{ date }}">{{ date | dateDisplay }}</time>
</p>
<main>
  {{ content | safe }}
  <h2>{{ season }}</h2>
  <ul class="podcasts">
  {%- if season == 'Season 1' -%}
    {%- for page in collections.season1 -%}
      <li>
        <a href="{{ page.url }}">{{ page.data.title }}</a> -
        <time datetime="{{ page.date }}">{{ page.date | dateDisplay("LLLL d, y") }}</time>
        <br />
        {{ page.content | safe }}
      </li>
    {%- endfor -%}
  {%- endif -%}
  {%- if season == 'Season 2' -%}
    {%- for page in collections.season2 -%}
      <li>
        <a href="{{ page.url }}">{{ page.data.title }}</a> -
        <time datetime="{{ page.date }}">{{ page.date | dateDisplay("LLLL d, y") }}</time>
        <br />
        {{ page.content | safe }}
      </li>
    {%- endfor -%}
  {%- endif -%}
  {%- if season == 'Season 3' -%}
    {%- for page in collections.season3 -%}
      <li>
        <a href="{{ page.url }}">{{ page.data.title }}</a> -
        <time datetime="{{ page.date }}">{{ page.date | dateDisplay("LLLL d, y") }}</time>
        <br />
        {{ page.content | safe }}
      </li>
    {%- endfor -%}
  {%- endif -%}
  {%- if season == 'Season 4' -%}
    {%- for page in collections.season4 -%}
      <li>
        <a href="{{ page.url }}">{{ page.data.title }}</a> -
        <time datetime="{{ page.date }}">{{ page.date | dateDisplay("LLLL d, y") }}</time>
        <br />
        {{ page.content | safe }}
      </li>
    {%- endfor -%}
  {%- endif -%}
  {%- if season == 'Season 5' -%}
    {%- for page in collections.season5 -%}
      <li>
        <a href="{{ page.url }}">{{ page.data.title }}</a> -
        <time datetime="{{ page.date }}">{{ page.date | dateDisplay("LLLL d, y") }}</time>
        <br />
        {{ page.content | safe }}
      </li>
    {%- endfor -%}
  {%- endif -%}
  {%- if season == 'Season 6' -%}
    {%- for page in collections.season6 -%}
      <li>
        <a href="{{ page.url }}">{{ page.data.title }}</a> -
        <time datetime="{{ page.date }}">{{ page.date | dateDisplay("LLLL d, y") }}</time>
        <br />
        {{ page.content | safe }}
      </li>
    {%- endfor -%}
  {%- endif -%}
  {%- if season == 'Season 7' -%}
    {%- for page in collections.season7 -%}
      <li>
        <a href="{{ page.url }}">{{ page.data.title }}</a> -
        <time datetime="{{ page.date }}">{{ page.date | dateDisplay("LLLL d, y") }}</time>
        <br />
        {{ page.content | safe }}
      </li>
    {%- endfor -%}
  {%- endif -%}
  {%- if season == 'Season 8' -%}
    {%- for page in collections.season8 -%}
      <li>
        <a href="{{ page.url }}">{{ page.data.title }}</a> -
        <time datetime="{{ page.date }}">{{ page.date | dateDisplay("LLLL d, y") }}</time>
        <br />
        {{ page.content | safe }}
      </li>
    {%- endfor -%}
  {%- endif -%}
  {%- if season == 'Season 9' -%}
    {%- for page in collections.season9 -%}
      <li>
        <a href="{{ page.url }}">{{ page.data.title }}</a> -
        <time datetime="{{ page.date }}">{{ page.date | dateDisplay("LLLL d, y") }}</time>
        <br />
        {{ page.content | safe }}
      </li>
    {%- endfor -%}
  {%- endif -%}
  {%- if season == 'Season 10' -%}
    {%- for page in collections.season10 -%}
      <li>
        <a href="{{ page.url }}">{{ page.data.title }}</a> -
        <time datetime="{{ page.date }}">{{ page.date | dateDisplay("LLLL d, y") }}</time>
        <br />
        {{ page.content | safe }}
      </li>
    {%- endfor -%}
  {%- endif -%}
  {%- if season == 'Season 11' -%}
    {%- for page in collections.season11 -%}
      <li>
        <a href="{{ page.url }}">{{ page.data.title }}</a> -
        <time datetime="{{ page.date }}">{{ page.date | dateDisplay("LLLL d, y") }}</time>
        <br />
        {{ page.content | safe }}
      </li>
    {%- endfor -%}
  {%- endif -%}
  {%- if season == 'Season 12' -%}
    {%- for page in collections.season12 -%}
      <li>
        <a href="{{ page.url }}">{{ page.data.title }}</a> -
        <time datetime="{{ page.date }}">{{ page.date | dateDisplay("LLLL d, y") }}</time>
        <br />
        {{ page.content | safe }}
      </li>
    {%- endfor -%}
  {%- endif -%}
  {%- if season == 'Season 13' -%}
    {%- for page in collections.season13 -%}
      <li>
        <a href="{{ page.url }}">{{ page.data.title }}</a> -
        <time datetime="{{ page.date }}">{{ page.date | dateDisplay("LLLL d, y") }}</time>
        <br />
        {{ page.content | safe }}
      </li>
    {%- endfor -%}
  {%- endif -%}
  {%- if season == 'Season 14' -%}
    {%- for page in collections.season14 -%}
      <li>
        <a href="{{ page.url }}">{{ page.data.title }}</a> -
        <time datetime="{{ page.date }}">{{ page.date | dateDisplay("LLLL d, y") }}</time>
        <br />
        {{ page.content | safe }}
      </li>
    {%- endfor -%}
  {%- endif -%}
  </ul>
  </div>
</main>
