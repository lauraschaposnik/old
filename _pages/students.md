---
layout: page
permalink: /students/
title: Students
description:  
years: [UIC, Other]
nav: false
heading: Students
---

<div class="publications">

In the last decade I have mentored several students at different levels. Below is a list of my former and current students.  To find more information about my broader "academic family" visit my <a href="https://www.mathgenealogy.org/id.php?id=171532">genealogy</a> entry. 
 
 <br>
 <hr>
<span style="font-size:15px">

<h2>Current</h2>
 
 {%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f current -q @*[year={{y}}]* %}
{% endfor %}

  <br>

 <hr>
<span style="font-size:15px">

<h2>Former</h2>

In reverse chronological order

<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f past -q @*[year={{y}}]* %}
{% endfor %}

 
