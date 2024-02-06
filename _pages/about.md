---
title: "About"

excerpt: "Welcome to our VIOS collaboratory."
header:
  overlay_filter: 0.75
  overlay_image: homepage.jpg

layout: splash
permalink: /
---
VIOS (pronounced vEEOs) means life (Βίος) in Greek; its common English
equivalent *bio* abounds in science as the word denoting everything about life
(biology, biomedicine, bioimaging...). Life is central to our mission. With
advances in artificial intelligence (AI), computer vision and inverse problems, our
mission is to address societal problems by solving key challenges in the life
and natural sciences. This mission inspires our drive in interdisciplinary AI, where we use motivating applications to propose new AI-driven solutions. 

## News
{% for post in site.posts limit:3 %}
  * **{{ post.title }}**: {{ post.excerpt | remove: '<p>' | remove: '</p>' }}
{% endfor %}

<a href="/news" class="btn btn--info btn--small">Read More</a>

{% include about-bottom.html %}
