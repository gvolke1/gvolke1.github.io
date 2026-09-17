---
layout: archive
title: "Web GIS and Development Projects"
permalink: /portfolio/web-development/
author_profile: true
skill_names:
  - "Web Development"
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

[Professional experience]({{ '/professional-experience/' | relative_url }}) | [Portfolio by skill]({{ '/portfolio/' | relative_url }})