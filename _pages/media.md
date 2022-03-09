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
 
 My work within geometry as well as on interdisciplinary areas and outreach has been featured in several media outlets. Here you can find a quasi complete list, with information on the topic appearing in the <b>Abs</b> buttons, and links to the media within the title. 

<div id="publicationList" class="publications">
 
{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f media -q @*[year={{y}}]* %}
{% endfor %}

</div>