---
title: Recipe Repository
layout: index
---

# Recipes

| Recipe | Tags   |
|---|---|
{% for recipe in site.recipes | sort -%}
| [{{ recipe.title }}]({{ recipe.url | relative_url }}) | {{ recipe.tags }} |
{% endfor -%}