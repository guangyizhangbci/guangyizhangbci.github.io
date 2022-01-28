---
layout: page
permalink: /publications/
title: publications
description: publications by categories in chronological order
years: [2018,2019,2020,2021,2022]
nav: true
---
<!-- _pages/publications.md -->
<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
