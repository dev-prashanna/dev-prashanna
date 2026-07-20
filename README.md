<div align="center">

<!-- ═══════════════════════════════════════════════════════════════ -->
<!--  DRAGON ANIMATION - Kali Linux Aesthetic                       -->
<!-- ═══════════════════════════════════════════════════════════════ -->

<svg width="0" height="0" style="position:absolute">
  <defs>
    <filter id="glow">
      <feGaussianBlur stdDeviation="3" result="coloredBlur"/>
      <feMerge><feMergeNode in="coloredBlur"/><feMergeNode in="SourceGraphic"/></feMerge>
    </filter>
    <filter id="fireGlow">
      <feGaussianBlur stdDeviation="4" result="blur"/>
      <feMerge><feMergeNode in="blur"/><feMergeNode in="SourceGraphic"/></feMerge>
    </filter>
    <radialGradient id="fireGrad" cx="50%" cy="50%" r="50%">
      <stop offset="0%" style="stop-color:#fff700;stop-opacity:1"/>
      <stop offset="30%" style="stop-color:#ff6600;stop-opacity:0.9"/>
      <stop offset="70%" style="stop-color:#ff0000;stop-opacity:0.6"/>
      <stop offset="100%" style="stop-color:#ff0000;stop-opacity:0"/>
    </radialGradient>
    <linearGradient id="dragonBody" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" style="stop-color:#1a1a2e"/>
      <stop offset="50%" style="stop-color:#16213e"/>
      <stop offset="100%" style="stop-color:#0f3460"/>
    </linearGradient>
    <linearGradient id="dragonWing" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" style="stop-color:#0f3460;stop-opacity:0.8"/>
      <stop offset="100%" style="stop-color:#e94560;stop-opacity:0.3"/>
    </linearGradient>
    <linearGradient id="kaliGreen" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" style="stop-color:#36d399"/>
      <stop offset="50%" style="stop-color:#21c45d"/>
      <stop offset="100%" style="stop-color:#1a9c4a"/>
    </linearGradient>
  </defs>
</svg>

