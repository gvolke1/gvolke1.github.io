---
layout: archive
title: "Project Coordination and Stakeholder Communication Projects"
permalink: /portfolio/project-coordination/
author_profile: true
skill_id: project-coordination
---

[Return to all portfolio skills]({{ '/portfolio/' | relative_url }})

I coordinate technical work with developers, agency staff, service providers, and other stakeholders to resolve questions and move projects forward.

### Capabilities
- Stakeholder communication
- Requirements clarification
- Workflow coordination
- Technical handoffs

{% assign project_count = 0 %}
<ul>
{% for post in site.portfolio %}
  {% if post.skill_types contains "project-coordination" %}
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
