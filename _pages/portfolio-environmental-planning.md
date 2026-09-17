---
layout: archive
title: "Environmental Planning and Review Projects"
permalink: /portfolio/environmental-planning/
author_profile: true
skill_id: environmental-planning
---

[Return to all portfolio skills]({{ '/portfolio/' | relative_url }})

I combine geographic research, resource screening, and written analysis to support environmental review and project planning.

### Capabilities
- Resource screening and GIS overlays
- Environmental review support
- Agency coordination
- Cultural and natural resource analysis

{% assign project_count = 0 %}
<ul>
{% for post in site.portfolio %}
  {% if post.skill_types contains "environmental-planning" %}
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
