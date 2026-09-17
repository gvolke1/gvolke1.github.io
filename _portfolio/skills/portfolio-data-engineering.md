---
layout: archive
title: "Data Engineering and API Integration Projects"
permalink: /portfolio/data-engineering/
author_profile: true
skill_names:
  - "Data Engineering and API Integration"
---

[Return to all portfolio skills]({{ '/portfolio/' | relative_url }})

I develop workflows that retrieve, clean, transform, and connect data from APIs, GIS services, and other sources.

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
