---
layout: page
permalink: /publications/by-category
title: Publications by Category
description: 
nav: false
nav_order: 92
categories:
  - preprint
  - conference
  - journal
---

<!-- _pages/publications.md -->

<!-- Bibsearch Feature -->

Please refer to [Google Scholar](https://scholar.google.com/citations?user=RPmhP24AAAAJ&hl=en&oi=ao) page for the up-to-date list.

<!-- {% include bib_search.liquid %} -->
<div class="publications">
  {% for c in page.categories %}
    <h2 class="category">{{c}}</h2>
    {% bibliography -q @*[category={{c}}]* %}
  {% endfor %}
</div>