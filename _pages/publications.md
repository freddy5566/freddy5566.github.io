---
layout: page
permalink: /publications/
title: Publications
description: <b>*</b> denotes equal contribution
years_preprint: [2024, 2023]
years: [2024, 2023, 2022, 2021]
nav: true
nav_order: 1
---
<!-- _pages/publications.md -->

<article>

<div class="publications">
<h2 class="publ-cat">Preprints</h2>
{%- for y in page.years_preprint %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f preprints -q @*[year={{y}}]* %}
{% endfor %}
</div>

<div class="publications">
<h2 class="publ-cat">Peer-reviewed Journal & Conference Papers</h2>
{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f jour_and_conf -q @*[year={{y}}]* %}
{% endfor %}
</div>
</article>