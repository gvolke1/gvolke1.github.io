---
layout: archive
title: "Web GIS and Development Projects"
permalink: /portfolio/web-development/
author_profile: true
skill_id: web-development
---

[Return to all portfolio skills]({{ '/portfolio/' | relative_url }})

I build interactive web maps and application services that make geographic and operational information easier to access.

### Capabilities
- JavaScript, HTML, CSS, and Leaflet-based interfaces
- Front-end data integration for GIS and operational data
- Web mapping and application service workflows
- Project-based geospatial product delivery

{% assign project_count = 0 %}
<ul>
{% for post in site.portfolio %}
  {% if post.skill_types contains "web-development" %}
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