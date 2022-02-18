---
layout: page
permalink: /students/
title: Students
description:  
years: [2022, 2021, 2020, 2019, 2018, 2017, 2016, 2015, 2014, 2013]
nav: false
heading: Students
---

<div class="publications">

In the last decade I have mentored several students at different levels. Below is a list of my former and current students.  To find more information about my broader "academic family" visit my <a href="https://www.mathgenealogy.org/id.php?id=171532">genealogy</a> entry. 

<h2>Current</h2>
 
 {%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f current -q @*[year={{y}}]* %}
{% endfor %}

</div>


<h2>Former</h2>
In reverse chronological order

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f past -q @*[year={{y}}]* %}
{% endfor %}

 
