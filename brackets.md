---
layout: page
title: Brackets
subtitle: 
---
<!---<div class="gallery">
  {% for i in (1..6) %}
    <img src="/assets/img/bracket_{{ i }}.png" alt="Bracket {{ i }}">
  {% endfor %}
</div>--->

<div class="banner-container">
  <div class="banner">
    <img src="/assets/img/bracket_1.png" alt="Bracket 1">
    <img src="/assets/img/bracket_2.png" alt="Bracket 2">
    <img src="/assets/img/bracket_3.png" alt="Bracket 3">
    <img src="/assets/img/bracket_4.png" alt="Bracket 4">
    <img src="/assets/img/bracket_5.png" alt="Bracket 5">
    <img src="/assets/img/bracket_6.png" alt="Bracket 6">
  </div>
</div>

{% raw %}
<script>
window.addEventListener('load', function() {
  adjustBannerWidth();
});

window.addEventListener('resize', function() {
  adjustBannerWidth();
});

function adjustBannerWidth() {
  var banner = document.querySelector('.banner');
  var images = banner.querySelectorAll('img');
  var bannerWidth = banner.offsetWidth;

  for (var i = 0; i < images.length; i++) {
    images[i].style.width = bannerWidth + 'px';
  }
}
</script>
{% endraw %}
