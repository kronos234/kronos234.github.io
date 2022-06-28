---
layout: publications
permalink: /publications/
title: Publications
description: 
years: [2022, 2021]
#yearsp: [2022]
nav: true
---

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
