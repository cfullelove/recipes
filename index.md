---
title: Recipe Repository
---

# Recipes

{% for recipe in site.recipes | %}
| [{{ recipe.title }}]({{ recipe.url | relative_url }}) | {{recipe.tags}} |
{% endfor %}