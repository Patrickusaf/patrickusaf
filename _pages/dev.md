---
permalink: /dev/
title: "dev"
excerpt: "Dev"
author_profile: true
---

## Software Development

{% include group-by-array collection=site.posts field="dev" %}

{% for tag in group_names %}
  {% assign posts = group_items[forloop.index0] %}
  <h2 id="{{ tag | slugify }}" class="archive__subtitle">{{ tag }}</h2>
  {% for post in posts %}
    {% include archive-single.html %}
  {% endfor %}
{% endfor %}
