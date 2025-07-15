---
layout: default
permalink: /publications/
# type: article
title: Publications
description: Publications by yearly categories in reversed chronological order.
years: [2025, 2024]
publication_photo: http://via.placeholder.com/200
---

<div class="grid-container">
    <h1 class="separator-center font-bold margin-top-3">{{ page.title }}</h1>
</div>

<div class="grid-container">
  {% for y in page.years %}
    <div class="margin-bottom-3">
      <h3 class="separator-left margin-bottom-2">{{y}}</h3>
      {% bibliography -f biblio -q @*[year={{y}}]* %}
    </div>
  {% endfor %}
</div>

