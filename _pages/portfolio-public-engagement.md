---
layout: archive
title: "Demographic Analysis and Public Engagement Projects"
permalink: /portfolio/public-engagement/
author_profile: true
skill_id: public-engagement
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
  {% if post.skill_types contains "public-engagement" %}
    {% assign project_count = project_count | plus: 1 %}
    <li style="margin-bottom: 1.25rem;">
      <a href="{{ post.url | relative_url }}"><strong>{{ post.title }}</strong></a>
      <div style="margin-top: 0.25rem;">{{ post.skill_contributions[page.skill_id] }}</div>
    </li>
  {% endif %}
{% endfor %}
</ul>

{% if project_count == 0 %}
No projects have been added yet.
{% endif %}

[Professional experience]({{ '/professional-experience/' | relative_url }}) | [Portfolio by skill]({{ '/portfolio/' | relative_url }})
