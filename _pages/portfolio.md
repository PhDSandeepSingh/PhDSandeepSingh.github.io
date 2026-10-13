---
layout: archive
title: "Research Projects & Software"
permalink: /portfolio/
author_profile: true
---

Explore my open-source research software, data engineering pipelines, and machine learning models. Each project includes reproducible code, documentation, and notebooks.

{% include base_path %}

{% for post in site.portfolio reversed %}
  {% include archive-single.html %}
{% endfor %}
