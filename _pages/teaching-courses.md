---
layout: page
permalink: /teaching-courses/
title: Courses
description:
years: [Spring 2025, Fall 2024, Spring 2024, Fall 2023, Spring 2023, Fall 2022, Spring 2022, Fall 2021, Spring 2021, Fall 2020, Spring 2020, Fall 2019, Spring 2019,  Fall 2018, Spring 2018, Fall 2017, Spring 2017, Fall 2016, Spring 2016, Fall 2015, Spring 2015, Fall 2014, Spring 2014, Fall 2013]
nav: false
heading: Courses
---

Below are listed all the courses that I have taught as the primary instructor since arriving to the US in 2013, with
links to their respective websites.  

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f classes -q @*[year={{y}}]* %}
{% endfor %}

</div>