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
  {% if 'Season 1' in season %}
    {%- for page in collections.season1 -%}
      <li>
        <a href="{{ page.url }}">{{ page.data.title }}</a> -
        <time datetime="{{ page.date }}">{{ page.date | dateDisplay("LLLL d, y") }}</time>
        <br />
        {{ page.content | safe }}
      </li>
    {%- endfor -%}
  {%- endif -%}
  {% if 'Season 2' in season %}
    {%- for page in collections.season2 -%}
      <li>
        <a href="{{ page.url }}">{{ page.data.title }}</a> -
        <time datetime="{{ page.date }}">{{ page.date | dateDisplay("LLLL d, y") }}</time>
        <br />
        {{ page.content | safe }}
      </li>
    {%- endfor -%}
  {%- endif -%}
  {% if 'Season 3' in season %}
    {%- for page in collections.season3 -%}
      <li>
        <a href="{{ page.url }}">{{ page.data.title }}</a> -
        <time datetime="{{ page.date }}">{{ page.date | dateDisplay("LLLL d, y") }}</time>
        <br />
        {{ page.content | safe }}
      </li>
    {%- endfor -%}
  {%- endif -%}
  {% if 'Season 4' in season %}
    {%- for page in collections.season4 -%}
      <li>
        <a href="{{ page.url }}">{{ page.data.title }}</a> -
        <time datetime="{{ page.date }}">{{ page.date | dateDisplay("LLLL d, y") }}</time>
        <br />
        {{ page.content | safe }}
      </li>
    {%- endfor -%}
  {%- endif -%}
  {% if 'Season 5' in season %}
    {%- for page in collections.season5 -%}
      <li>
        <a href="{{ page.url }}">{{ page.data.title }}</a> -
        <time datetime="{{ page.date }}">{{ page.date | dateDisplay("LLLL d, y") }}</time>
        <br />
        {{ page.content | safe }}
      </li>
    {%- endfor -%}
  {%- endif -%}
  {% if 'Season 6' in season %}
    {%- for page in collections.season6 -%}
      <li>
        <a href="{{ page.url }}">{{ page.data.title }}</a> -
        <time datetime="{{ page.date }}">{{ page.date | dateDisplay("LLLL d, y") }}</time>
        <br />
        {{ page.content | safe }}
      </li>
    {%- endfor -%}
  {%- endif -%}
  {% if 'Season 7' in season %}
    {%- for page in collections.season7 -%}
      <li>
        <a href="{{ page.url }}">{{ page.data.title }}</a> -
        <time datetime="{{ page.date }}">{{ page.date | dateDisplay("LLLL d, y") }}</time>
        <br />
        {{ page.content | safe }}
      </li>
    {%- endfor -%}
  {%- endif -%}
  {% if 'Season 8' in season %}
    {%- for page in collections.season8 -%}
      <li>
        <a href="{{ page.url }}">{{ page.data.title }}</a> -
        <time datetime="{{ page.date }}">{{ page.date | dateDisplay("LLLL d, y") }}</time>
        <br />
        {{ page.content | safe }}
      </li>
    {%- endfor -%}
  {%- endif -%}
  {% if 'Season 9' in season %}
    {%- for page in collections.season9 -%}
      <li>
        <a href="{{ page.url }}">{{ page.data.title }}</a> -
        <time datetime="{{ page.date }}">{{ page.date | dateDisplay("LLLL d, y") }}</time>
        <br />
        {{ page.content | safe }}
      </li>
    {%- endfor -%}
  {%- endif -%}
  {% if 'Season 10' in season %}
    {%- for page in collections.season10 -%}
      <li>
        <a href="{{ page.url }}">{{ page.data.title }}</a> -
        <time datetime="{{ page.date }}">{{ page.date | dateDisplay("LLLL d, y") }}</time>
        <br />
        {{ page.content | safe }}
      </li>
    {%- endfor -%}
  {%- endif -%}
  {% if 'Season 11' in season %}
    {%- for page in collections.season11 -%}
      <li>
        <a href="{{ page.url }}">{{ page.data.title }}</a> -
        <time datetime="{{ page.date }}">{{ page.date | dateDisplay("LLLL d, y") }}</time>
        <br />
        {{ page.content | safe }}
      </li>
    {%- endfor -%}
  {%- endif -%}
  {% if 'Season 12' in season %}
    {%- for page in collections.season12 -%}
      <li>
        <a href="{{ page.url }}">{{ page.data.title }}</a> -
        <time datetime="{{ page.date }}">{{ page.date | dateDisplay("LLLL d, y") }}</time>
        <br />
        {{ page.content | safe }}
      </li>
    {%- endfor -%}
  {%- endif -%}
  {% if 'Season 13' in season %}
    {%- for page in collections.season13 -%}
      <li>
        <a href="{{ page.url }}">{{ page.data.title }}</a> -
        <time datetime="{{ page.date }}">{{ page.date | dateDisplay("LLLL d, y") }}</time>
        <br />
        {{ page.content | safe }}
      </li>
    {%- endfor -%}
  {%- endif -%}
  {% if 'Season 14' in season %}
    {%- for page in collections.season14 -%}
      <li>
        <a href="{{ page.url }}">{{ page.data.title }}</a> -
        <time datetime="{{ page.date }}">{{ page.date | dateDisplay("LLLL d, y") }}</time>
        <br />
        {{ page.content | safe }}
      </li>
    {%- endfor -%}
  {%- endif -%}
  <br class="clear" />
  </div>
</main>
