---
layout: page
permalink: /collaborators/
title: Collaborators
description:  
years: [Argentina, Australia, Brazil, Canada, Cyprus,  France, Germany, Greece,  India, Switzerland, Turkey, UK, USA,]
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

