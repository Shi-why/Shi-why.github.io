---
layout: page
permalink: /publications/
title: Publications.
description: Here is a list of my peer-reviewed publications and conference proceedings.
nav: true
nav_order: 1
---

<!-- _pages/publications.md -->
<div class="publications">

<h2>Papers</h2>
{% bibliography -f {{ site.scholar.bibliography }} -q @*[type=paper]* %}

<h2>Conference Proceedings</h2>
{% bibliography -f {{ site.scholar.bibliography }} -q @*[type=conference]* %}

</div>
