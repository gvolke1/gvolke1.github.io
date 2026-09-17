---
layout: archive
title: "Dashboards and Business Intelligence Projects"
permalink: /portfolio/business-intelligence/
author_profile: true
skill_id: business-intelligence
---

[Return to all portfolio skills]({{ '/portfolio/' | relative_url }})

I help turn operational needs into dashboard components, organizational charts, and workflow prototypes that teams can develop and use.

### Capabilities
- Dashboards and prototypes
- Power BI and Power Apps
- Synthetic data and testing
- Interface and workflow design

{% assign project_count = 0 %}
<ul>
{% for post in site.portfolio %}
  {% if post.skill_types contains "business-intelligence" %}
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
