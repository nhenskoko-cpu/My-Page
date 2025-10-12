<section class="community-section fade-in">
  <h2>🌟 Join Our Community</h2>
  <p>
    Be part of an inspiring circle of learners and dreamers.  
    Together, we grow, shine, and uplift each other every day. 🌱✨
  </p>
  <a href="https://m.facebook.com/profile.php?id=61581782202928" target="_blank" class="community-btn">
    💫 Join Our Community
  </a>
</section>

<style>
  .community-section {
    text-align: center;
    background: linear-gradient(180deg, var(--light-bg), #ffffff00);
    padding: 60px 20px;
    margin-top: 60px;
    border-top: 1px solid var(--gold-glow);
    border-bottom: 1px solid var(--gold-glow);
    box-shadow: 0 0 25px rgba(248, 210, 74, 0.3);
    opacity: 0;
    transform: translateY(40px);
    transition: opacity 1.2s ease, transform 1.2s ease;
  }

  .community-section.visible {
    opacity: 1;
    transform: translateY(0);
  }

  .community-section h2 {
    color: var(--deep-blue);
    font-family: 'Poppins', sans-serif;
    font-size: 2em;
    text-shadow: 0 0 12px var(--gold-glow);
  }

  .community-section p {
    color: var(--deep-blue);
    font-size: 1.1em;
    margin: 20px auto;
    max-width: 600px;
    line-height: 1.6;
  }

  .community-btn {
    display: inline-block;
    background: var(--gold-glow);
    color: var(--deep-blue);
    padding: 12px 28px;
    border-radius: 30px;
    font-weight: 700;
    text-decoration: none;
    box-shadow: 0 0 20px var(--gold-glow);
    animation: pulseGlow 3s infinite ease-in-out;
    transition: 0.3s;
  }

  .community-btn:hover {
    background: var(--deep-blue);
    color: var(--gold-glow);
    box-shadow: 0 0 25px var(--gold-glow);
    animation: none;
  }

  @keyframes pulseGlow {
    0% { box-shadow: 0 0 10px var(--gold-glow); transform: scale(1); }
    50% { box-shadow: 0 0 25px var(--gold-glow); transform: scale(1.05); }
    100% { box-shadow: 0 0 10px var(--gold-glow); transform: scale(1); }
  }

  @media (prefers-color-scheme: dark) {
    .community-section {
      background: radial-gradient(circle at top, #00122e, #000);
    }
    .community-section h2, .community-section p {
      color: var(--soft-white);
    }
    .community-btn {
      background: var(--soft-white);
      color: var(--deep-blue);
    }
    .community-btn:hover {
      background: var(--gold-glow);
      color: var(--deep-blue);
    }
  }
</style>

<script>
  // 🌟 Fade-in animation on scroll
  const fadeElements = document.querySelectorAll('.fade-in');

  function handleScroll() {
    fadeElements.forEach(el => {
      const rect = el.getBoundingClientRect();
      if (rect.top < window.innerHeight - 100) {
        el.classList.add('visible');
      }
    });
  }

  window.addEventListener('scroll', handleScroll);
  handleScroll();
</script>