---
layout: page
permalink: /talks/
title: Talks
description: my research publications
years: [2022, 2021, 2020, 2019, 2018, 2017, 2016, 2015, 2014, 2013]
nav: true
---
<!-- _pages/publications.md -->
<div class="publications">

My research spans the study of the geometry and topology of moduli spaces of decorated bundles, Hitchin systems, mirror symmetry and hyperpolygons.  My papers are listed below in reverse chronological order by year. Note that authors on all of my publications appear alphabetically except in our Nature Scientific Reports paper, where authors are by contribution.
Citations to my papers can be found on <a href="https://scholar.google.com/citations?user=5cLd6dIAAAAJ&hl=en">Google Scholar</a>.
Paper tags are colored as follows:
<span class="badge badge-danger">journal article</span> <span class="badge badge-primary">conference article</span> <span class="badge badge-warning">editorial work</span> <span class="badge badge-light">manuscript</span> .


{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
