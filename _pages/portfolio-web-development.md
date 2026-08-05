---
layout: archive
title: "Web GIS and Development Projects"
permalink: /portfolio/web-development/
author_profile: true
---
[Return to all portfolio skills]({{ '/portfolio/' | relative_url }})

{% assign project_count = 0 %}

<ul>
{% for post in site.portfolio %}
  {% if post.skill_types contains "developer" %}
    {% assign project_count = project_count | plus: 1 %}
    <li>
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    </li>
  {% endif %}
{% endfor %}
</ul>

{% if project_count == 0 %}
No development projects have been added yet.
{% endif %}