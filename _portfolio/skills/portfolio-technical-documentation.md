---
layout: archive
title: "Technical Documentation and Knowledge Transfer Projects"
permalink: /portfolio/technical-documentation/
author_profile: true
skill_names:
  - "Technical Documentation and Knowledge Transfer"
---

[Return to all portfolio skills]({{ '/portfolio/' | relative_url }})

I document methods, requirements, and procedures so colleagues can understand, review, and repeat the work.

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

