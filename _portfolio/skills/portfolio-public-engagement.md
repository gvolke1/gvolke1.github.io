---
layout: archive
title: "Demographic Analysis and Public Engagement Projects"
permalink: /portfolio/public-engagement/
author_profile: true
skill_names:
  - "Demographic Analysis and Public Engagement"
---

[Return to all portfolio skills]({{ '/portfolio/' | relative_url }})

I analyze community information and communicate project findings through maps, presentations, public materials, and outreach.

### Capabilities
- Census and demographic analysis
- Survey mapping
- Public meeting support
- Academic and stakeholder outreach

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
