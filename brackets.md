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

window.addEventListener('load', function() {
  adjustBannerWidth();
});
