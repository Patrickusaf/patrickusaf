---
layout: archive
permalink: /motor/
title: "Motorcycles"
excerpt: "Motorcycles"
author_profile: false
---

## Motorcycles

<h3 class="archive__subtitle">{{ site.data.ui-text[site.locale].recent_posts | default: "Recent Posts" }}</h3>

{% for post in paginator.posts %}
  {% include archive-single.html %}
{% endfor %}

{% include paginator.html %}

{% include base_path %}
{% assign author = site.author %}
