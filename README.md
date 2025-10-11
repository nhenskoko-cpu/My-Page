<style>
  /* 🌸 Intro Screen Styling */
  #introScreen {
    position: fixed;
    inset: 0;
    background: radial-gradient(circle at center, #00153a 0%, #00091c 100%);
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    color: white;
    font-family: 'Poppins', sans-serif;
    z-index: 9999;
    animation: fadeOutIntro 1s ease forwards;
    animation-delay: 3.5s; /* stays for ~3.5 seconds */
  }

  .intro-content {
    text-align: center;
    animation: fadeInUp 1.5s ease;
  }

  .logo-glow {
    font-size: 4rem;
    color: gold;
    text-shadow: 
      0 0 10px silver,
      0 0 20px #9dd9ff,
      0 0 40px rgba(255,255,255,0.8);
    margin-bottom: 20px;
    animation: shimmer 3s infinite ease-in-out;
  }

  #introScreen h1 {
    font-size: 2.6rem;
    color: #f8b400;
    margin: 0;
    text-shadow: 0 0 15px rgba(255,255,255,0.7);
    animation: glowText 2s infinite alternate;
  }

  #introScreen p {
    font-size: 1.2rem;
    color: #e6e6e6;
    margin-top: 10px;
    opacity: 0.9;
  }

  @keyframes shimmer {
    0% { text-shadow: 0 0 10px silver, 0 0 20px #9dd9ff; }
    50% { text-shadow: 0 0 30px white, 0 0 50px #9dd9ff; }
    100% { text-shadow: 0 0 10px silver, 0 0 20px #9dd9ff; }
  }

  @keyframes fadeInUp {
    from { opacity: 0; transform: translateY(30px); }
    to { opacity: 1; transform: translateY(0); }
  }

  @keyframes glowText {
    0% { text-shadow: 0 0 10px #f8b400; }
    100% { text-shadow: 0 0 30px #9b59b6; }
  }

  @keyframes fadeOutIntro {
    to { opacity: 0; visibility: hidden; }
  }

  body.loaded #introScreen {
    animation: fadeOutIntro 1s ease forwards;
  }
</style>
