---
layout: archive
title: "Environmental Planning and Review Projects"
permalink: /portfolio/environmental-planning/
author_profile: true
skill_names:
  - "Environmental Planning and Review"
---

[Return to all portfolio skills]({{ '/portfolio/' | relative_url }})

I combine geographic research, resource screening, and written analysis to support environmental review and project planning.

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

