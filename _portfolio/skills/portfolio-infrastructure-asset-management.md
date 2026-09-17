---
layout: archive
title: "Infrastructure and Asset Management Projects"
permalink: /portfolio/infrastructure-asset-management/
author_profile: true
skill_names:
  - "Infrastructure and Asset Management"
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
