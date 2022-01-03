---
layout: page
permalink: /publications/
title: publications
description: Check my <a href="https://scholar.google.com/citations?user={{ site.scholar_userid }}" title="Google Scholar">Google Scholar</a> profile for an up-to-date list of publications.
years: [2022, 2021, 2020]
nav: true
order: 1
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
