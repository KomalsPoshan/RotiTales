---
layout: default
title: Education
permalink: /education.html
---

<h1 style="header">Educational Videos</h1>

<div class="shorts-carousel">
  <div class="carousel-slide center">
    <iframe id="current-video" allowfullscreen></iframe>
  </div>
  <div class="carousel-slide">
    <iframe id="prev-video" allowfullscreen></iframe>
    <div class="overlay-div" onclick="moveCarousel(-1)"></div>
  </div>
  <div class="carousel-slide">
    <iframe id="next-video" allowfullscreen></iframe>
    <div class="overlay-div" onclick="moveCarousel(1)"></div>
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
  const prev = document.getElementById('prev-video');
  const curr = document.getElementById('current-video');
  const next = document.getElementById('next-video');
  const total = videoIds.length;

  // Determine which element is moving to center
  const target = direction > 0 ? next : prev;

  // Add the transitionend listener BEFORE triggering transforms
  target.addEventListener('transitionend', function handler() {
    // Update current index
    currentIndex = (currentIndex + direction + total) % total;

    // Reset transforms and update video sources
    updateIframes();

    // Clean up the handler
    target.removeEventListener('transitionend', handler);
  });

  // Trigger animated transform
  if (direction > 0) {
    // Move next to center
    curr.style.transform = 'translateX(-60%) scale(0.9)';
    next.style.transform = 'translateX(0) scale(1)';
    prev.style.transform = 'translateX(-120%) scale(0.9)';
  } else {
    // Move prev to center
    curr.style.transform = 'translateX(60%) scale(0.9)';
    prev.style.transform = 'translateX(0) scale(1)';
    next.style.transform = 'translateX(120%) scale(0.9)';
  }
}


  document.addEventListener('DOMContentLoaded', updateIframes);
</script>
