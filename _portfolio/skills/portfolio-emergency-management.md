---
layout: archive
title: "Emergency Management and Public Safety Analytics Projects"
permalink: /portfolio/emergency-management/
author_profile: true
skill_names:
  - "Emergency Management and Public Safety Analytics"
---

[Return to all portfolio skills]({{ '/portfolio/' | relative_url }})

I prepare geographic and operational data to support understanding of hazards, emergency demand, infrastructure, and population characteristics.

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

