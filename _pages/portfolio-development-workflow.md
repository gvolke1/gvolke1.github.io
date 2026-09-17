---
layout: archive
title: "Development Workflow and Collaboration Projects"
permalink: /portfolio/development-workflow/
author_profile: true
skill_id: development-workflow
---

[Return to all portfolio skills]({{ '/portfolio/' | relative_url }})

I organize, test, and share code so teammates can review the work and continue developing it.

### Capabilities
- GitHub collaboration
- API testing and validation
- Code review and documentation
- Python and environment management

{% assign project_count = 0 %}
<ul>
{% for post in site.portfolio %}
  {% if post.skill_types contains "development-workflow" %}
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
