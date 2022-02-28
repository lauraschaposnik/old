---
layout: page
order: 2
permalink: /publications/
title: Publications
description: 
years: [2022, 2021, 2020, 2019, 2018, 2017, 2016, 2015, 2014, 2013]
nav: false
heading: Publications
---

<!-- _pages/publications.md -->
<div class="publications">


My research program is dedicated to the study of the geometry and topology of the moduli spaces of Higgs bundles, integrable systems and decorated bundles, and the geometric structures they parametrize.   In particular, I am interested in understanding  of branes of Higgs bundles,  dualities within quiver varieties in general, and within generalized hyperpolygons in particular, with views towards applications to the Langlands program for wild Hitchin systems. 

<br>
<br>

In a different direction, I am interested in the appearences of  geometric structures and patterns, and in particular symmetries, within different areas of sciences. This secondary side of my research  can be thought of as divided into  three main themes:  Patterns and viruses;  Patterns within human behaviour; and Patterns within crystals and plants.

<br>
<br>

My <b>45+ pieces</b> both within geometry as well as on other topics are listed below in reverse chronological order by year. Note that authors on all of my publications appear alphabetically except in our Nature Scientific Reports paper, where authors are by contribution.
Citations to my papers can be found on <a href="https://scholar.google.com/citations?user=5cLd6dIAAAAJ&hl=en">Google Scholar</a>.
Paper tags are colored as follows:
<span class="badge badge-danger">journal article</span> <span class="badge badge-primary">conference article</span> <span class="badge badge-warning">editorial work</span> <span class="badge badge-light">manuscript</span> .


{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
