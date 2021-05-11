---
layout: page
permalink: /publications/
title: publications
description: Find more information on <a href='https://scholar.google.com/citations?user=zyd3R2X4AAAAJ&hl=en'>Google scholar</a>. 
years: [2021, 2020, 2019, 2018, 2017, 2016, 2015, 2014, 2013]
nav: true
---

<div class="publications">

{% for y in page.years %}
  <!-- <h2 class="year">{{y}}</h2> -->
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>