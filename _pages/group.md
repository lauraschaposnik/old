---
layout: page
permalink: /group/
title: Research Group
description:  
years: [Postdoc, UIC, Other]
nav: false
heading: Research Group
---

<div class="publications">

In the last decade I have mentored several students at different levels, and more recently, I have slowly started to build a research group at UIC working on geometric problems in the interface of mathematical physics, string theory and other areas of science. Below you can find the current members of the group, and you can see a <a href="https://lauraschaposnik.com/collaborators/"> list of collaborators here</a> and a <a href="https://lauraschaposnik.com/visitors/"> list of visitors here</a>. 
 
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


<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f past -q @*[year={{y}}]* %}
{% endfor %}

 
