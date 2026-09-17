---
layout: archive
title: "Dashboards and Business Intelligence Projects"
permalink: /portfolio/business-intelligence/
author_profile: true
skill_names:
  - "Application Prototyping, Dashboards and Business Intelligence"
  - "Dashboards and Business Intelligence"
---

[Return to all portfolio skills]({{ '/portfolio/' | relative_url }})

I help turn operational needs into dashboard components, organizational charts, and workflow prototypes that teams can develop and use.

{% assign project_count = 0 %}
<ul>
{% for post in site.portfolio %}
  {% assign matches_skill = false %}
  {% for skill_name in page.skill_names %}
    {% if post.skills contains skill_name %}
      {% assign matches_skill = true %}
    {% endif %}
  {% endfor %}
  {% if matches_skill %}
    {% assign project_count = project_count | plus: 1 %}
    <li><a href="{{ post.url | relative_url }}"><strong>{{ post.title }}</strong></a></li>
  {% endif %}
{% endfor %}
</ul>

{% if project_count == 0 %}
No projects have been added yet.
{% endif %}

