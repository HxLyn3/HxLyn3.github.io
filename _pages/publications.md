---
layout: page
permalink: /publications/
title: Publications
description: my publications sorted by year
years: [2025, 2024, 2023]
nav: true
nav_order: 2
---
\* indicates equal contributioncon.

<!-- _pages/publications.md -->

<!-- Bibsearch Feature -->

{% include bib_search.liquid %}

#### Papers

<div class="publications">

{% for y in page.years %}

<div>{{y}}</div>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
