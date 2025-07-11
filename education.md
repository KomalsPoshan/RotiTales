---
layout: default
title: Education
permalink: /education.html
---

<h1 style="header">Educational Videos</h1>

<div class="shorts-carousel">
  <div class="carousel-slide">
    <iframe id="prev-video" allowfullscreen></iframe>
    <div class="overlay-div" onclick="moveCarousel(-1)"></div>
  </div>
  <div class="carousel-slide">
    <iframe id="next-video" allowfullscreen></iframe>
    <div class="overlay-div" onclick="moveCarousel(1)"></div>
  </div>
  <div class="carousel-slide center">
    <iframe id="current-video" allowfullscreen></iframe>
  </div>
</div>

<script>
  const videoIds = [
    "GI2yXCMt6qY",
    "mxb1spl3uEQ",
    "UmADIP7Eneo",
    "bKHeCYNw9bY",
    "5VvCXdIaX_k",
    "ef1_NUR4aig",
    "oQPZyqFDFJc",
    "pPo5bd8tm2Y"
  ];

  let currentIndex = 0;

  function updateIframes() {
    const total = videoIds.length;
    const prev = (currentIndex - 1 + total) % total;
    const next = (currentIndex + 1) % total;

    document.getElementById('prev-video').src = `https://www.youtube.com/embed/${videoIds[prev]}`;
    document.getElementById('current-video').src = `https://www.youtube.com/embed/${videoIds[currentIndex]}`;
    document.getElementById('next-video').src = `https://www.youtube.com/embed/${videoIds[next]}`;
  }

  function moveCarousel(direction) {
    const total = videoIds.length;
    currentIndex = (currentIndex + direction + total) % total;
    updateIframes();
  }

  document.addEventListener('DOMContentLoaded', updateIframes);
</script>
