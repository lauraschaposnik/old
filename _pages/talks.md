---
layout: page
permalink: /talks/
title: Talks and Trips
description:  
years: [2024,2023,2022, 2021, 2020, 2019, 2018, 2017, 2016, 2015, 2014, 2013]
nav: false
heading: Talks and Trips
---


<div class="publications">


I have given <b>150+ talks</b> on my research area as well as outreach talks over the years. Below you can find a quasi complete list of them where I have classified them as
<span class="badge badge-danger">Conference</span> <span class="badge badge-primary">Seminar</span> <span class="badge badge-warning">Colloquia, Plenary talk or mini course </span>  and <span class="badge badge-light">Outreach</span> . Trips to workshops and conferences at which I am not giving talks (which I'll be doing more often than not) appear in  <span class="badge badge-success">Trips</span> 


{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f talks -q @*[year={{y}}]* %}
{% endfor %}

</div>
