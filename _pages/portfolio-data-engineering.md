---
layout: archive
title: "Data Engineering and API Integration Projects"
permalink: /portfolio/data-engineering/
author_profile: true
skill_id: data-engineering
---

[Return to all portfolio skills]({{ '/portfolio/' | relative_url }})

I develop workflows that retrieve, clean, transform, and connect data from APIs, GIS services, and other sources.

### Capabilities
- API and service integration
- Data extraction, cleaning, and transformation
- GeoJSON and spatial-data preparation
- ETL workflows and schema organization

{% assign project_count = 0 %}
<ul>
{% for post in site.portfolio %}
  {% if post.skill_types contains "data-engineering" %}
    {% assign project_count = project_count | plus: 1 %}
    <li style="margin-bottom: 1.25rem;">
      <a href="{{ post.url | relative_url }}"><strong>{{ post.title }}</strong></a>
      <div style="margin-top: 0.25rem;">{{ post.skill_contributions[page.skill_id] }}</div>
    </li>
  {% endif %}
{% endfor %}
</ul>

{% if project_count == 0 %}
No projects have been added yet.
{% endif %}

[Professional experience]({{ '/professional-experience/' | relative_url }}) | [Portfolio by skill]({{ '/portfolio/' | relative_url }})
