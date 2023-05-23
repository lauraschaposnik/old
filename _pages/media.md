---
layout: page
order: 2
permalink: /media/
title: Media
description: 
years: [2023, 2022, 2021,2020,2019,2018,2017,2016,2009]
nav: false
heading: Media
---
 
 My work within geometry as well as on interdisciplinary areas and outreach has been featured in <b> 40+ </b> media outlets. Here you can find a quasi complete list, with information on the topic appearing in the <b>Abs</b> buttons, and links to the media within the title. 

<div id="publicationList" class="publications">
 
{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f media -q @*[year={{y}}]* %}
{% endfor %}

</div>
