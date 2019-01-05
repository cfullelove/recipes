---
title: Recipe Repository
---

# Recipes

{% for recipe in site.recipes | %}
- [{{ recipe.title }} - ({{recipe.tags}})]({{ recipe.url | relative_url }})
{% endfor %}

## Debug


{{ site.collections | inspect }}

{% for recipe in site.recipes | %}
## {{ recipe.title }}

```
{{ recipe | inspect }}
```

{% endfor %}
