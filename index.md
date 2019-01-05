---
title: Recipe Repository
---

{% for recipe in site.recipes | %}
    <p>
        <a href="{{ recipe.url}}">{{ recipe.title }} - ({{recipe.tags}})</a>
    </p>
{% endfor %}
