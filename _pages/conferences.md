---
layout: page
permalink: /conferences/
title: Conferences
description: 
years: [2024,2023,2022,2021]
nav: true
nav_order: 1
---
<!-- _pages/conferences.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f conferences -q @*[year={{y}}]* %}
{% endfor %}

</div>
