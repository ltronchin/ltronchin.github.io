---
layout: page
permalink: /publications/
title: publications
description: An up-to-date list is available on Google Scholar
years: [2020, 2021]
nav: true
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
