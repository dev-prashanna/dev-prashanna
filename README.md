<h1 align="center">
  <svg width="800" height="200" viewBox="0 0 800 200" xmlns="http://www.w3.org/2000/svg">
    <!-- Background -->
    <rect width="800" height="200" fill="#0d1117" rx="8"/>
    
    <!-- Dragon Body -->
    <g transform="translate(100, 80)">
      <!-- Wing back -->
      <path d="M60,30 Q40,-10 15,-25 Q25,-5 28,10 Q18,-15 -5,-20 Q12,0 20,15 Q5,-5 -10,0 Q10,10 25,20 L55,35 Z" 
            fill="#161b22" stroke="#30363d" stroke-width="1">
        <animateTransform attributeName="transform" type="rotate" 
          values="0 60 30;-8 60 30;0 60 30;5 60 30;0 60 30" dur="1.5s" repeatCount="indefinite"/>
      </path>
      
      <!-- Body -->
      <ellipse cx="70" cy="35" rx="35" ry="18" fill="#161b22" stroke="#30363d" stroke-width="1"/>
      
      <!-- Head -->
      <ellipse cx="105" cy="28" rx="18" ry="12" fill="#161b22" stroke="#30363d" stroke-width="1"/>
      
      <!-- Snout -->
      <path d="M120,25 Q132,22 138,25 Q140,30 136,33 Q128,35 120,32 Z" fill="#161b22" stroke="#30363d" stroke-width="0.8"/>
      
      <!-- Eye -->
      <circle cx="112" cy="25" r="3" fill="#f85149">
        <animate attributeName="r" values="3;2.5;3" dur="3s" repeatCount="indefinite"/>
      </circle>
      <circle cx="113" cy="24" r="1" fill="#fff" opacity="0.7"/>
      
      <!-- Horns -->
      <path d="M100,20 Q95,5 98,0" stroke="#f85149" stroke-width="2" fill="none" stroke-linecap="round"/>
      <path d="M108,18 Q106,4 110,0" stroke="#f85149" stroke-width="1.5" fill="none" stroke-linecap="round"/>
      
      <!-- Spine -->
      <path d="M80,22 L78,14 M88,20 L87,12 M96,20 L96,12 M104,21 L105,13" 
            stroke="#f85149" stroke-width="1.5" stroke-linecap="round" opacity="0.6"/>
      
      <!-- Tail -->
      <path d="M38,40 Q20,50 5,45 Q-5,40 -10,48 Q-5,55 5,52 Q-15,50 -20,42" 
            fill="none" stroke="#f85149" stroke-width="2" stroke-linecap="round"/>
      <path d="M-20,42 L-28,35 L-22,42 L-28,50 L-20,42" fill="#f85149" opacity="0.7"/>
      
      <!-- Legs -->
      <path d="M55,50 L50,65 L47,68" stroke="#30363d" stroke-width="1.5" fill="none" stroke-linecap="round"/>
      <path d="M85,48 L88,63 L91,66" stroke="#30363d" stroke-width="1.5" fill="none" stroke-linecap="round"/>
      
      <!-- Wing front -->
      <path d="M60,30 Q40,-10 15,-25 Q25,-5 28,10 Q18,-15 -5,-20 Q12,0 20,15 Q5,-5 -10,0 Q10,10 25,20 L55,35 Z" 
            fill="none" stroke="#30363d" stroke-width="0.8" opacity="0.5">
        <animateTransform attributeName="transform" type="rotate" 
          values="0 60 30;-8 60 30;0 60 30;5 60 30;0 60 30" dur="1.5s" repeatCount="indefinite"/>
      </path>

      <!-- Fire -->
      <g>
        <ellipse cx="155" cy="28" rx="25" ry="6" fill="#f85149" opacity="0">
          <animate attributeName="opacity" values="0;0.6;0.8;0.4;0" dur="4s" repeatCount="indefinite"/>
          <animate attributeName="rx" values="5;20;30;25;5" dur="4s" repeatCount="indefinite"/>
        </ellipse>
        <ellipse cx="170" cy="28" rx="15" ry="4" fill="#f0883e" opacity="0">
          <animate attributeName="opacity" values="0;0.5;0.7;0.3;0" dur="4s" begin="0.2s" repeatCount="indefinite"/>
          <animate attributeName="rx" values="3;15;22;18;3" dur="4s" begin="0.2s" repeatCount="indefinite"/>
        </ellipse>
        <ellipse cx="180" cy="28" rx="8" ry="3" fill="#f0e68c" opacity="0">
          <animate attributeName="opacity" values="0;0.4;0.6;0.2;0" dur="4s" begin="0.4s" repeatCount="indefinite"/>
          <animate attributeName="rx" values="2;10;15;10;2" dur="4s" begin="0.4s" repeatCount="indefinite"/>
        </ellipse>
      </g>

      <!-- Flying path -->
      <animateMotion dur="12s" repeatCount="indefinite"
        path="M0,0 C50,-30 150,20 250,-10 C350,-40 450,10 350,30 C250,50 100,10 0,0"/>
    </g>

    <!-- Title text -->
    <text x="400" y="90" text-anchor="middle" font-family="monospace" font-size="42" font-weight="bold" fill="#f0e68c">
      PRASHANNA
      <animate attributeName="fill" values="#f0e68c;#f85149;#f0e68c" dur="4s" repeatCount="indefinite"/>
    </text>
    <text x="400" y="120" text-anchor="middle" font-family="monospace" font-size="16" fill="#8b949e">
      &gt; cybersecurity_dev --mode=aggressive
    </text>
    <text x="400" y="145" text-anchor="middle" font-family="monospace" font-size="13" fill="#3fb950">
      ESP32 · Android · Pentesting · IoT · Hardware Hacking
    </text>
  </svg>
