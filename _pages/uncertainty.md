---
layout: page
permalink: /publications/uncertainty
title: Publications
description: <sup>*</sup>authors contributed equally. <br> <br>
  <a href=uncertainty style="color:var(--global-theme-color)">#Uncertainty Quantification</a>
  <a href=latent>#Latent Variable Models</a>
  <a href=dynamical>#Dynamical Systems</a>
  <a href=graph>#Graph Learning</a>
  <a href=sensor>#Sensors</a>
years: [2025, 2024, 2022, 2021, 2020, 2019, 2018]
nav: false
---

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}, uncertainty=true]*%}
{% endfor %}

</div>
