---
layout: page
permalink: /publications/
title: publications
description: [Google Scholar](https://scholar.google.com/citations?user=UJWY9B0AAAAJ&hl=en)
years: [2023, 2018, 2015, 2014]
nav: true
nav_order: 1
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f {{ site.scholar.bibliography }} -q @*[year={{y}}]* %}
{% endfor %}

</div>
