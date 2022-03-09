---
layout: page
order: 2
permalink: /media/
title: Media
description: 
years: [2009]
nav: false
heading: Media
---
 
 

<div id="publicationList" class="publications">
 
{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f media -q @*[year={{y}}]* %}
{% endfor %}

</div>
