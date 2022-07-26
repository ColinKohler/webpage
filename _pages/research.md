---
title: "Research"
layout: collection
permalink: /research/
author_profile: true
classes: wide
---

A complete list of plublications can be found at [Google Scholar](https://scholar.google.com/citations?hl=en&user=QuFhQt0AAAAJ).

---

{% assign works = site.research | sort: "order" | reverse %}

{% for work in works %}
  {% assign pdf = work.pdf %}
  {% assign code = work.code %}
  {% assign website = work.website %}
  {% assign cite = work.cite %}
  <h2> {{ work.title }} ({{ work.year }}) </h2>
  {{ work.authors }} --- {{ work.publication }}
  <p float="left">
    {% include button.html button_name="PDF" onclick=pdf button_class="primary" %}
    {% include button.html button_name="Code" onclick=code button_class="primary" %}
    {% include button.html button_name="Website" onclick=website button_class="primary" %}
    {% include button.html button_name="Cite" onclick=cite button_class="primary" %}
  </p>
  **Abstract:** {{ work.abstract }}

  ---
{% endfor %}
