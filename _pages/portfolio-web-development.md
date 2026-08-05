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

    <li style="margin-bottom: 2rem;">
      <a href="{{ post.url | relative_url }}">
        <strong>{{ post.title }}</strong>
      </a>

      {% if post.header.teaser %}
        <a href="{{ post.url | relative_url }}">
          <img
            src="{{ post.header.teaser | prepend: '/images/' | relative_url }}"
            alt="Preview of {{ post.title }}"
            style="display: block; width: 100%; max-width: 600px; height: auto; margin-top: 0.75rem;"
          >
        </a>
      {% endif %}
    </li>

  {% endif %}
{% endfor %}
</ul>

{% if project_count == 0 %}
No development projects have been added yet.
{% endif %}