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

  <ol>
    <li>{% if page.url != pagination.href.first %}<a href="{{ pagination.href.first }}">First</a>{% else %}First{% endif %}</li>
    <li>{% if pagination.href.previous %}<a href="{{ pagination.href.previous }}">Previous</a>{% else %}Previous{% endif %}</li>
{%- for pageEntry in pagination.pages %}
    <li><a href="{{ pagination.hrefs[ loop.index0 ] }}"{% if page.url == pagination.hrefs[ loop.index0 ] %} aria-current="page"{% endif %}>Page {{ loop.index }}</a></li>
{%- endfor %}
    <li>{% if pagination.href.next %}<a href="{{ pagination.href.next }}">Next</a>{% else %}Next{% endif %}</li>
    <li>{% if page.url != pagination.href.last %}<a href="{{ pagination.href.last }}">Last</a>{% else %}Last{% endif %}</li>
  </ol>


  <h2>{{ season }}</h2>
  <ul class="podcasts">
  {%- if season == 'Season 1' -%}
    {%- for page in collections.season1 -%}
      <li>
        <a href="{{ page.url }}">{{ page.data.title }}</a> -
        <time datetime="{{ page.date }}">{{ page.date | dateDisplay("LLLL d, y") }}</time>
        <br />
        {{ page.content | safe }}
    {%- endfor -%}
  {%- endif -%}
  {%- if season == 'Season 2' -%}
    {%- for page in collections.season2 -%}
      <li>
        <a href="{{ page.url }}">{{ page.data.title }}</a> -
        <time datetime="{{ page.date }}">{{ page.date | dateDisplay("LLLL d, y") }}</time>
        <br />
        {{ page.content | safe }}
    {%- endfor -%}
  {%- endif -%}
  {%- if season == 'Season 3' -%}
    {%- for page in collections.season3 -%}
      <li>
        <a href="{{ page.url }}">{{ page.data.title }}</a> -
        <time datetime="{{ page.date }}">{{ page.date | dateDisplay("LLLL d, y") }}</time>
        <br />
        {{ page.content | safe }}
    {%- endfor -%}
  {%- endif -%}
  {%- if season == 'Season 4' -%}
    {%- for page in collections.season4 -%}
      <li>
        <a href="{{ page.url }}">{{ page.data.title }}</a> -
        <time datetime="{{ page.date }}">{{ page.date | dateDisplay("LLLL d, y") }}</time>
        <br />
        {{ page.content | safe }}
    {%- endfor -%}
  {%- endif -%}
  {%- if season == 'Season 5' -%}
    {%- for page in collections.season5 -%}
      <li>
        <a href="{{ page.url }}">{{ page.data.title }}</a> -
        <time datetime="{{ page.date }}">{{ page.date | dateDisplay("LLLL d, y") }}</time>
        <br />
        {{ page.content | safe }}
    {%- endfor -%}
  {%- endif -%}
  {%- if season == 'Season 6' -%}
    {%- for page in collections.season6 -%}
      <li>
        <a href="{{ page.url }}">{{ page.data.title }}</a> -
        <time datetime="{{ page.date }}">{{ page.date | dateDisplay("LLLL d, y") }}</time>
        <br />
        {{ page.content | safe }}
    {%- endfor -%}
  {%- endif -%}
  </div>
</main>
