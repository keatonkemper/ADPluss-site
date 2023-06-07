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
    {% for i in (1..6) %}
      <img src="/assets/img/bracket_{{ i }}.png" alt="Bracket {{ i }}">
    {% endfor %}
  </div>
</div>

{% raw %}
<script>
window.addEventListener('load', function() {
  startBannerScroll();
});

function startBannerScroll() {
  var banner = document.querySelector('.banner');
  var bannerWidth = banner.offsetWidth;
  var scrollDistance = banner.scrollWidth - bannerWidth;
  var currentPosition = 0;

  setInterval(function() {
    currentPosition += 1;
    if (currentPosition > scrollDistance) {
      currentPosition = 0;
    }
    banner.style.transform = 'translateX(-' + currentPosition + 'px)';
  }, 10);
}
</script>
{% endraw %}
