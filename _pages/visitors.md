---
layout: page
permalink: /visitors/
title: Visitors
description:  
years: [2024, 2023, 2022, 2021, 2020, 2019, 2018, 2017, 2016, 2015]
nav: false
heading: Visitors
---

<div class="publications">


Hosting visitors and interacting with colleagues is a very important part of my research, and thus I am always eager to host collaborators and colleagues at my university. Below is a list of people who have visited me in the last few years -- if you are interested in visiting in the futre, please do reach out. 


{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f visitors -q @*[year={{y}}]* %}
{% endfor %}

</div>
