---
layout: home
title: Home
---

<!-- ====== FULL-SCREEN VIDEO CAROUSEL ====== -->
<div class="hero-carousel">

  <!-- Branding — top left, logo + title inline -->
  <div class="hero-brand">
    <img src="/assets/images/rotitales_roti_on_fire_logo.png" alt="Roti Tales" class="hero-brand-logo" />
    <div class="hero-brand-text">
      <h1 class="hero-brand-title">Roti Tales</h1>
      <p class="hero-brand-sub">Helping families eat healthier rotis</p>
    </div>
  </div>

  <!-- Carousel viewport -->
  <div class="carousel-viewport">
    <div class="carousel-track" id="carousel-track">

      <!-- Slide 1: API-controlled autoplay video -->
      <div class="carousel-slide is-active" data-index="0">
        <div class="slide-card">
          <div class="slide-video slide-video-api">
            <div id="hero-player"></div>
          </div>
          <button class="card-mute is-muted" id="ctrl-mute" aria-label="Toggle sound">
            <svg class="sound-icon-muted" viewBox="0 0 24 24" width="18" height="18" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
              <path d="M11 5L6 9H2v6h4l5 4V5z"/>
              <line x1="23" y1="9" x2="17" y2="15"/>
              <line x1="17" y1="9" x2="23" y2="15"/>
            </svg>
            <svg class="sound-icon-on" viewBox="0 0 24 24" width="18" height="18" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
              <path d="M11 5L6 9H2v6h4l5 4V5z"/>
              <path d="M19.07 4.93a10 10 0 010 14.14"/>
              <path d="M15.54 8.46a5 5 0 010 7.07"/>
            </svg>
          </button>
          <div class="slide-label">
            <h3>Are all carbs bad?</h3>
            <p>Simple swaps for more nutritious rotis</p>
          </div>
        </div>
      </div>

      <!-- Slide 2 -->
      <div class="carousel-slide" data-index="1">
        <div class="slide-card">
          <div class="slide-video">
            <iframe src="https://www.youtube.com/embed/oQPZyqFDFJc" allowfullscreen loading="lazy"></iframe>
          </div>
          <div class="slide-label">
            <h3>Nutrition Made Simple</h3>
            <p>Quick tips that pack a punch</p>
          </div>
        </div>
      </div>

      <!-- Slide 3: Connect card -->
      <div class="carousel-slide" data-index="2">
        <div class="slide-card">
          <div class="slide-connect">
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
      </div>

      <!-- Slide 4 -->
      <div class="carousel-slide" data-index="3">
        <div class="slide-card">
          <div class="slide-video">
            <iframe src="https://www.youtube.com/embed/ef1_NUR4aig" allowfullscreen loading="lazy"></iframe>
          </div>
          <div class="slide-label">
            <h3>Kitchen Vibes</h3>
            <p>Feel-good roti making moments</p>
          </div>
        </div>
      </div>

    </div>
  </div>

  <!-- Controls — bottom center -->
  <div class="hero-controls">
    <button class="ctrl-btn" id="ctrl-prev" aria-label="Previous">
      <svg viewBox="0 0 24 24" width="20" height="20" fill="none" stroke="currentColor" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round"><polyline points="15 18 9 12 15 6"/></svg>
    </button>

    <button class="ctrl-btn ctrl-playpause" id="ctrl-playpause" aria-label="Play/Pause">
      <svg class="pp-pause" viewBox="0 0 24 24" width="18" height="18" fill="currentColor"><rect x="6" y="4" width="4" height="16"/><rect x="14" y="4" width="4" height="16"/></svg>
      <svg class="pp-play" viewBox="0 0 24 24" width="18" height="18" fill="currentColor"><polygon points="5,3 19,12 5,21"/></svg>
    </button>

    <div class="hero-dots" id="hero-dots">
      <span class="dot active" data-slide="0"></span>
      <span class="dot" data-slide="1"></span>
      <span class="dot" data-slide="2"></span>
      <span class="dot" data-slide="3"></span>
    </div>

    <button class="ctrl-btn" id="ctrl-next" aria-label="Next">
      <svg viewBox="0 0 24 24" width="20" height="20" fill="none" stroke="currentColor" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round"><polyline points="9 18 15 12 9 6"/></svg>
    </button>
  </div>

</div>

<!-- ====== OUR MISSION ====== -->
<div class="mission-section">
  <div class="mission-inner">
    <img src="/assets/images/Poshan_Logo_2Color-Flour.png" alt="Poshan" class="mission-logo" />
    <h2 class="mission-title">Healthier Rotis, Happier Families</h2>
    <p class="mission-text">Roti Tales is a Poshan initiative empowering families with simple ways to make everyday rotis more nutritious — one recipe at a time.</p>
    <a class="mission-cta platform-trigger" href="#">
      Follow RotiTales
      <span class="mission-cta-arrow">&#8594;</span>
    </a>
  </div>
</div>

<!-- ====== PLATFORM CHOOSER POPUP ====== -->
<div class="platform-overlay" id="platform-popup">
  <div class="platform-modal">
    <button class="platform-close" id="platform-close" type="button">&times;</button>
    <div class="platform-header">
      <img src="/assets/images/rotitales_roti_on_fire_logo.png" alt="Roti Tales" class="platform-logo" />
      <div class="platform-brand">
        <h3 class="platform-heading">Roti Tales</h3>
        <p class="platform-tagline">Healthier rotis, happier families</p>
      </div>
    </div>
    <p class="platform-cta-text">Follow us &mdash; never miss a recipe!</p>
    <div class="platform-row">
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

