---
title: "About"

excerpt: "VIOS collaboratory is part of the Institute for Digital
          Communications in The School of Engineering at The University of
          Edinburgh."
header:
  overlay_filter: 0.75
  overlay_image: homepage.jpg

layout: splash
permalink: /
---
Welcome to our VIOS collaboratory. VIOS (pronounced vEEOs) means life (Βίος) in
Greek; in its common English writing *bio* is abound in science as the word
denoting everything about life (biology, biomedicine, bioimaging)... Life is
central to our mission.  With advances in artificial intelligence, computer
vision and inverse problems our mission is to solve key challenges in the life
and natural sciences addressing societal problems.  

## News
{% for post in site.posts limit:5 %}
  * **{{ post.title }}**: {{ post.excerpt | remove: '<p>' | remove: '</p>' }}
{% endfor %}

<a href="/news" class="btn btn--info btn--small">Read More</a>

{% include about-bottom.html %}
