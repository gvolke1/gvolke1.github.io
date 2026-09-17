---
layout: archive
title: "Cartography and Data Visualization Projects"
permalink: /portfolio/cartography/
author_profile: true
skill_names:
  - "Cartography and Data Visualization"
  - "Cartography, Graphic Design and Data Visualization"
---

[Return to all portfolio skills]({{ '/portfolio/' | relative_url }})

I design maps and visualizations that explain geographic patterns, support comparisons, and respond to questions from project stakeholders.

{% assign project_count = 0 %}
<ul>
{% for post in site.portfolio %}
  {% assign matches_skill = false %}
  {% for skill_name in page.skill_names %}
    {% if post.skills contains skill_name %}
      {% assign matches_skill = true %}
    {% endif %}
  {% endfor %}
  {% if matches_skill %}
    {% assign project_count = project_count | plus: 1 %}
    <li><a href="{{ post.url | relative_url }}"><strong>{{ post.title }}</strong></a></li>
  {% endif %}
{% endfor %}
</ul>

{% if project_count == 0 %}
No projects have been added yet.
{% endif %}

