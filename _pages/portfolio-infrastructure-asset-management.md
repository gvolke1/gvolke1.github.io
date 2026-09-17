---
layout: archive
title: "Infrastructure and Asset Management Projects"
permalink: /portfolio/infrastructure-asset-management/
author_profile: true
skill_id: infrastructure-asset-management
---

[Return to all portfolio skills]({{ '/portfolio/' | relative_url }})

I maintain geographic and operational information that supports infrastructure planning, construction, and ongoing updates.

### Capabilities
- Fiber and utility mapping
- Construction and asset records
- Cost and inspection support
- Operational GIS updates

{% assign project_count = 0 %}
<ul>
{% for post in site.portfolio %}
  {% if post.skill_types contains "infrastructure-asset-management" %}
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
