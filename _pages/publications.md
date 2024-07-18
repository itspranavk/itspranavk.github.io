---
layout: page
permalink: /publications/
title: Publications
description: 
years: [2024,2023,2022,Under Review]
nav: true
nav_order: 1
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  {% if y == "Under Review" -%}
    <h2 class="under_review">{{y}}</h2>
  {%- else -%}
    <h2 class="year">{{y}}</h2>
  {%- endif %}
  
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
