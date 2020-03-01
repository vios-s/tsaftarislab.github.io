---
title: "Team"
permalink: /team/
---
![Team]({{ base_path }}/assets/images/team/team.jpg)

If you want to join the team as a PhD student or a PostDoc, read about open
positions [here]({{ base_path }}/join_us/). If you wish to join the group as an
MSc or undergraduate student, drop Prof. Tsaftaris an email so we can arrange to
chat.

## Academic Staff

{% for member in site.team %}
  {% if member.role == "staff" %}  
    {% include team/member.html %}
  {% endif %}
{% endfor %}

## Post-doctoral Researchers

{% for member in site.team %}
  {% if member.role == "postdoc" %}  
    {% include team/member.html %}
  {% endif %}
{% endfor %}

## PhD Students

{% for member in site.team %}
  {% if member.role == "phd" %}  
    {% include team/member.html %}
  {% endif %}
{% endfor %}


## Visiting Students

{% for member in site.team %}
  {% if member.role == "visiting" %}  
    {% include team/member.html %}
  {% endif %}
{% endfor %}

## Alumni

* Dr. Mario Valerio Giuffrida (PhD/PostDoc) - Lecturer, Napier University,
  United Kingdom
* Mr. Hao Chen (BEng) - MSc Student, Carnegie Mellon University, United States
* Dr. Thomas Joyce (PostDoc) - PostDoc, ETH Zurich, Switzerland
* Dr. Ilkay Oksuz (PhD) - PostDoc, King's College London, United Kingdom
* Dr. Massimo Minervini (PhD/PostDoc) - CET Electronics, Italy
* Dr. Cristian Rusu (PostDoc) - Lecturer, National University of Ireland,
  Ireland
* Dr. Marco Bevilacqua (PostDoc) - PostDoc, Bordeaux, INP, France
* Dr. Anirban Mukhopadhyay (PostDoc) - Head, Medical and Environmental Computing
 (MEC-Lab), TU Darmstadt, Germany
