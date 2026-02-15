---
layout: home
title: Home
---

<!-- ====== CINEMATIC HERO ====== -->
<div class="hero">
  <div class="hero-video-wrap">
    <div id="hero-player"></div>
  </div>

  <!-- Mobile fallback: roti-on-flame when autoplay is blocked -->
  <img src="/assets/images/rotitales_roti_on_fire_logo.png" alt="Roti Tales" class="hero-mobile-poster" />

  <div class="hero-overlay"></div>

  <div class="hero-content">
    <img src="/assets/images/rotitales_roti_on_fire_logo.png" alt="Roti Tales" class="hero-logo" />
    <h1 class="hero-title">Roti Tales</h1>
    <p class="hero-tagline">Helping families eat healthier rotis</p>
    <a class="hero-cta" href="#reels" target="_self" id="hero-explore-btn">
      <span class="hero-cta-icon">&#9654;</span> Explore
    </a>
  </div>

  <!-- Sound toggle (SVG icons for cross-browser support) -->
  <button class="hero-sound-btn is-muted" id="hero-sound-btn" aria-label="Toggle sound">
    <svg class="sound-icon-muted" viewBox="0 0 24 24" width="22" height="22" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
      <path d="M11 5L6 9H2v6h4l5 4V5z"/>
      <line x1="23" y1="9" x2="17" y2="15"/>
      <line x1="17" y1="9" x2="23" y2="15"/>
    </svg>
    <svg class="sound-icon-on" viewBox="0 0 24 24" width="22" height="22" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
      <path d="M11 5L6 9H2v6h4l5 4V5z"/>
      <path d="M19.07 4.93a10 10 0 010 14.14"/>
      <path d="M15.54 8.46a5 5 0 010 7.07"/>
    </svg>
  </button>

  <div class="hero-scroll-hint" id="scroll-hint">
    <span>Scroll to explore</span>
    <div class="scroll-arrow"></div>
  </div>
</div>

<!-- ====== IMMERSIVE VIDEO FEED ====== -->
<div class="reel-feed" id="reels">

  <div class="reel-section reel-dark">
    <div class="reel-card">
      <div class="reel-video">
        <iframe src="https://www.youtube.com/embed/pPo5bd8tm2Y" allowfullscreen loading="lazy"></iframe>
      </div>
      <div class="reel-info">
        <h3 class="reel-title">The Healthier Roti</h3>
        <p class="reel-desc">Simple swaps to make your everyday roti more nutritious</p>
      </div>
    </div>
  </div>

  <div class="reel-section reel-warm">
    <div class="reel-card">
      <div class="reel-video">
        <iframe src="https://www.youtube.com/embed/oQPZyqFDFJc" allowfullscreen loading="lazy"></iframe>
      </div>
      <div class="reel-info">
        <h3 class="reel-title">Nutrition Made Simple</h3>
        <p class="reel-desc">Quick tips that pack a punch</p>
      </div>
    </div>
  </div>

  <!-- Connect card woven into the scroll -->
  <div class="reel-section reel-connect">
    <div class="reel-card connect-card">
      <img src="/assets/images/rotitales_roti_on_fire_logo.png" alt="Roti Tales" class="connect-logo" />
      <h3 class="connect-title">Join the Family</h3>
      <p class="connect-desc">Follow Roti Tales everywhere</p>
      <div class="connect-grid">
        <a href="https://www.youtube.com/@rotitales" class="connect-link">
          <img src="/assets/icons/youtube-clay.svg" alt="YouTube" />
          <span>YouTube</span>
        </a>
        <a href="https://instagram.com/rotitales" class="connect-link">
          <img src="/assets/icons/instagram-clay.svg" alt="Instagram" />
          <span>Instagram</span>
        </a>
        <a href="https://www.facebook.com/rotitales" class="connect-link">
          <img src="/assets/icons/facebook-clay.svg" alt="Facebook" />
          <span>Facebook</span>
        </a>
        <a href="https://www.linkedin.com/showcase/rotitales" class="connect-link">
          <img src="/assets/icons/linkedin-clay.svg" alt="LinkedIn" />
          <span>LinkedIn</span>
        </a>
      </div>
    </div>
  </div>

  <div class="reel-section reel-dark">
    <div class="reel-card">
      <div class="reel-video">
        <iframe src="https://www.youtube.com/embed/ef1_NUR4aig" allowfullscreen loading="lazy"></iframe>
      </div>
      <div class="reel-info">
        <h3 class="reel-title">Kitchen Vibes</h3>
        <p class="reel-desc">Feel-good roti making moments</p>
      </div>
    </div>
  </div>

