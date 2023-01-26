---
layout: page
permalink: /publications/
title: publications
description: Publications in reverse chronological order.
years: [2023, 2022, 2019, 2016, 2014, 2013]
nav: true
nav_order: 3
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
