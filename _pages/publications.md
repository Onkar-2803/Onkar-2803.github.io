---
layout: page
permalink: /publications/
title: Publications
years: [2024, 2023, 2022, 2021]
nav: true
nav_order: 2
---
Publications in reversed chronological order. My <a href="https://scholar.google.com/citationsuser=19OfMHYAAAAJ&hl=en&authuser=1"> Google Scholar </a> is more likely to be up to date.

<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
