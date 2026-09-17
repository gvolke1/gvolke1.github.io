---
layout: archive
title: "GIS and Spatial Analysis Projects"
permalink: /portfolio/spatial-analysis/
author_profile: true
skill_id: spatial-analysis
---

[Return to all portfolio skills]({{ '/portfolio/' | relative_url }})

I prepare and analyze geographic data, troubleshoot spatial relationships, and select methods that fit the question and available information.

### Capabilities
- QGIS, ArcGIS, GeoPandas, and geocoding workflows
- Spatial joins, H3 indexing, and travel-time isochrones
- Parcel and infrastructure analysis for planning decisions
- Data troubleshooting and method selection for project needs

{% assign project_count = 0 %}
<ul>
{% for post in site.portfolio %}
  {% if post.skill_types contains "spatial-analysis" %}
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