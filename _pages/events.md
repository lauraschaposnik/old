---
layout: page
title: events
permalink: /events/
description: A growing collection of your events.
nav: true
display_categories: [RTG Workshops, Spectral Workshops, Sonia Kovalevsky Days]
horizontal: false
---

<!-- pages/events.md -->
<div class="events">
{%- if site.enable_event_categories and page.display_categories %}
  <!-- Display categorized events -->
  {%- for category in page.display_categories %}
  <h2 class="category">{{ category }}</h2>
  {%- assign categorized_events = site.events | where: "category", category -%}
  {%- assign sorted_events = categorized_events | sort: "importance" %}
  <!-- Generate cards for each event -->
  {% if page.horizontal -%}
  <div class="container">
    <div class="row row-cols-2">
    {%- for event in sorted_events -%}
      {% include events_horizontal.html %}
    {%- endfor %}
    </div>
  </div>
  {%- else -%}
  <div class="grid">
    {%- for event in sorted_events -%}
      {% include events.html %}
    {%- endfor %}
  </div>
  {%- endif -%}
  {% endfor %}

{%- else -%}
<!-- Display events without categories -->
  {%- assign sorted_events = site.events | sort: "importance" -%}
  <!-- Generate cards for each event -->
  {% if page.horizontal -%}
  <div class="container">
    <div class="row row-cols-2">
    {%- for event in sorted_events -%}
      {% include events_horizontal.html %}
    {%- endfor %}
    </div>
  </div>
  {%- else -%}
  <div class="grid">
    {%- for event in sorted_events -%}
      {% include events.html %}
    {%- endfor %}
  </div>
  {%- endif -%}
{%- endif -%}
</div>

