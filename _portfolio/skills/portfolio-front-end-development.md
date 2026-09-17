---
layout: archive
title: "Front End Development Projects"
permalink: /portfolio/front-end-development/
author_profile: true
skill_names:
  - "Front End Development"
---

[Return to all portfolio skills]({{ '/portfolio/' | relative_url }})

I build and integrate browser-based interfaces that make project data and functionality accessible to users.

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

