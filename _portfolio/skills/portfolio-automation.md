---
layout: archive
title: "Automation and Workflow Improvement Projects"
permalink: /portfolio/automation/
author_profile: true
skill_names:
  - "Automation and Workflow Improvement"
---

[Return to all portfolio skills]({{ '/portfolio/' | relative_url }})

I improve recurring processes by replacing repetitive manual steps with reusable scripts, GIS uploads, and standardized workflows.

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

