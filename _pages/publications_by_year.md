---
layout: page
permalink: /publications/by-year
title: Publications by Year
description: 
nav: false
nav_order: 91
years:
  - 2024
  - 2023
  - 2022
  - 2021
---

<!-- _pages/publications.md -->

<!-- Bibsearch Feature -->

Please refer to [Google Scholar](https://scholar.google.com/citations?user=RPmhP24AAAAJ&hl=en&oi=ao) page for the up-to-date list.

<!-- {% include bib_search.liquid %} -->
<div class="publications">
  {% for y in page.years %}
    {% bibliography -q @*[year={{y}}]* %}
  {% endfor %}
</div>