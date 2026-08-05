---
layout: archive
title: "GIS and Spatial Analysis Projects"
permalink: /portfolio/spatial-analysis/
author_profile: true
---

[Return to all portfolio skills]({{ '/portfolio/' | relative_url }})

{% assign project_count = 0 %}

<ul>
{% for post in site.portfolio %}
  {% if post.skill_types contains "spatial-analysis" %}
    {% assign project_count = project_count | plus: 1 %}
    <li>
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    </li>
  {% endif %}
{% endfor %}
</ul>

{% if project_count == 0 %}
No spatial analysis projects have been added yet.
{% endif %}