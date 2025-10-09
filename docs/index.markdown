---
layout: default
title: "All About Docs"
---

# Welcome to All About Docs

If you can see this, your Aviator theme is working! 🎉

{% for page in site.pages %}

- [{{ page.title | default: page.name }}]({{ page.url | relative_url }})
  {% endfor %}
