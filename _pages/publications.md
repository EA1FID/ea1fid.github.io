---
layout: page
permalink: /store/
title: Store
description: In our eBay store, you can find all the materials you need to build any of our antennae!
years: [VHF, UHF]
nav: true
---

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
