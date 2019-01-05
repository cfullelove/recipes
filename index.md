---
title: Recipe Repository
---

{% assign tags =  site.recipes | map: 'tags' | join: ','  | split: ',' | uniq %}
{% for tag in tags %}
  <h3>{{ tag }}</h3>
  <ul>
  {% for recipe in site.recipes %}
    {% if recipe.tags contains tag %}
    <li><a href="{{ site.baseurl }}{{ recipe.url }}">{{ recipe.title }}</a></li>
    {% endif %}
  {% endfor %}
  </ul>
{% endfor %}