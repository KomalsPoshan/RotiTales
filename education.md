---
layout: default
title: Education
permalink: /education.html
---

<h1 style="text-align: center; margin-top: 2rem;">Educational Videos</h1>

<div class="shorts-carousel">
  <div class="carousel-track">
    <div class="carousel-slide">
      <iframe id="prevVideo" allowfullscreen />
      <div class="overlayDiv" onclick="moveCarousel(-1)"/>
    </div>
    <div class="carousel-slide center">
      <iframe id="currentVideo" allowfullscreen />
    </div>
    <div class="carousel-slide">
      <iframe id="nextVideo" allowfullscreen />
      <div class="overlayDiv" onclick="moveCarousel(1)"/>
    </div>
  </div>

  <button class="carousel-nav next" onclick="moveCarousel(1)">&#10095;</button>
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

    document.getElementById('prevVideo').src = `https://www.youtube.com/embed/${videoIds[prev]}`;
    document.getElementById('currentVideo').src = `https://www.youtube.com/embed/${videoIds[currentIndex]}`;
    document.getElementById('nextVideo').src = `https://www.youtube.com/embed/${videoIds[next]}`;
  }

  function moveCarousel(direction) {
    const total = videoIds.length;
    currentIndex = (currentIndex + direction + total) % total;
    updateIframes();
  }

  document.addEventListener('DOMContentLoaded', updateIframes);
</script>
