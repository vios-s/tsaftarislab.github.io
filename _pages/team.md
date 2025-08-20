---
title: "Team"

permalink: /team/
sidebar:
  nav: "team"
---

{% assign banners = "team.jpg|team4.jpg|team5.jpg|team6.jpg" | split: "|" %}

<link rel="stylesheet" href="https://unpkg.com/swiper@11/swiper-bundle.min.css">

<div class="swiper team-banner-swiper" style="--swiper-navigation-color:#000;--swiper-pagination-color:#000;">
  <div class="swiper-wrapper">
    {% for img in banners %}
      <div class="swiper-slide">
        <img
          src="{{ base_path }}/assets/images/team/{{ img }}"
          alt="Team banner {{ forloop.index }}"
          style="width:100%;height:auto;display:block;"
          loading="lazy"
        />
      </div>
    {% endfor %}
  </div>

{% assign banners_count = banners | size %}
{% if banners_count > 1 %}
<div class="swiper-pagination"></div>
<div class="swiper-button-prev" aria-label="Previous banner"></div>
<div class="swiper-button-next" aria-label="Next banner"></div>
{% endif %}

</div>

<script src="https://unpkg.com/swiper@11/swiper-bundle.min.js"></script>
<script>
(function(){
  if (window.__teamSwiperInitDone) return;
  window.__teamSwiperInitDone = true;

  var count = {{ banners | size }};
  var options = {
    slidesPerView: 1,
    loop: count > 1,
    autoplay: count > 1 ? { delay: 4000, disableOnInteraction: false } : false,
    spaceBetween: 0,
    pagination: count > 1 ? { el: '.team-banner-swiper .swiper-pagination', clickable: true } : {},
    navigation: count > 1 ? {
      nextEl: '.team-banner-swiper .swiper-button-next',
      prevEl: '.team-banner-swiper .swiper-button-prev'
    } : {}
  };
  window.__teamSwiper = new Swiper('.team-banner-swiper', options);
})();
</script>

If you want to join the team as a PhD student or a PostDoc, read about open
positions [here]({{ base_path }}/join_us/). If you wish to join the group as an
MSc or undergraduate student, drop [Academic Staff] an email to arrange a chat.

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

## Software Engineer {#sde}

{% for member in site.team %}
{% if member.role == "sde" %}  
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

- Dr [Fasih Haider](https://scholar.google.com/citations?hl=en&user=9xYJHP8AAAAJ) (PostDoc) - University of Edinburgh
- Dr [Jingshuai Liu](https://scholar.google.com/citations?hl=en&user=_a-15AgAAAAJ) (PostDoc) - Chongqing University, China
- Dr [Pedro Sanchez](https://www.ppsanchez.com/) (PhD) - Sinkove
- Dr [Andrew Wood]() (Software Engineer) - Lloyds Banking Group
- Dr [Jinghan Sun](https://scholar.google.com/citations?hl=en&user=T0ru9jYAAAAJ) (Visiting Member) - Tencent
- Dr [Xiao Liu](https://www.linkedin.com/in/xiao-liu-020b59158/) (PhD) - Huawei
- Mr [Grzegorz Jacenków](https://www.linkedin.com/in/jacenkow/) (PhD) - Data Scientist at Amazon
- Dr [Nikolaos Dionelis](https://uk.linkedin.com/in/nikolaos-dionelis-60688279) (PostDoc) - Joint Research Centre, EU
- Dr [John Hartley](https://www.linkedin.com/in/john-hartley-4b37219b) (PostDoc) - Data Scientist at Natwest Group
- Mr [Victor Campello](https://www.linkedin.com/in/v%C3%ADctor-m-campello-b3b635130) (Visiting PhD) - PhD at Universitat de Barcelona
- Dr [Chen Qin](https://sites.google.com/view/chen-qin/) (Lecturer) - Lecturer/Assistant Professor, Imperial College, London
- Dr [Spyridon Thermos](https://spthermo.github.io/) (PostDoc) - Startup Founder
- Dr [Tian Xia](https://www.linkedin.com/in/tian-xia-67b5b8109/) (PhD) - PostDoc at The University of Edinburgh, Scotland
- Mr [Andrei Dobrescu](https://www.linkedin.com/in/andreidobrescu/) (PhD) - Computer Vision Researcher at CattleEye
- Mr Phivos Sofokleous (MSc)
- Dr [Gabriele Valvano](https://www.linkedin.com/in/gabriele-valvano/?locale=en_US) (Visiting PhD) - Lead AI Specialist, Baker Hughes, Italy
- Dr Haochuan Jiang (PostDoc) - Lecturer, Xi'an Jiaotong-Liverpool University, China
- Dr Agisilaos Chartsias (PhD) - Deep Learning Resarch Scientist, Ultromics, United Kingdom
- Mr [Hao Chen](https://www.linkedin.com/in/haochen97) (BEng) - PhD Student,
  Carnegie Mellon University, United States
- Dr [Thomas Joyce](https://biomed.ee.ethz.ch/institute/People/person-detail.MjU0MzMx.TGlzdC8yNTA2LC0xMTc1NTEzMTIz.html)
  (PostDoc) - PostDoc, ETH Zurich, Switzerland
- Dr [Ilkay Oksuz](https://sites.google.com/view/oksuzilkay) (PhD) - Assistant
  Professor, Istanbul Technical University, Turkey
- Dr [Massimo Minervini](https://www.linkedin.com/in/minervini/) (PhD/PostDoc) -
  CET Electronics, Italy
- Dr [Cristian Rusu](https://www.ncirl.ie/About/A-Z-Staff-Directory/Staff/347)
  (PostDoc) - IIT
- Dr [Marco Bevilacqua](https://www.linkedin.com/in/marcobevilacqua) (PostDoc) -
  Data Scientist, Cdiscount, France
- Dr [Anirban Mukhopadhyay](https://sites.google.com/site/geometricanirban/)
  (PostDoc) - Head, Medical and Environmental Computing (MEC-Lab), TU Darmstadt,
  Germany
