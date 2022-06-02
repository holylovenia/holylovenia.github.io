---
layout: page
permalink: /publications/
title: publications
description: complete and up-to-date list of publications can be accessed [here](https://scholar.google.co.id/citations?user=bugb-lAAAAAJ&hl=en).
years: [2019, 2021, 2022]
nav: true
nav_order: 2
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
