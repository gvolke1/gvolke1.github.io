---
layout: archive
title: "Emergency Management and Public Safety Analytics Projects"
permalink: /portfolio/emergency-management/
author_profile: true
skill_id: emergency-management
---

[Return to all portfolio skills]({{ '/portfolio/' | relative_url }})

I prepare geographic and operational data to support understanding of hazards, emergency demand, infrastructure, and population characteristics.

### Capabilities
- CAD and incident analysis
- Hazard and exposure mapping
- Travel-time and resource coverage
- Demand and risk assessment

{% assign project_count = 0 %}
<ul>
{% for post in site.portfolio %}
  {% if post.skill_types contains "emergency-management" %}
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
