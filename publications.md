---
layout: default
permalink: /publications/
# type: article
title: Publications
description: Publications by yearly categories in reversed chronological order.
years: [2025, 2024, 2023]
publication_photo: http://via.placeholder.com/200
---

<div class="grid-container">
    <h1 class="separator-center font-bold margin-top-3">{{ page.title }}</h1>
    <p class="text-center margin-bottom-3" style="background-color:#f9f9f9; padding:10px; border-left:4px solid #ccc; font-style:italic;">
      Please refer to <a href="https://scholar.google.com/citations?user=s1IAWfgAAAAJ&hl=en" target="_blank" style="text-decoration: underline;">here</a> for the full publication list.
    </p>
</div>

<div class="grid-container">
  {% for y in page.years %}
    <div class="margin-bottom-3">
      <h3 class="separator-left margin-bottom-2">{{ y }}</h3>
      {% bibliography -f biblio --query @*[year={{y}}]* --sort none %}
    </div>
  {% endfor %}
</div>

