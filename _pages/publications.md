---
layout: page
permalink: /publications/
title: Publications
description: List of publications
years_first: [2022, 2021, 2020, 2015]
years_cols: [2023, 2022, 2021, 2019, 2017, 2015, 2014]
nav: true
nav_order: 2
---

<!-- _pages/publications.md -->
<div class="publications">

<h3> First author </h3>

{%- for y in page.years_first %}

  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

<h3> Collaborations </h3>

{%- for y in page.years_cols %}

  <h2 class="year">{{y}}</h2>
  {% bibliography -f collaborations -q @*[year={{y}}]* %}
{% endfor %}

</div>
