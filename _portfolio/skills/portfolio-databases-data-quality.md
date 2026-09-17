---
layout: archive
title: "Databases and Data Quality Projects"
permalink: /portfolio/databases-data-quality/
author_profile: true
skill_names:
  - "Databases and Data Quality"
---

[Return to all portfolio skills]({{ '/portfolio/' | relative_url }})

I organize and maintain database and GIS records, checking that their structure and attributes support the work they are intended to inform.

### Capabilities
- PostgreSQL and SQL workflows
- GIS database maintenance
- Attribute and schema checks
- Metadata and record consistency

{% assign project_count = 0 %}
<ul>
{% for post in site.portfolio %}
  {% if post.skills contains page.skill_names[0] %}
    {% assign project_count = project_count | plus: 1 %}
    <li><a href="{{ post.url | relative_url }}"><strong>{{ post.title }}</strong></a></li>
  {% endif %}
{% endfor %}
</ul>

{% if project_count == 0 %}
No projects have been added yet.
{% endif %}

[Professional experience]({{ '/professional-experience/' | relative_url }}) | [Portfolio by skill]({{ '/portfolio/' | relative_url }})
