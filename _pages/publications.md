---
layout: page
permalink: /publications/
title: publications
description: 
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

<!-- {%- for y in page.p_years %} -->
<h2 class="under_submission">Under submission</h2>
  {% bibliography -f under_submission%}
<!-- {% endfor %} -->

<!-- {%- for y in page.p_years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %} -->

{%- for y in page.t_years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f theses -q @*[year={{y}}]* %}
{% endfor %}

</div>