</div>

<!-- ====== OUR MISSION (user loves this section) ====== -->
<div class="mission-section">
  <div class="mission-inner">
    <img src="/assets/images/Poshan_Logo_2Color-Flour.png" alt="Poshan" class="mission-logo" />
    <h2 class="mission-title">Healthier Rotis, Happier Families</h2>
    <p class="mission-text">Roti Tales is a Poshan initiative empowering families with simple ways to make everyday rotis more nutritious — one recipe at a time.</p>
    <a class="mission-cta" href="https://poshan.us">
      Learn about Poshan
      <span class="mission-cta-arrow">&#8594;</span>
    </a>
  </div>
</div>

<!-- ====== PLATFORM CHOOSER POPUP ====== -->
<div class="platform-overlay" id="platform-popup">
  <div class="platform-modal">
    <button class="platform-close" id="platform-close" type="button">&times;</button>
    <img src="/assets/images/rotitales_roti_on_fire_logo.png" alt="Roti Tales" class="platform-logo" />
    <h3 class="platform-heading">Find us on</h3>
    <div class="platform-grid">
      <a href="https://www.youtube.com/@rotitales" class="platform-option">
        <img src="/assets/icons/youtube-clay.svg" alt="YouTube" />
        <span>YouTube</span>
      </a>
      <a href="https://instagram.com/rotitales" class="platform-option">
        <img src="/assets/icons/instagram-clay.svg" alt="Instagram" />
        <span>Instagram</span>
      </a>
      <a href="https://www.facebook.com/rotitales" class="platform-option">
        <img src="/assets/icons/facebook-clay.svg" alt="Facebook" />
        <span>Facebook</span>
      </a>
      <a href="https://www.linkedin.com/showcase/rotitales" class="platform-option">
        <img src="/assets/icons/linkedin-clay.svg" alt="LinkedIn" />
        <span>LinkedIn</span>
      </a>
    </div>
  </div>
</div>

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

// Smooth scroll for Explore button
var exploreBtn = document.getElementById('hero-explore-btn');
if (exploreBtn) {
  exploreBtn.addEventListener('click', function(e) {
    e.preventDefault();
    var target = document.getElementById('reels');
    if (target) {
      target.scrollIntoView({ behavior: 'smooth' });
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

// Sound toggle for hero video
var soundBtn = document.getElementById('hero-sound-btn');
if (soundBtn) {
  soundBtn.addEventListener('click', function(e) {
    e.stopPropagation();
    if (!heroPlayer || !heroPlayer.isMuted) return;
    if (heroPlayer.isMuted()) {
      heroPlayer.unMute();
      soundBtn.classList.remove('is-muted');
    } else {
      heroPlayer.mute();
      soundBtn.classList.add('is-muted');
    }
  });
}

// Platform chooser popup
(function() {
  var popup = document.getElementById('platform-popup');
  var closeBtn = document.getElementById('platform-close');
  if (!popup) return;

  function openPopup() {
    popup.classList.add('is-open');
  }
  function closePopup() {
    popup.classList.remove('is-open');
  }

  // Any element with .platform-trigger opens the popup
  document.querySelectorAll('.platform-trigger').forEach(function(el) {
    el.addEventListener('click', function(e) {
      e.preventDefault();
      e.stopPropagation();
      openPopup();
    });
  });

  if (closeBtn) {
    closeBtn.addEventListener('click', closePopup);
  }

  // Close on backdrop click
  popup.addEventListener('click', function(e) {
    if (e.target === popup) {
      closePopup();
    }
  });

  // Close on Escape
  document.addEventListener('keydown', function(e) {
    if (e.key === 'Escape') closePopup();
  });
})();
</script>
