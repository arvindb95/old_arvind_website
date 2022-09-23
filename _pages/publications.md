---
layout: page
permalink: /publications/
title: Publications
description: A selected list of works that I have contributed to. Please look up my NASA ADS Page linked in the bottom for more publications. 
years: [2022,2021, 2017]
nav: true
icon: fa-book
order: 2
social: true
---

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
