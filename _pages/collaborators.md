---
layout: page
permalink: /collaborators/
title: Collaborators
description:  
years: [2022, 2021, 2020, 2019, 2018, 2017, 2016, 2015]
nav: false
heading: Collaborators
---

<div class="publications">


I thoroughly enjoy working with researchers within my area as well as in other other areas of science and humanities. Below is a list of the collaborators with whom I have published papers.


{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f collaborators -q @*[year={{y}}]* %}
{% endfor %}

</div>
