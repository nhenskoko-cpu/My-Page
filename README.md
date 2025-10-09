Growth and Shine 
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Aurena’s Magical Learn & Grow Page</title>

<!-- Google Font -->
<link href="https://fonts.googleapis.com/css2?family=Quicksand:wght@400;600;700&display=swap" rel="stylesheet">

<style>
body {
  font-family: 'Quicksand', sans-serif;
  background: linear-gradient(135deg, #fff7fc, #f0faff);
  margin: 0;
  color: #333;
  overflow-x: hidden;
}

/* 🌈 Section */
.inspiration-section {
  text-align: center;
  padding: 60px 15px;
}

/* 🌈 Title */
.rainbow-title {
  font-size: 2.3em;
  font-weight: 700;
  background: linear-gradient(90deg, #ff7eb9, #ff65a3, #7afcff, #feff9c, #fff740, #ff7eb9);
  background-size: 400%;
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  animation: rainbowFlow 8s ease infinite;
}
@keyframes rainbowFlow {
  0% { background-position: 0% 50%; }
  50% { background-position: 100% 50%; }
  100% { background-position: 0% 50%; }
}

/* ✨ Grid */
.inspiration-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  gap: 25px;
  max-width: 900px;
  margin: 40px auto;
}

/* 💖 Boxes */
.inspire-box {
  background: #ffffffd9;
  border-radius: 20px;
  padding: 20px;
  box-shadow: 0 4px 12px rgba(255, 182, 193, 0.3);
  transition: 0.4s;
  opacity: 0;
  transform: translateY(20px);
}
.inspire-box:hover {
  transform: translateY(-8px) scale(1.03);
  box-shadow: 0 6px 18px rgba(255, 105, 180, 0.35);
}

/* Fade in */
.fade1 { animation: fadeInBox 1s ease forwards 0.5s; }
.fade2 { animation: fadeInBox 1s ease forwards 1s; }
.fade3 { animation: fadeInBox 1s ease forwards 1.5s; }
.fade4 { animation: fadeInBox 1s ease forwards 2s; }
@keyframes fadeInBox {
  from { opacity: 0; transform: translateY(30px); }
  to { opacity: 1; transform: translateY(0); }
}

/* Button */
.inspire-btn {
  display: inline-block;
  margin-top: 12px;
  padding: 12px 24px;
  font-size: 16px;
  border-radius: 28px;
  background-color: #ff66b3;
  color: #fff;
  text-decoration: none;
  font-weight: 600;
  transition: 0.3s;
  animation: pulseHeart 3s ease-in-out infinite;
}
.inspire-btn:hover {
  background-color: #ff85c1;
  transform: scale(1.05);
}
@keyframes pulseHeart {
  0%,100% { transform: scale(1); box-shadow: 0 0 0 rgba(255,102,179,0); }
  50% { transform: scale(1.08); box-shadow: 0 0 15px rgba(255,102,179,0.4); }
}

/* Learn Content */
.learn-content {
  display: none;
  max-width: 700px;
  margin: 25px auto;
  background: #fffafc;
  border-radius: 18px;
  padding: 25px;
  box-shadow: 0 6px 20px rgba(255,182,193,0.25);
  position: relative;
  overflow: hidden;
}
.learn-content.open { display: block; animation: fadeInBox 1s ease forwards; }

/* Sparkle Particles */
.sparkle {
  position: absolute;
  width: 6px;
  height: 6px;
  background: radial-gradient(circle, #fffacd 0%, rgba(255, 255, 255, 0) 70%);
  border-radius: 50%;
  opacity: 0.7;
  pointer-events: none;
  animation: sparkleMove linear infinite;
}
@keyframes sparkleMove {
  0% { transform: translate(0,0) scale(0.5); opacity: 0; }
  10% { opacity: 0.8; }
  50% { opacity: 0.6; }
  100% { transform: translate(var(--sparkle-x,0), var(--sparkle-y,-200px)) scale(1.2); opacity: 0; }
}

/* Floating Emojis */
.floating-emoji {
  position: absolute;
  font-size: 1.6rem;
  animation: floatEmoji linear infinite;
  opacity: 0.8;
}
@keyframes floatEmoji {
  0% { transform: translateY(0) rotate(0deg); opacity: 0; }
  10% { opacity: 1; }
  90% { opacity: 1; }
  100% { transform: translateY(-180px) rotate(360deg); opacity: 0; }
}
</style>
</head>
<body>

<section id="content-sections" class="inspiration-section">
  <h2 class="rainbow-title">🌈 Four Ways to Grow and Shine</h2>

  <div class="inspiration-grid">
    <div class="inspire-box fade1">
      <h3>🌱 Mindset Tips</h3>
      <p>Stay positive, build confidence, and focus your energy on becoming your best self every day.</p>
      <a href="#mindset" class="inspire-btn" onclick="toggleContent('mindset')">Learn 🌸</a>
    </div>

    <div class="inspire-box fade2">
      <h3>💼 Simple Business Tips</h3>
      <p>Learn simple ways to grow your ideas into a successful business—step by step!</p>
      <a href="#business" class="inspire-btn" onclick="toggleContent('business')">Learn 💖</a>
    </div>

    <div class="inspire-box fade3">
      <h3>🌟 Community Inspiration</h3>
      <p>Feel encouraged by real stories of people spreading kindness and positive change.</p>
      <a href="#community" class="inspire-btn" onclick="toggleContent('community')">Learn 💕</a>
    </div>

    <div class="inspire-box fade4">
      <h3>📈 Leadership & Growth</h3>
      <p>Lead with purpose, grow with passion, and make an inspiring impact wherever you go.</p>
      <a href="#leadership" class="inspire-btn" onclick="toggleContent('leadership')">Learn ✨</a>
    </div>
  </div>

  <div id="mindset" class="learn-content">
    <h3>🌱 Mindset Tips</h3>
    <p>Believe in your potential and treat every challenge as a teacher. Each moment of growth starts with a choice to keep going. 🌻</p>
  </div>

  <div id="business" class="learn-content">
    <h3>💼 Simple Business Tips</h3>
    <p>Start small, stay consistent, and give your work a personal touch. Every great business began with courage and care. 💼✨</p>
  </div>

  <div id="community" class="learn-content">
    <h3>🌟 Community Inspiration</h3>
    <p>Kindness grows when shared. Inspire others through small actions that brighten hearts. 🌸🌍</p>
  </div>

  <div id="leadership" class="learn-content">
    <h3>📈 Leadership & Growth</h3>
    <p>True leaders lift others. Lead with love, stay humble, and keep learning—your light guides the way. 🌞</p>
  </div>
</section>

<audio id="chime-sound" src="https://www.soundjay.com/misc/sounds/bell-ringing-05.mp3" preload="auto"></audio>

<script>
const emojiSets = {
  mindset: ['🌿','🌸','💫','✨','🍃'],
  business: ['💼','💖','💡','📈','🌟'],
  community: ['🌍','💞','🌸','🌈','🤝'],
  leadership: ['🔥','🌞','⭐','🚀','💪']
};

function createFloatingEmojis(section, emojis) {
  for(let i=0; i<12; i++) {
    const emoji = document.createElement('span');
    emoji.className = 'floating-emoji';
    emoji.textContent = emojis[Math.floor(Math.random() * emojis.length)];
    emoji.style.left = `${Math.random()*90}%`;
    emoji.style.bottom = '-20px';
    emoji.style.animationDuration = `${3+Math.random()*3}s`;
    emoji.style.animationDelay = `${Math.random()*2}s`;
    section.appendChild(emoji);
  }
}

function createSparkles(section, count=15) {
  for(let i=0;i<count;i++){
    const sparkle = document.createElement('span');
    sparkle.className = 'sparkle';
    sparkle.style.left = `${Math.random()*100}%`;
    sparkle.style.top = `${Math.random()*100}%`;
    sparkle.style.setProperty('--sparkle-x', `${(Math.random()-0.5)*100}px`);
    sparkle.style.setProperty('--sparkle-y', `${-100-Math.random()*100}px`);
    sparkle.style.animationDuration = `${4+Math.random()*4}s`;
    sparkle.style.animationDelay = `${Math.random()*3}s`;
    section.appendChild(sparkle);
  }
}

function toggleContent(id){
  const section = document.getElementById(id);
  const all = document.querySelectorAll('.learn-content');
  all.forEach(s=>{
    s.classList.remove('open');
    s.querySelectorAll('.floating-emoji,.sparkle').forEach(e=>e.remove());
  });

  section.classList.toggle('open');
  if(section.classList.contains('open')){
    createFloatingEmojis(section, emojiSets[id]);
    createSparkles(section, 20);
    const chime = document.getElementById('chime-sound');
    chime.currentTime = 0;
    chime.play().catch(()=>{});
  }
  section.scrollIntoView({behavior:'smooth', block:'center'});
}
</script>
</body>
</html>
