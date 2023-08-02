---
layout: page
permalink: /publications/
title: Publications
description: Complete and up-to-date list of publications can be accessed via <a href='https://scholar.google.com/citations?user=bugb-lAAAAAJ' target='_blank'><u>Google Scholar</u></a>.
years: [2023, 2022, 2021, 2019]
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
