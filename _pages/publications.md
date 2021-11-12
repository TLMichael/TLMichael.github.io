---
layout: page
permalink: /publications/
title: Publications
years: [2021, 2020]
nav: true
---

<div class="publications">

<!-- (* Equal contribution; † Corresponding author) -->
(* Equal contribution)

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
