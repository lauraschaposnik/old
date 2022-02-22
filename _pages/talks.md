---
layout: page
permalink: /talks/
title: Talks
description:  
years: [2022, 2021, 2020, 2019, 2018, 2017, 2016, 2015, 2014, 2013]
nav: false
heading: Talks
---


<div class="publications">


I have given <b>100+ talks</b> on my research area as well as outreach talks over the years. Below you can find a quasi complete list of them where I have classified them as
<span class="badge badge-danger">Conference</span> <span class="badge badge-primary">Seminar</span> <span class="badge badge-warning">Colloquia, Plenary talk or mini course </span>  and <span class="badge badge-light">Outreach</span> .


{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f talks -q @*[year={{y}}]* %}
{% endfor %}

</div>
