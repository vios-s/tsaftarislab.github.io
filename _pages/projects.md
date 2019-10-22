---
title: "Projects"
permalink: /projects/
---

{% for project in site.projects reversed %}
  {% include projects/projects.html %}
{% endfor %}
