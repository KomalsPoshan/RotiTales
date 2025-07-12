---
layout: default
title: Education
permalink: /education.html
---

<h1 style="header">Educational Videos</h1>

<div class="shorts-carousel">
  <div class="carousel-slide">
    <iframe allowfullscreen></iframe>
  </div>
  <div class="carousel-slide">
    <iframe allowfullscreen></iframe>
    <div class="overlay-div" onclick="moveCarousel(-1)"></div>
  </div>
  <div class="carousel-slide">
    <iframe allowfullscreen></iframe>
  </div>
  <div class="carousel-slide">
    <iframe allowfullscreen></iframe>
    <div class="overlay-div" onclick="moveCarousel(1)"></div>
  </div>
  <div class="carousel-slide">
    <iframe allowfullscreen></iframe>
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

  let currVideoIndex = 0;

  let items = document.querySelectorAll('.carousel-slide');
  let videoItems = document.querySelectorAll('.carousel-slide iframe');

  function loadElements() {
    let active = 2;
    items[active].style.transform = 'none';
    items[active].style.zIndex = 1;
    items[active].style.filter = 'none';
    items[active].style.opacity = 1;

    var stt = 0;
    for (var i = active + 1; i < items.length; i++) {
      stt++;
      items[i].style.transform = 'translateX(${120*stt}px) scale(${1 - 0.2*stt}) rotateY(-1 deg)';
      items[i].style.zIndex = -stt;
      items[i].style.filter = 'blue(5px)';
      items[i].style.opacity = stt > 1 ? 0 : 0.6;      
    }

    stt = 0;
    for (var i = active - 1; i >= 0; i--) {
      stt++;
      items[i].style.transform = 'translateX(${-120*stt}px) scale(${1 - 0.2*stt}) rotateY(1 deg)';
      items[i].style.zIndex = -stt;
      items[i].style.filter = 'blue(5px)';
      items[i].style.opacity = stt > 1 ? 0 : 0.6;      
    }
  }

  function loadVideos() {
    let active = 2;
    videoItems[active].src = videoIds[currVideoIndex];
    for (var i = active + 1; i < videoItems.length; i++) {
      index = (currVideoIndex + videoIds.length - 1)%videoIds.length;
      videoItems[i].src = videoIds[index];
    }
    for (var i = active - 1; i >= 0; i--) {
      index = (currVideoIndex + 1)%videoIds.length;
      videoItems[i].src = videoIds[index];
    }
  }

  function loadAll() {
  loadVideos();
  loadElements();
  }

function moveCarousel(direction) {
  currVideoIndex = (currVideoIndex + videoIds.length + direction)%videoIds.length;
  loadAll();
}

document.addEventListener('DOMContentLoaded', loadAll);
</script>
