---
layout: page
permalink: /publications/
title: Publications
description: 
years: [2022]
nav: true
nav_order: 2
---
<!-- _pages/publications.md -->
<div class="publications">

<h2>Journals</h2>
{% bibliography -f papers -q @*[year=forthcoming]* %}

{%- for y in page.years %}
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

<h2>Technical Papers</h2>
{%- for y in page.years %}
  {% bibliography -f technical -q @*[year={{y}}]* %}
{% endfor %}

</div>
