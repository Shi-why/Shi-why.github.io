---
layout: page
permalink: /publications/
title: Publications
description: Below is the list of my publications(published and under preparation) along with conference proceedings.
nav: true
years: [2023,2021,2018]
nav_order: 1
---
<!-- _pages/publications.md -->
<div class="publications">
  <!-- Add your legend here -->
  <div class="legend">
    <p><strong>Legend:</strong></p>
    <ul>
      <li><strong>O.Res:</strong> Original Research</li>
      <li><strong>Rev.:</strong> Review article</li>
      <li><strong>Conf.:</strong> Conference Proceeding</li>
      <!-- Add more abbreviations as needed -->
    </ul>
  </div>

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f {{ site.scholar.bibliography }} -q @*[year={{y}}]* %}

{% endfor %}

</div>
