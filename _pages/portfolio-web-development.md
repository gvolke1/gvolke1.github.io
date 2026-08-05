---
layout: archive
title: "Web GIS and Development Projects"
permalink: /portfolio/web-development/
author_profile: true
---

[Return to all portfolio skills]({{ '/portfolio/' | relative_url }})

These projects demonstrate web development, interactive mapping,
application development, and related technical skills.

<div class="grid__wrapper">
{% assign project_count = 0 %}

{% for post in site.portfolio %}
  {% if post.skill_types contains "developer" %}
    {% assign project_count = project_count | plus: 1 %}
    {% include archive-single.html type="grid" %}
  {% endif %}
{% endfor %}
</div>

{% if project_count == 0 %}
No development projects have been added yet.
{% endif %}