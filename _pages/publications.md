---
layout: page
permalink: /publications/
title: Publications
description: Here you can find a list of publications related to AI auditing that are output of the aiaudit.org network or its contributors
years: [2021, 2020]
nav: true
nav-order: b
---
# Standardization
<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f standards -q @*[year={{y}}]* %}
{% endfor %}

</div>

# Conferences and journals
<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>

# Preprints
<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f preprints -q @*[year={{y}}]* %}
{% endfor %}

</div>
