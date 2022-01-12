---
layout: archive 
title: "Blog"
permalink: /blog/
author_profile: true
---

{% for collection in site.collections %}
  {% if collection.label == "posts" %} {% continue %} {% endif %} 
  <h2 id="{{ collection.label | slugify %}}" class="archive__subtitle">{{ collection.label }}</h2>

  {% for post in collection.docs %}
    {% include archive-single.html %}
  {% endfor %}
{% endfor %}
