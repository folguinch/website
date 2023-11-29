---
layout: page
title: DIHCA survey
description: A close-up view into the formation of high-mass stars with ALMA.
img: assets/img/dihca_logo.png
importance: 1
category: research
years_dihca: [2023, 2022, 2021]
years_other: [2023]
---

## Highlights

### Spiral accretion in G336.01-0.82

We found streams of gas bringing fresh material to the disk surrounding a high-mass protostar.
The interactive figure shows that the kinematics of this gas can be explained with models including rotation and gravitational collapse.
The gas seems to be accumulating in the outskirts of the disk and in the future can be accreted or induce fragmentation, allowing the formation of stellar companions.

{% include x3d.html file="assets/x3d/interactive_figure_final.x3d" name="g336" %}

## Publications

<div class="publications">
{%- for y in page.years_dihca %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f dihca -q @*[year={{y}}]* %}
{% endfor %}
</div>

#### Other publications using DIHCA data

<div class="publications">
{%- for y in page.years_other %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f dihca_other -q @*[year={{y}}]* %}
{% endfor %}
</div>
