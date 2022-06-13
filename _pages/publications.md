---
layout: page
permalink: /publications/
title: Publications
description: 
years: []
nav: true
nav_order: 2
---
<!-- _pages/publications.md -->
<div class="publications">

<h2 class="year">forthcoming</h2>
{% bibliography -f papers -q @*[year=forthcoming]* %}

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
