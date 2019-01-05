---
title: Recipe Repository
---

# Recipes

{% for recipe in site.recipes | %}
- [{{ recipe.title }} - ({{recipe.tags}})]({{ recipe.url}})</a>
{% endfor %}
