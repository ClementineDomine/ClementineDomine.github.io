---
layout: page
permalink: /publications/
title: publications
description: (*) denotes equal contribution.
years: [2022,2023]
nav: "publications"
header:
  teaser: /assets/img/teaser_clem Small.jpeg

---
<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
