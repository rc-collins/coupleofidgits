---
layout: layouts/base.njk
pageClass: episodes
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
    {%- for page in collections.episode -%}
    <li><a href="{{ page.url }}">{{ page.data.title }}</a></li>
    {%- endfor -%}
  {% endif %}
  </ul>
  <br class="clear" />
  </div>
</main>
