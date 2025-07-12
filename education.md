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
    videoItems[active].style.pointerEvents = 'none';
    videoItems[active].style.cursor = 'pointer';

    var stt = 0;
    for (var i = active + 1; i < items.length; i++) {
      stt++;
      x = 120*stt;
      scale = 1 - 0.1*stt;
      items[i].style.transform = "translateX(" + x + "px) scale(" + scale + ')';
      items[i].style.zIndex = -stt;
      items[i].style.filter = 'blue(5px)';
      items[i].style.opacity = stt > 1 ? 0 : 0.6;      
      videoItems[i].style.pointerEvents = 'none';
    }

    stt = 0;
    for (var i = active - 1; i >= 0; i--) {
      stt++;
      x = -120*stt;
      scale = 1 - 0.1*stt;
      items[i].style.transform = "translateX(" + x + "px) scale(" + scale + ')';
      items[i].style.zIndex = -stt;
      items[i].style.filter = 'blue(5px)';
      items[i].style.opacity = stt > 1 ? 0 : 0.6;      
      videoItems[i].style.pointerEvents = 'none';
    }
  }

  function getUrl(videoIdIndex) {
    var videoId = videoIds[videoIdIndex];
    return "https://www.youtube.com/embed/" + videoId;
  }

  function loadVideos() {
    let active = 2;
    videoItems[active].src = getUrl(currVideoIndex);
    for (var i = active + 1; i < videoItems.length; i++) {
      index = (currVideoIndex + videoIds.length - 1)%videoIds.length;
      videoItems[i].src = getUrl(index);
    }
    for (var i = active - 1; i >= 0; i--) {
      index = (currVideoIndex + 1)%videoIds.length;
      videoItems[i].src = getUrl(index);
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
