---
layout: page
permalink: /publications/
title: Publications.
description: Here is a list of my peer-reviewed publications and conference proceedings.
nav: true
years: [2023,2021]
nav_order: 1
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  <h3>Publications</h3>
  {% bibliography -f {{ site.scholar.bibliography }} -q @*[year={{y}}]* %}

{% endfor %}

</div>
