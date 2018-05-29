---
layout: archive
permalink: /motor/
title: "Motorcycles"
excerpt: "Motorcycles"
author_profile: false
---

## Motorcycles

<h3 class="archive__subtitle">{{ site.data.ui-text[site.locale].recent_posts | default: "Recent Posts" }}</h3>

<ul>
{% for post in site.posts %}
  <li>
    <a href="{% post.permalink %}">{% post.title %}</a>
    <p>{{ post.excerpt }}</p>
  </li>
{% endfor %}
</ul>

{% include paginator.html %}

{% include base_path %}
{% assign author = site.author %}
