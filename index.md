---
layout: home
title: Home
---

<!-- ====== CINEMATIC HERO ====== -->
<div class="hero">
  <div class="hero-video-wrap">
    <div id="hero-player"></div>
  </div>

  <div class="hero-overlay"></div>

  <div class="hero-content">
    <img src="/assets/images/Roti Tales - Logo.png" alt="Roti Tales" class="hero-logo" />
    <h1 class="hero-title">Roti Tales</h1>
    <p class="hero-tagline">Helping families eat healthier rotis</p>
    <a class="hero-cta" href="https://www.youtube.com/watch?v=pPo5bd8tm2Y" id="hero-watch-btn">
      <span class="hero-cta-icon">&#9654;</span> Watch Now
    </a>
  </div>

  <div class="hero-scroll-hint" id="scroll-hint">
    <span>Scroll to explore</span>
    <div class="scroll-arrow"></div>
  </div>
</div>

<!-- ====== WATCH & LEARN ====== -->
<div class="featured-section">
  <h2 class="section-title">Watch & Learn</h2>
  <p class="section-subtitle">Quick videos on how to make healthier rotis for your family</p>

  <div class="video-row">
    <div class="video-card">
      <iframe src="https://www.youtube.com/embed/pPo5bd8tm2Y" allowfullscreen loading="lazy"></iframe>
    </div>
    <div class="video-card">
      <iframe src="https://www.youtube.com/embed/oQPZyqFDFJc" allowfullscreen loading="lazy"></iframe>
    </div>
    <div class="video-card">
      <iframe src="https://www.youtube.com/embed/ef1_NUR4aig" allowfullscreen loading="lazy"></iframe>
    </div>
  </div>

  <a class="cta-button" href="https://www.youtube.com/playlist?list=PLca7YZGvJBnX8Q_pfbBsePRChDufQQVE2">
    <img src="/assets/icons/youtube-clay.svg" alt="YouTube" />
    <img class="cta-button-hover" src="/assets/icons/youtube-flour.svg" alt="YouTube" />
    <span>Watch the full playlist</span>
    <img class="arrow" src="/assets/icons/arrow-clay.svg" alt="Arrow" />
    <img class="arrow cta-button-hover" src="/assets/icons/arrow-flour.svg" alt="Arrow" />
  </a>
</div>

<!-- ====== FROM OUR INSTAGRAM ====== -->
<div class="featured-section">
  <h2 class="section-title">From Our Instagram</h2>
  <p class="section-subtitle">Tips, reels & behind-the-scenes</p>

  <div class="instagram-row">
    <blockquote class="instagram-media" data-instgrm-captioned data-instgrm-permalink="https://www.instagram.com/reel/DFuftgwJPbM/" data-instgrm-version="14">
      <a href="https://www.instagram.com/reel/DFuftgwJPbM/"></a>
    </blockquote>

    <blockquote class="instagram-media" data-instgrm-captioned data-instgrm-permalink="https://www.instagram.com/reel/DFYTsZbpsaC/" data-instgrm-version="14">
      <a href="https://www.instagram.com/reel/DFYTsZbpsaC/"></a>
    </blockquote>
  </div>

  <a class="cta-button" href="https://instagram.com/rotitales">
    <img src="/assets/icons/instagram-clay.svg" alt="Instagram" />
    <img class="cta-button-hover" src="/assets/icons/instagram-flour.svg" alt="Instagram" />
    <span>Follow us on Instagram</span>
    <img class="arrow" src="/assets/icons/arrow-clay.svg" alt="Arrow" />
    <img class="arrow cta-button-hover" src="/assets/icons/arrow-flour.svg" alt="Arrow" />
  </a>
</div>

<!-- ====== CONNECT WITH US ====== -->
<div class="featured-section">
  <h2 class="section-title">Connect With Us</h2>

  <div class="social-links">
    <a class="social-button" href="https://www.facebook.com/rotitales">
      <img src="/assets/icons/facebook-clay.svg" alt="Facebook logo" />
      <img class="social-button-hover" src="/assets/icons/facebook-flour.svg" alt="Facebook logo"/>
      <div class="social-label">Facebook</div>
      <img class="arrow" src="/assets/icons/arrow-clay.svg" alt="Arrow icon" />
      <img class="arrow social-button-hover" src="/assets/icons/arrow-flour.svg" alt="Arrow icon"/>
    </a>

    <a class="social-button" href="https://instagram.com/rotitales">
      <img src="/assets/icons/instagram-clay.svg" alt="Instagram logo" />
      <img class="social-button-hover" src="/assets/icons/instagram-flour.svg" alt="Instagram logo"/>
      <div class="social-label">Instagram</div>
      <img class="arrow" src="/assets/icons/arrow-clay.svg" alt="Arrow icon" />
      <img class="arrow social-button-hover" src="/assets/icons/arrow-flour.svg" alt="Arrow icon"/>
    </a>

    <a class="social-button" href="https://www.linkedin.com/showcase/rotitales">
      <img src="/assets/icons/linkedin-clay.svg" alt="LinkedIn logo" />
      <img class="social-button-hover" src="/assets/icons/linkedin-flour.svg" alt="LinkedIn logo"/>
      <div class="social-label">LinkedIn</div>
      <img class="arrow" src="/assets/icons/arrow-clay.svg" alt="Arrow icon" />
      <img class="arrow social-button-hover" src="/assets/icons/arrow-flour.svg" alt="Arrow icon"/>
    </a>

    <a class="social-button" href="https://www.youtube.com/@rotitales">
      <img src="/assets/icons/youtube-clay.svg" alt="YouTube logo" />
      <img class="social-button-hover" src="/assets/icons/youtube-flour.svg" alt="YouTube logo"/>
      <div class="social-label">YouTube</div>
      <img class="arrow" src="/assets/icons/arrow-clay.svg" alt="Arrow icon" />
      <img class="arrow social-button-hover" src="/assets/icons/arrow-flour.svg" alt="Arrow icon"/>
    </a>
  </div>
</div>

<script async src="//www.instagram.com/embed.js"></script>

<!-- YouTube IFrame API for background hero video -->
<script>
var tag = document.createElement('script');
tag.src = "https://www.youtube.com/iframe_api";
var firstScriptTag = document.getElementsByTagName('script')[0];
firstScriptTag.parentNode.insertBefore(tag, firstScriptTag);

var heroPlayer;
function onYouTubeIframeAPIReady() {
  heroPlayer = new YT.Player('hero-player', {
    videoId: 'pPo5bd8tm2Y',
    playerVars: {
      autoplay: 1,
      mute: 1,
      controls: 0,
      showinfo: 0,
      rel: 0,
      loop: 1,
      playlist: 'pPo5bd8tm2Y',
      modestbranding: 1,
      iv_load_policy: 3,
      disablekb: 1,
      fs: 0,
      playsinline: 1
    },
    events: {
      onReady: function(e) {
        e.target.playVideo();
      },
      onStateChange: function(e) {
        if (e.data === YT.PlayerState.ENDED) {
          heroPlayer.playVideo();
        }
      }
    }
  });
}

// Fade out scroll hint on scroll
window.addEventListener('scroll', function() {
  var hint = document.getElementById('scroll-hint');
  if (hint) {
    hint.style.opacity = window.scrollY > 80 ? '0' : '1';
  }
});
</script>
