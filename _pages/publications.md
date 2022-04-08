---
layout: page
permalink: /publications/
title: publications
description: Check my Google Scholar profile for an up-to-date list of publications.
years: [2022, 2021, 2020]
nav: true
order: 2
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
