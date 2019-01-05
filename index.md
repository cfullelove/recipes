---
title: Recipe Repository
---

# Recipes

{% for recipe in site.recipes | %}
- [{{ recipe.title }} - ({{recipe.tags}})]({{ recipe.url}})
{% endfor %}

{% for recipe in site.recipes | %}
## {{ recipe.title }}

{{ recipe | jsonify }}

`{{ recipe | jsonify }}`

{{ recipe | inspect }}

`{{ recipe | inspect }}`

{% endfor %}

## Debug

- Directory: {{ site.recipes.directory }}
- Relative Directory: {{ site.recipes.relative_directory}}

{{ site.recipes | inspect }}

{{ site.collections | inspect }}