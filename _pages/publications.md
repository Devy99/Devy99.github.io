---
layout: page
permalink: /publications/
title: publications
nav: true
nav_order: 1
years: [2025]
---

<h1>Publications</h1>
{% for y in page.years %}
  <div class="row m-0 p-0" style="border-bottom: 1px solid #ddd;">
    <div class="col-sm-11 p-0">
      {% bibliography -f papers -q @*[year={{y}}]* %}
    </div>
    <div class="col-sm-1 align-self-end mt-2 p-0 pr-1">
      <h3 class="bibliography-year">{{y}}</h3>
    </div>
  </div>
{% endfor %}