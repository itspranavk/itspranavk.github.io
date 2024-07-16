---
layout: page
permalink: /conferences/
title: Conference Publications
description: 
years: [2024,2023,2022,2021]
nav: true
nav_order: 2
---
<!-- _pages/conferences.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f conferences -q @*[year={{y}}]* %}
{% endfor %}

</div>
