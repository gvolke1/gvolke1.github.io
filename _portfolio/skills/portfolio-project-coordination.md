---
layout: archive
title: "Project Coordination and Stakeholder Communication Projects"
permalink: /portfolio/project-coordination/
author_profile: true
skill_names:
  - "Project Coordination and Stakeholder Communication"
---

[Return to all portfolio skills]({{ '/portfolio/' | relative_url }})

I coordinate technical work with developers, agency staff, service providers, and other stakeholders to resolve questions and move projects forward.

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