<!-- ====== FOLLOW NUDGE (appears after 5s) ====== -->
<div class="follow-nudge" id="follow-nudge">
  <svg class="follow-nudge-hand" viewBox="0 0 24 24" width="28" height="28" fill="none" stroke="currentColor" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round">
    <path d="M18 11V6a2 2 0 00-4 0v1"/>
    <path d="M14 10V4a2 2 0 00-4 0v6"/>
    <path d="M10 10.5V6a2 2 0 00-4 0v8"/>
    <path d="M18 11a2 2 0 014 0v3a8 8 0 01-8 8h-2c-2.5 0-4.5-1-6.2-2.8L3 16.4a2 2 0 013-2.6l.6.6"/>
  </svg>
  <span class="follow-nudge-text">Follow us!</span>
</div>

<!-- YouTube IFrame API -->
<script>
var tag = document.createElement('script');
tag.src = "https://www.youtube.com/iframe_api";
var firstScriptTag = document.getElementsByTagName('script')[0];
firstScriptTag.parentNode.insertBefore(tag, firstScriptTag);

var heroPlayer;
var isPlaying = true;

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
      onReady: function(e) { e.target.playVideo(); },
      onStateChange: function(e) {
        if (e.data === YT.PlayerState.ENDED) heroPlayer.playVideo();
      }
    }
  });
}

// ===== Carousel =====
(function() {
  var track = document.getElementById('carousel-track');
  var dots = document.querySelectorAll('#hero-dots .dot');
  var totalSlides = dots.length;
  var current = 0;

  var slides = document.querySelectorAll('.carousel-slide');

  function goTo(idx) {
    if (idx < 0) idx = totalSlides - 1;
    if (idx >= totalSlides) idx = 0;
    current = idx;
    var slidePct = parseFloat(getComputedStyle(document.documentElement).getPropertyValue('--slide-pct')) || 70;
    var offset = (100 - slidePct) / 2;
    track.style.transform = 'translateX(' + (offset - current * slidePct) + '%)';
    dots.forEach(function(d, i) {
      d.classList.toggle('active', i === current);
    });
    slides.forEach(function(s, i) {
      s.classList.toggle('is-active', i === current);
    });
    // Pause hero player when not on slide 0, resume when back
    if (heroPlayer && heroPlayer.pauseVideo) {
      if (current === 0 && isPlaying) {
        heroPlayer.playVideo();
      } else {
        heroPlayer.pauseVideo();
      }
    }
  }

  document.getElementById('ctrl-prev').addEventListener('click', function() { goTo(current - 1); });
  document.getElementById('ctrl-next').addEventListener('click', function() { goTo(current + 1); });

  // Dot click navigation
  dots.forEach(function(dot) {
    dot.addEventListener('click', function() {
      goTo(parseInt(this.getAttribute('data-slide')));
    });
  });

  // Swipe support
  var startX = 0;
  var viewport = document.querySelector('.carousel-viewport');
  viewport.addEventListener('touchstart', function(e) { startX = e.touches[0].clientX; }, { passive: true });
  viewport.addEventListener('touchend', function(e) {
    var diff = startX - e.changedTouches[0].clientX;
    if (Math.abs(diff) > 50) {
      goTo(diff > 0 ? current + 1 : current - 1);
    }
  });

  // Keyboard arrows
  document.addEventListener('keydown', function(e) {
    if (e.key === 'ArrowRight') goTo(current + 1);
    if (e.key === 'ArrowLeft') goTo(current - 1);
  });
})();

// ===== Mute toggle =====
var muteBtn = document.getElementById('ctrl-mute');
muteBtn.addEventListener('click', function() {
  if (!heroPlayer || !heroPlayer.isMuted) return;
  if (heroPlayer.isMuted()) {
    heroPlayer.unMute();
    muteBtn.classList.remove('is-muted');
  } else {
    heroPlayer.mute();
    muteBtn.classList.add('is-muted');
  }
});

// ===== Play/Pause toggle =====
var ppBtn = document.getElementById('ctrl-playpause');
ppBtn.addEventListener('click', function() {
  if (!heroPlayer || !heroPlayer.getPlayerState) return;
  var state = heroPlayer.getPlayerState();
  if (state === YT.PlayerState.PLAYING) {
    heroPlayer.pauseVideo();
    isPlaying = false;
    ppBtn.classList.add('is-paused');
  } else {
    heroPlayer.playVideo();
    isPlaying = true;
    ppBtn.classList.remove('is-paused');
  }
});

// ===== Platform chooser popup =====
(function() {
  var popup = document.getElementById('platform-popup');
  var closeBtn = document.getElementById('platform-close');
  if (!popup) return;

  function openPopup() {
    popup.classList.add('is-open');
    dismissNudge();
  }
  function closePopup() {
    popup.classList.remove('is-open');
  }

  document.querySelectorAll('.platform-trigger').forEach(function(el) {
    el.addEventListener('click', function(e) {
      e.preventDefault();
      e.stopPropagation();
      openPopup();
    });
  });

  if (closeBtn) closeBtn.addEventListener('click', closePopup);
  popup.addEventListener('click', function(e) { if (e.target === popup) closePopup(); });
  document.addEventListener('keydown', function(e) { if (e.key === 'Escape') closePopup(); });
  window._openPlatformPopup = openPopup;
})();

// ===== Follow nudge =====
var nudgeDismissed = false;
function dismissNudge() {
  nudgeDismissed = true;
  var nudge = document.getElementById('follow-nudge');
  if (nudge) nudge.classList.remove('is-visible');
}

(function() {
  var nudge = document.getElementById('follow-nudge');
  if (!nudge) return;
  if (!nudgeDismissed) nudge.classList.add('is-visible');
  nudge.addEventListener('click', function() {
    if (window._openPlatformPopup) window._openPlatformPopup();
    dismissNudge();
  });
})();
</script>
