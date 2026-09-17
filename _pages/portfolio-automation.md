---
layout: archive
title: "Automation and Workflow Improvement Projects"
permalink: /portfolio/automation/
author_profile: true
skill_id: automation
---

[Return to all portfolio skills]({{ '/portfolio/' | relative_url }})

I improve recurring processes by replacing repetitive manual steps with reusable scripts, GIS uploads, and standardized workflows.

### Capabilities
- Process redesign
- GIS upload automation
- Map production automation
- Repeatable geoprocessing

{% assign project_count = 0 %}
<ul>
{% for post in site.portfolio %}
  {% if post.skill_types contains "automation" %}
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
