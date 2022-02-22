---
layout: page
permalink: /events/
title: Events
description:  
years: [2023, 2022, 2021, 2020, 2019, 2018, 2017, 2016, 2015, 2014]
nav: false
heading: Events organized
---


<div class="publications">


 
I draw a lot of inspiration for my research and teaching through interactions with people across fields, and because of this I keep an active role organizing international events, graduate schools and outreach events. Below you can find a quasi complete list of the <b>40+ different events</b> I have organized.  


{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f events -q @*[year={{y}}]* %}
{% endfor %}

</div>
