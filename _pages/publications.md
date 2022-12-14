---
layout: page
order: 2
permalink: /publications/
title: Publications
description: 
years: [2023, 2022, 2021, 2020, 2019, 2018, 2017, 2016, 2015, 2014, 2013]
nav: false
heading: Publications
---

<!-- _pages/publications.md -->

<script>
function filterSubject(filter) {
  var list = document.getElementById("publicationList");
  var rows = list.getElementsByClassName("row");
  
  // Loop through all rows, hide those which don't match the selected filter
  for (i = 0; i < rows.length; i++) {
    var primaryClass = rows[i].getElementsByClassName("category-tag")[0];
	if (primaryClass.textContent.indexOf(filter) > -1) {
        rows[i].style.display = "";
    } else {
        rows[i].style.display = "none";
    }
  }
  
  // Loop through all sections, hide those which are empty
  var years = list.getElementsByClassName("year");
  for (i = 0; i < years.length; i++) {
    var count = 0;
    for (j = 0; j < rows.length; j++) {
	  var section_tag = rows[j].getElementsByClassName("section-tag")[0];
	  if (section_tag.textContent == years[i].textContent && rows[j].style.display == "") { count++; }
	}
	if (count != 0) {
	  years[i].style.display = "";
	} else {
	  years[i].style.display = "none";
	}
  }
}
</script>

My research program is dedicated to the study of the geometry and topology of the moduli spaces of Higgs bundles, integrable systems and decorated bundles, and the geometric structures they parametrize.   In particular, I am interested in understanding  of branes of Higgs bundles,  dualities within quiver varieties in general, and within generalized hyperpolygons in particular, with views towards applications to the Langlands program for wild Hitchin systems. In a different direction, I am interested in the appearances  of  geometric structures and symmetries within different areas of sciences, which has led to some publications in applied mathematics. You can see my work in each area by clicking on the links below.

<center>
<p>
<abbr class="{{site.data.badge_colors['darkgrey']}}" onclick="filterSubject('')" style="cursor: pointer;">all</abbr>&ensp;
<abbr class="{{site.data.badge_colors['darkgrey']}}" onclick="filterSubject('geometry')" style="cursor: pointer;">geometry</abbr>&ensp;
<abbr class="{{site.data.badge_colors['darkgrey']}}" onclick="filterSubject('applied')" style="cursor: pointer;">interdisciplinary</abbr>
</p>
</center>

My <b>45+ pieces</b> both within geometry as well as on other topics are listed below in reverse chronological order by year. Note that authors on all of my publications appear alphabetically except in our Nature Scientific Reports paper, where authors are by contribution.
Citations to my papers can be found on <a href="https://scholar.google.com/citations?user=5cLd6dIAAAAJ&hl=en">Google Scholar</a>.
Paper tags are colored as follows:
<span class="badge badge-danger">journal article</span> <span class="badge badge-primary">conference article</span> <span class="badge badge-warning">editorial work</span> <span class="badge badge-light">manuscript</span> .

<div id="publicationList" class="publications">
 
{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