</h1>

---

## About

Security researcher and hardware hacker focused on **embedded systems exploitation**, **wireless protocol analysis**, and **IoT security**. Building tools that bridge the gap between hardware and software security testing.

Currently developing **CYPHEX** — an ESP32-based wireless security platform with Android companion app for real-time WiFi/BT scanning and packet injection.

---

## Tech Stack

| Category | Technologies |
|----------|-------------|
| **Embedded** | ESP32, Arduino, C/C++, Firmware Reverse Engineering |
| **Mobile** | Kotlin, Jetpack Compose, Android Security |
| **Security** | WiFi/BT Exploitation, Packet Injection, BLE Attacks |
| **Network** | Promiscuous Mode, Deauth Attacks, Evil Portal, Wardriving |
| **Tools** | Kali Linux, Wireshark, Nmap, Burp Suite |
| **Languages** | Python, SQL, Bash, Kotlin, C++ |

---

## Current Project

### CYPHEX — ESP32 Security Platform

| Component | Description |
|-----------|-------------|
| **Firmware** | Filtered ESP32 Marauder for generic ESP32 — WiFi scanning, BLE attacks, packet injection |
| **Android App** | Kotlin/Compose controller with Bluetooth SPP + WiFi/WebSocket connectivity |
| **Features** | Real-time packet monitor, deauth, beacon spam, BLE spam, evil portal, CLI terminal |

```bash
# ESP32 Serial CLI Commands
scanall              # Scan all WiFi networks
sniffbeacon          # Capture beacon frames
attack -t deauth -c  # Deauthentication attack
blespam -t sourapple # BLE Apple spam
packetcount          # Live packet monitor
```

---

## GitHub Stats

<table>
  <tr>
    <td>
      <img src="https://github-readme-stats.vercel.app/api?username=dev-prashanna&show_icons=true&theme=dark&bg_color=0d1117&title_color=f0e68c&icon_color=3fb950&text_color=8b949e&border_color=30363d" width="400" alt="Stats"/>
    </td>
    <td>
      <img src="https://github-readme-streak-stats.herokuapp.com/?user=dev-prashanna&theme=dark&background=0d1117&ring=f0e68c&fire=f85149&currStreakLabel=3fb950&sideLabels=8b949e" width="400" alt="Streak"/>
    </td>
  </tr>
</table>

<table>
  <tr>
    <td>
      <img src="https://github-readme-activity-graph.vercel.app/graph?username=dev-prashanna&bg_color=0d1117&color=3fb950&line=f85149&point=ffffff&area=true&area_color=161b22&hide_border=false" width="830" alt="Activity Graph"/>
    </td>
  </tr>
</table>

---

## Connect

[![GitHub](https://img.shields.io/badge/GitHub-dev--prashanna-8b949e?style=flat&logo=github)](https://github.com/dev-prashanna)
[![Email](https://img.shields.io/badge/Email-developerprashanna@gmail.com-f85149?style=flat&logo=gmail)](mailto:developerprashanna@gmail.com)

---

<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:0d1117,50:161b22,100:0d1117&height=80&section=footer" width="100%"/>
</p>
