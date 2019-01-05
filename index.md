---
title: Recipe Repository
---

# Recipes

{% for recipe in site.recipes | %}
- [{{ recipe.title }} - ({{recipe.tags}})]({{ recipe.url}})
{% endfor %}


## Debug

- Directory: {{ site.recipes.directory }}
- Relative Directory: {{ site.recipes.relative_directory}}