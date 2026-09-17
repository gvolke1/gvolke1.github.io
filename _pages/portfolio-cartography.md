---
layout: archive
title: "Cartography and Data Visualization Projects"
permalink: /portfolio/cartography/
author_profile: true
skill_id: cartography
---

[Return to all portfolio skills]({{ '/portfolio/' | relative_url }})

I design maps and visualizations that explain geographic patterns, support comparisons, and respond to questions from project stakeholders.

### Capabilities
- Thematic mapping and statistical classification
- Symbology, dashboards, and map-layer organization
- Construction mapbooks and public-facing map products
- Visual communication for decision support and stakeholder review

{% assign project_count = 0 %}
<ul>
{% for post in site.portfolio %}
  {% if post.skill_types contains "cartography" %}
    {% assign project_count = project_count | plus: 1 %}
    <li style="margin-bottom: 1.25rem;">
      <a href="{{ post.url | relative_url }}"><strong>{{ post.title }}</strong></a>
      <div style="margin-top: 0.25rem;">{{ post.skill_contributions[page.skill_id] }}</div>
    </li>
  {% endif %}
{% endfor %}
</ul>

{% if project_count == 0 %}
No cartography projects have been added yet.
{% endif %}

[Professional experience]({{ '/professional-experience/' | relative_url }}) | [Portfolio by skill]({{ '/portfolio/' | relative_url }})