<style>
  @keyframes dragonFly {
    0%   { transform: translate(-120px, 60px) rotate(-5deg) scale(0.85); }
    15%  { transform: translate(50px, -30px) rotate(3deg) scale(0.95); }
    30%  { transform: translate(200px, 40px) rotate(-8deg) scale(0.9); }
    45%  { transform: translate(350px, -20px) rotate(5deg) scale(1); }
    60%  { transform: translate(200px, 70px) rotate(-3deg) scale(0.92); }
    75%  { transform: translate(50px, 10px) rotate(7deg) scale(0.88); }
    90%  { transform: translate(-80px, -10px) rotate(-6deg) scale(0.93); }
    100% { transform: translate(-120px, 60px) rotate(-5deg) scale(0.85); }
  }

  @keyframes wingFlap {
    0%, 100% { transform: scaleY(1) rotate(0deg); }
    25%      { transform: scaleY(0.7) rotate(-5deg); }
    50%      { transform: scaleY(1.1) rotate(3deg); }
    75%      { transform: scaleY(0.8) rotate(-3deg); }
  }

  @keyframes fireBreath {
    0%, 40%, 100% { opacity: 0; transform: scale(0) translateX(0); }
    50%           { opacity: 1; transform: scale(1.2) translateX(30px); }
    70%           { opacity: 0.8; transform: scale(1.5) translateX(60px); }
    85%           { opacity: 0.3; transform: scale(0.8) translateX(40px); }
  }

  @keyframes fireParticles {
    0%   { opacity: 1; transform: translate(0, 0) scale(1); }
    100% { opacity: 0; transform: translate(80px, -20px) scale(0.3); }
  }

  @keyframes eyeGlow {
    0%, 100% { filter: drop-shadow(0 0 3px #e94560); opacity: 1; }
    50%      { filter: drop-shadow(0 0 8px #e94560); opacity: 0.8; }
  }

  @keyframes titleGlow {
    0%, 100% { text-shadow: 0 0 10px #36d399, 0 0 20px #36d399, 0 0 40px #1a9c4a; }
    50%      { text-shadow: 0 0 20px #36d399, 0 0 40px #36d399, 0 0 80px #1a9c4a; }
  }

  @keyframes subtitleFlicker {
    0%, 100% { opacity: 1; }
    92%      { opacity: 1; }
    93%      { opacity: 0.3; }
    94%      { opacity: 1; }
    96%      { opacity: 0.5; }
    97%      { opacity: 1; }
  }

  @keyframes float {
    0%, 100% { transform: translateY(0px); }
    50%      { transform: translateY(-8px); }
  }

  @keyframes borderPulse {
    0%, 100% { border-color: rgba(54, 211, 153, 0.3); }
    50%      { border-color: rgba(54, 211, 153, 0.8); }
  }

  .dragon-container {
    position: relative;
    width: 100%;
    height: 280px;
    overflow: hidden;
    margin: -20px 0 0 0;
  }

  .dragon-svg {
    animation: dragonFly 12s ease-in-out infinite;
    filter: drop-shadow(0 0 15px rgba(233, 69, 96, 0.4));
  }

  .dragon-wing {
    transform-origin: 45% 55%;
    animation: wingFlap 1.2s ease-in-out infinite;
  }

  .fire-breath {
    animation: fireBreath 5s ease-in-out infinite;
    transform-origin: left center;
  }

  .fire-particle {
    animation: fireParticles 2s ease-out infinite;
  }

  .fire-particle:nth-child(2) { animation-delay: 0.3s; }
  .fire-particle:nth-child(3) { animation-delay: 0.6s; }
  .fire-particle:nth-child(4) { animation-delay: 0.9s; }
  .fire-particle:nth-child(5) { animation-delay: 1.2s; }

  .dragon-eye {
    animation: eyeGlow 2s ease-in-out infinite;
  }

  .hero-title {
    font-size: 2.8em;
    font-weight: 900;
    letter-spacing: 4px;
    animation: titleGlow 3s ease-in-out infinite;
    margin: 10px 0 5px 0;
  }

  .hero-subtitle {
    font-family: 'Courier New', monospace;
    font-size: 1.1em;
    color: #36d399;
    animation: subtitleFlicker 4s infinite;
    margin: 5px 0;
  }

  .section-card {
    background: linear-gradient(135deg, rgba(26, 26, 46, 0.8), rgba(15, 52, 96, 0.6));
    border: 1px solid rgba(54, 211, 153, 0.3);
    border-radius: 12px;
    padding: 20px;
    margin: 15px 0;
    animation: borderPulse 4s ease-in-out infinite, float 6s ease-in-out infinite;
    backdrop-filter: blur(10px);
  }

  .tech-badge {
    display: inline-block;
    padding: 5px 14px;
    margin: 4px;
    border-radius: 20px;
    font-size: 0.85em;
    font-weight: 600;
    border: 1px solid rgba(54, 211, 153, 0.4);
    background: rgba(54, 211, 153, 0.1);
    color: #36d399;
    transition: all 0.3s ease;
  }

  .tech-badge:hover {
    background: rgba(54, 211, 153, 0.25);
    border-color: #36d399;
    transform: translateY(-2px);
  }

  .stat-card {
    display: inline-block;
    text-align: center;
    padding: 12px 24px;
    margin: 6px;
    border-radius: 10px;
    background: rgba(15, 52, 96, 0.5);
    border: 1px solid rgba(233, 69, 96, 0.3);
    min-width: 100px;
  }

  .stat-number {
    font-size: 1.8em;
    font-weight: 800;
    color: #e94560;
    display: block;
  }

  .stat-label {
    font-size: 0.8em;
    color: #8892b0;
    text-transform: uppercase;
    letter-spacing: 1px;
  }

  .kali-divider {
    height: 2px;
    background: linear-gradient(90deg, transparent, #36d399, #e94560, #36d399, transparent);
    margin: 25px 0;
    border: none;
  }

  a {
    color: #36d399;
    text-decoration: none;
    transition: all 0.3s ease;
  }

  a:hover {
    color: #e94560;
    text-shadow: 0 0 10px rgba(233, 69, 96, 0.5);
  }
</style>

<!-- ═══════════════ DRAGON ANIMATION ═══════════════ -->
<div class="dragon-container">
<svg class="dragon-svg" viewBox="0 0 300 180" width="300" height="180" xmlns="http://www.w3.org/2000/svg">
  <!-- Dragon Body -->
  <path d="M120,95 Q130,75 150,70 Q170,65 185,72 Q200,80 195,95 Q190,110 175,115 Q160,120 140,118 Q125,115 120,105 Z" 
        fill="url(#dragonBody)" stroke="#e94560" stroke-width="1.5" filter="url(#glow)"/>
  
  <!-- Dragon Head -->
  <path d="M185,72 Q200,65 215,68 Q225,72 228,80 Q230,88 222,92 Q210,95 195,95 Q188,90 185,82 Z" 
        fill="#1a1a2e" stroke="#e94560" stroke-width="1.2"/>
  
  <!-- Dragon Snout -->
  <path d="M222,80 Q235,76 245,78 Q250,82 248,88 Q242,92 232,90 Q225,88 222,85 Z" 
        fill="#16213e" stroke="#e94560" stroke-width="1"/>
  
  <!-- Dragon Jaw -->
  <path d="M228,88 Q238,92 245,95 Q240,98 232,96 Q225,94 222,90 Z" 
        fill="#0f3460" stroke="#e94560" stroke-width="0.8"/>
  
  <!-- Dragon Eye -->
  <ellipse class="dragon-eye" cx="218" cy="78" rx="4" ry="3.5" fill="#e94560"/>
  <ellipse cx="219" cy="77" rx="1.5" ry="1.5" fill="#fff" opacity="0.8"/>
  
  <!-- Dragon Horns -->
  <path d="M200,68 Q195,50 200,42 Q205,50 210,60" fill="none" stroke="#e94560" stroke-width="2" stroke-linecap="round"/>
  <path d="M208,65 Q205,48 210,40 Q214,48 215,58" fill="none" stroke="#e94560" stroke-width="1.5" stroke-linecap="round"/>
  
  <!-- Dragon Wing (Back) -->
  <g class="dragon-wing">
    <path d="M145,80 Q130,40 105,25 Q115,35 120,50 Q110,30 95,20 Q108,38 115,55 Q100,35 80,30 Q95,45 110,60 Q90,45 70,45 Q90,55 110,65 L135,85 Z" 
          fill="url(#dragonWing)" stroke="#e94560" stroke-width="1" opacity="0.9"/>
  </g>
  
  <!-- Dragon Tail -->
  <path d="M120,100 Q100,110 80,105 Q60,100 45,110 Q35,120 30,115 Q40,105 55,100 Q45,95 35,85 Q50,90 65,95 Q55,85 45,75 Q60,80 75,90 Q85,80 95,85 Q105,90 115,95" 
          fill="none" stroke="#e94560" stroke-width="2" stroke-linecap="round" filter="url(#glow)"/>
  
  <!-- Tail Spade -->
  <path d="M35,85 L25,75 L30,85 L25,95 L35,85" fill="#e94560" opacity="0.8"/>
  
  <!-- Dragon Spine -->
  <path d="M140,68 L138,58 M150,65 L149,55 M160,67 L160,57 M170,70 L171,60 M178,73 L180,63" 
        stroke="#e94560" stroke-width="1.5" stroke-linecap="round" opacity="0.7"/>
  
  <!-- Dragon Chest Scales -->
  <path d="M145,100 Q155,105 165,102 Q175,98 185,100" fill="none" stroke="#36d399" stroke-width="0.8" opacity="0.4"/>
  <path d="M150,105 Q160,108 170,106 Q180,102 188,104" fill="none" stroke="#36d399" stroke-width="0.6" opacity="0.3"/>
  
  <!-- LEGS -->
  <path d="M145,115 Q142,130 138,140 Q135,145 132,142" fill="none" stroke="#e94560" stroke-width="1.5" stroke-linecap="round"/>
  <path d="M170,112 Q172,128 175,138 Q177,143 180,140" fill="none" stroke="#e94560" stroke-width="1.5" stroke-linecap="round"/>
  
  <!-- Claws -->
  <path d="M132,142 L128,145 M132,142 L130,147 M132,142 L134,146" stroke="#e94560" stroke-width="1" stroke-linecap="round"/>
  <path d="M180,140 L176,143 M180,140 L178,146 M180,140 L182,144" stroke="#e94560" stroke-width="1" stroke-linecap="round"/>

  <!-- ════════ FIRE BREATH ════════ -->
  <g class="fire-breath" filter="url(#fireGlow)">
    <!-- Main fire stream -->
    <ellipse cx="260" cy="84" rx="35" ry="12" fill="url(#fireGrad)" opacity="0.9"/>
    <ellipse cx="275" cy="84" rx="25" ry="8" fill="#ff6600" opacity="0.7"/>
    <ellipse cx="285" cy="84" rx="15" ry="5" fill="#fff700" opacity="0.8"/>
    
    <!-- Fire particles -->
    <circle class="fire-particle" cx="270" cy="78" r="3" fill="#ff6600" opacity="0.8"/>
    <circle class="fire-particle" cx="280" cy="88" r="2.5" fill="#ff9500" opacity="0.7"/>
    <circle class="fire-particle" cx="265" cy="90" r="2" fill="#e94560" opacity="0.6"/>
    <circle class="fire-particle" cx="290" cy="80" r="2" fill="#fff700" opacity="0.5"/>
    <circle class="fire-particle" cx="275" cy="75" r="1.5" fill="#ff6600" opacity="0.6"/>
    
    <!-- Sparks -->
    <circle cx="295" cy="76" r="1" fill="#fff700" opacity="0.9">
      <animate attributeName="opacity" values="0.9;0;0.9" dur="0.8s" repeatCount="indefinite"/>
    </circle>
    <circle cx="300" cy="82" r="0.8" fill="#ff9500" opacity="0.8">
      <animate attributeName="opacity" values="0.8;0;0.8" dur="0.6s" repeatCount="indefinite"/>
    </circle>
    <circle cx="288" cy="72" r="1.2" fill="#fff700" opacity="0.7">
      <animate attributeName="opacity" values="0.7;0;0.7" dur="1s" repeatCount="indefinite"/>
    </circle>
  </g>
</svg>
</div>

<!-- ═══════════════ HERO SECTION ═══════════════ -->

<h1 class="hero-title" style="color: #e94560;">PRASHANNA</h1>
<p class="hero-subtitle">&gt; <span style="color:#e94560">$</span> whoami <span style="color:#36d399">_</span></p>

<p style="color: #8892b0; font-size: 1.05em; max-width: 600px; margin: 10px auto;">
  <b style="color:#36d399">Cybersecurity Enthusiast</b> · 
  <b style="color:#e94560">Hardware Hacker</b> · 
  <b style="color:#36d399">Embedded Systems</b>
</p>

<img src="https://komarev.com/ghpvc/?username=dev-prashanna&color=36d399&style=for-the-badge&label=PROFILE+VIEWS" alt="views"/>

<hr class="kali-divider"/>

<!-- ═══════════════ STATS ═══════════════ -->

<div style="display: flex; justify-content: center; flex-wrap: wrap;">
  <div class="stat-card">
    <span class="stat-number">ESP32</span>
    <span class="stat-label">Hardware</span>
  </div>
  <div class="stat-card">
    <span class="stat-number" style="color:#36d399">Kali</span>
    <span class="stat-label">Pentesting</span>
  </div>
  <div class="stat-card">
    <span class="stat-number">IoT</span>
    <span class="stat-label">Security</span>
  </div>
</div>

<hr class="kali-divider"/>

<!-- ═══════════════ CURRENT PROJECT ═══════════════ -->

<div class="section-card">
  <h2 style="color:#e94560; margin-top:0;">🐉 Current Project: CYPHEX</h2>
  <p style="color:#8892b0;">
    ESP32-based wireless security testing platform with Android companion app.
    Real-time packet injection, WiFi/BT scanning, and BLE attacks — all from your phone.
  </p>
  <div style="margin-top: 12px;">
    <a href="https://github.com/dev-prashanna/CYPHEX">
      <img src="https://img.shields.io/badge/Repository-CYPHEX-36d399?style=for-the-badge&logo=github" alt="CYPHEX"/>
    </a>
    <a href="https://github.com/dev-prashanna/CYPHEX/tree/main/ESP32Marauder-Controller">
      <img src="https://img.shields.io/badge/Android_App-Kotlin-e94560?style=for-the-badge&logo=kotlin" alt="Kotlin"/>
    </a>
    <a href="https://github.com/dev-prashanna/CYPHEX/tree/main/ESP32Marauder">
      <img src="https://img.shields.io/badge/Firmware-ESP32-36d399?style=for-the-badge&logo=espressif" alt="ESP32"/>
    </a>
  </div>
</div>

<!-- ═══════════════ TECH STACK ═══════════════ -->

<div class="section-card">
  <h2 style="color:#36d399; margin-top:0;">⚡ Tech Arsenal</h2>
  <div>
    <span class="tech-badge">ESP32</span>
    <span class="tech-badge">Kotlin</span>
    <span class="tech-badge">Jetpack Compose</span>
    <span class="tech-badge">Android</span>
    <span class="tech-badge">Bluetooth SPP</span>
    <span class="tech-badge">WebSocket</span>
    <span class="tech-badge">WiFi Security</span>
    <span class="tech-badge">BLE</span>
    <span class="tech-badge">Penetration Testing</span>
    <span class="tech-badge">Embedded C++</span>
    <span class="tech-badge">Arduino</span>
    <span class="tech-badge">Material 3</span>
    <span class="tech-badge">Hilt DI</span>
    <span class="tech-badge">Room DB</span>
    <span class="tech-badge">Linux</span>
    <span class="tech-badge">Git</span>
    <span class="tech-badge">Python</span>
    <span class="tech-badge">SQL</span>
  </div>
</div>

<!-- ═══════════════ GITHUB STATS ═══════════════ -->

<div class="section-card" style="text-align:center;">
  <h2 style="color:#e94560; margin-top:0;">📊 GitHub Analytics</h2>
  <img src="https://github-readme-stats.vercel.app/api?username=dev-prashanna&show_icons=true&theme=chartreuse-dark&bg_color=0a0a1a&title_color=e94560&icon_color=36d399&text_color=8892b0&border_color=36d399&hide_border=false" width="48%" alt="Stats"/>
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=dev-prashanna&theme=chartreuse-dark&background=0a0a1a&ring=36d399&fire=e94560&currStreakLabel=36d399&sideLabels=e94560" width="48%" alt="Streak"/>
  <br/>
  <img src="https://github-readme-activity-graph.vercel.app/graph?username=dev-prashanna&bg_color=0a0a1a&color=36d399&line=e94560&point=36d399&area_color=0f3460&area=true&hide_border=false" width="97%" alt="Activity Graph"/>
</div>

<!-- ═══════════════ CONTRIBUTION蛇 ═══════════════ -->

<div class="section-card" style="text-align:center;">
  <h2 style="color:#36d399; margin-top:0;">🔥 Contribution Heatmap</h2>
  <img src="https://github-readme-activity-graph.vercel.app/graph?username=dev-prashanna&bg_color=0a0a1a&color=36d399&line=e94560&point=ffffff&area=true&area_color=e94560&hide_border=false&custom_title=CONTRIBUTION%20GRAPH" width="97%" alt="Graph"/>
</div>

<hr class="kali-divider"/>

<!-- ═══════════════ CONNECT ═══════════════ -->

<div style="text-align:center; margin: 20px 0;">
  <h2 style="color:#e94560;">🐍 Connect</h2>
  <a href="https://github.com/dev-prashanna">
    <img src="https://img.shields.io/badge/GitHub-dev--prashanna-36d399?style=for-the-badge&logo=github" alt="GitHub"/>
  </a>
  <a href="mailto:developerprashanna@gmail.com">
    <img src="https://img.shields.io/badge/Email-DevPrashanna-e94560?style=for-the-badge&logo=gmail" alt="Email"/>
  </a>
</div>

<!-- ═══════════════ FOOTER ═══════════════ -->

<hr class="kali-divider"/>

<p style="text-align:center; color:#8892b0; font-family: 'Courier New', monospace; font-size:0.85em;">
  <span style="color:#36d399">$</span> echo "Hacked with 🐉 by <span style="color:#e94560">Prashanna</span>" <span style="color:#36d399">|</span> <span style="color:#e94560">figlet</span>
</p>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0f3460,50:1a1a2e,100:0f3460&height=120&section=footer&text=PRASHANNA&fontSize=50&fontColor=36d399&fontAlignY=35&desc=CYBERSECURITY+%7C+HARDWARE+HACKING+%7C+IoT&descSize=14&descAlignY=55&descAlign=50&animation=twinkling" width="100%" alt="Footer"/>

</div>
