---
layout: page
permalink: /publications/
title: publications
description: publications by categories in reversed chronological order.
years: [2019, 2020, 2021, 2022, 2023]
nav: true
---

<div class="publications">

{% for y in page.years reversed %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
