---
layout: archive
title: "Development Workflow and Collaboration Projects"
permalink: /portfolio/development-workflow/
author_profile: true
skill_names:
  - "Development Workflow and Collaboration"
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
