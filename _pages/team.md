---
title: "Team"

permalink: /team/
sidebar:
  nav: "team"
---
![Team]({{ base_path }}/assets/images/team/team.jpg)

If you want to join the team as a PhD student or a PostDoc, read about open
positions [here]({{ base_path }}/join_us/). If you wish to join the group as an
MSc or undergraduate student, drop Sotos an email to arrange a chat.

## Academic Staff {#academic}

{% assign sorted = site.team | sort: 'order' %}
{% for member in sorted %}
  {% if member.role == "staff" %}  
    {% include team/member.html %}
  {% endif %}
{% endfor %}

## Post-doctoral Researchers {#pdra}

{% for member in site.team %}
  {% if member.role == "postdoc" %}  
    {% include team/member.html %}
  {% endif %}
{% endfor %}

## PhD Students {#phd}

{% for member in site.team %}
  {% if member.role == "phd" %}  
    {% include team/member.html %}
  {% endif %}
{% endfor %}


## Visiting Students {#visiting}

{% for member in site.team %}
  {% if member.role == "visiting" %}  
    {% include team/member.html %}
  {% endif %}
{% endfor %}

## Alumni {#alumni}

* Dr Marija Jegorova (PostDoc) - Postdoctoral Researcher, Facebook AI Research, United Kingdom
* Dr Haochuan Jiang (PostDoc) - Lecturer, Xi'an Jiaotong-Liverpool University, China
* Dr Agisilaos Chartsias (PhD) - Deep Learning Resarch Scientist, Ultromics, United Kingdom
* Mr [Hao Chen](https://www.linkedin.com/in/haochen97) (BEng) - MSc Student,
  Carnegie Mellon University, United States
* Dr [Thomas Joyce](https://biomed.ee.ethz.ch/institute/People/person-detail.MjU0MzMx.TGlzdC8yNTA2LC0xMTc1NTEzMTIz.html)
  (PostDoc) - PostDoc, ETH Zurich, Switzerland
* Dr [Ilkay Oksuz](https://sites.google.com/view/oksuzilkay) (PhD) - Assistant
  Professor, Istanbul Technical University, Turkey
* Dr [Massimo Minervini](https://www.linkedin.com/in/minervini/) (PhD/PostDoc) -
  CET Electronics, Italy
* Dr [Cristian Rusu](https://www.ncirl.ie/About/A-Z-Staff-Directory/Staff/347)
  (PostDoc) - Lecturer, National University of Ireland, Ireland
* Dr [Marco Bevilacqua](https://www.linkedin.com/in/marcobevilacqua) (PostDoc) -
  Cdiscount, France
* Dr [Anirban Mukhopadhyay](https://sites.google.com/site/geometricanirban/)
  (PostDoc) - Head, Medical and Environmental Computing (MEC-Lab), TU Darmstadt,
  Germany
