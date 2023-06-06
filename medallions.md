---
layout: page
title: Medallions
subtitle: 
---
<div class="gallery">
  {% for i in (1..7) %}
    <img src="/assets/img/medallion_{{ i }}.png" alt="Bracket {{ i }}">
  {% endfor %}
</div>