---
layout: page
order: 2
permalink: /media/
title: Media
description: 
years: [2022, 2021, 2020, 2019, 2018, 2017, 2016, 2015, 2014, 2013]
nav: false
heading: Media
---
 
 

<div id="publicationList" class="publications">
 
{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f media -q @*[year={{y}}]* %}
{% endfor %}

</div>
