---
title: "About"

excerpt: "VIOS /vEEOs/ Collaboratory is part of the Institute for Digital
          Communications in The School of Engineering at The University of
          Edinburgh."
header:
  overlay_filter: 0.75
  overlay_image: homepage.jpg

layout: splash
permalink: /
---
Our research interests are machine learning, deep learning, medical image
analysis (medical image computing), and image processing. Core research
application domains are computer aided diagnosis in medicine and computer vision
in agriculture (e.g. plant phenotyping, precision agriculture, agritech and
indoor farming).

## News
{% for post in site.posts limit:5 %}
  * **{{ post.title }}**: {{ post.excerpt | remove: '<p>' | remove: '</p>' }}
{% endfor %}

<a href="/news" class="btn btn--info btn--small">Read More</a>

{% include about-bottom.html %}
