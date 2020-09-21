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

<ul>
  {%- set nextPost = collections.posts | getNextCollectionItem(page) %}
  {%- if nextPost %}<li>Next: <a href="{{ nextPost.url | url }}">{{ nextPost.data.title }}</a></li>{% endif %}
  {%- set previousPost = collections.posts | getPreviousCollectionItem(page) %}
  {%- if previousPost %}<li>Previous: <a href="{{ previousPost.url | url }}">{{ previousPost.data.title }}</a></li>{% endif %}
</ul>


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
