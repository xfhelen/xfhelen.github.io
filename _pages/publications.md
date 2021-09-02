---
layout: page
permalink: /publications/
title: Publications
description: Publications by categories in reversed chronological order.
years: [2021, 2020, 2019, 2018, 2017, 2016]
nav: true
---

<div class="publications">
  <p>Conference Papers</p>
{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f conf_papers -q @*[year={{y}}]* %}
{% endfor %}

<p>Journal Papers</p>
{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f journal_papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
