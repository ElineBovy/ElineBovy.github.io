---
layout: page
permalink: /publications/
title: publications
description: 
us_count: [1]
# p_years: [2023]
t_years: [2023]
nav: true
nav_order: 1
scholar:
  last_name: [Bovy]
  first_name: [Eline]
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for c in page.us_count %}
  <h2 class="under_submission">Under submission</h2>
  {% bibliography -f under_submission -q @*[title={Imprecise Probabilities Meet Partial Observability: Game Semantics for Robust POMDPs}]%}
{% endfor %}

<!-- {%- for y in page.p_years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %} -->

{%- for y in page.t_years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f theses -q @*[year={{y}}]* %}
{% endfor %}

</div>