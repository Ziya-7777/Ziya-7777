<p align="center">
  <img src="banner.jpg" width="600" />
</p>
<p align="center">
<svg width="100%" height="450" viewBox="0 0 1200 450" xmlns="http://www.w3.org/2000/svg">
<p align="center">
<svg width="100%" height="500" viewBox="0 0 1200 500" xmlns="http://www.w3.org/2000/svg">

<defs>

<!-- Animated Background Gradient -->
<linearGradient id="sky" x1="0%" y1="0%" x2="0%" y2="100%">
  <stop offset="0%" stop-color="#000000"/>
  <stop offset="100%" stop-color="#1a0033"/>
</linearGradient>

<!-- Electric Glow -->
<filter id="electricGlow">
  <feGaussianBlur stdDeviation="5" result="blur"/>
  <feMerge>
    <feMergeNode in="blur"/>
    <feMergeNode in="SourceGraphic"/>
  </feMerge>
</filter>

<!-- Neon Border Glow -->
<filter id="neonBorder">
  <feGaussianBlur stdDeviation="8" result="glow"/>
  <feMerge>
    <feMergeNode in="glow"/>
    <feMergeNode in="SourceGraphic"/>
  </feMerge>
</filter>

</defs>

<!-- Background -->
<rect width="1200" height="500" fill="url(#sky)" rx="25"/>

<!-- Moving Starfield -->
<g>
  <circle cx="100" cy="50" r="2" fill="white">
    <animate attributeName="cy" values="0;500" dur="6s" repeatCount="indefinite"/>
  </circle>
  <circle cx="400" cy="80" r="2" fill="white">
    <animate attributeName="cy" values="0;500" dur="8s" repeatCount="indefinite"/>
  </circle>
  <circle cx="900" cy="30" r="2" fill="white">
    <animate attributeName="cy" values="0;500" dur="7s" repeatCount="indefinite"/>
  </circle>
</g>

<!-- Rain -->
<g stroke="#66ccff" stroke-width="2">
  <line x1="200" y1="0" x2="200" y2="20">
    <animate attributeName="y1" values="0;500" dur="1s" repeatCount="indefinite"/>
    <animate attributeName="y2" values="20;520" dur="1s" repeatCount="indefinite"/>
  </line>
  <line x1="800" y1="0" x2="800" y2="20">
    <animate attributeName="y1" values="0;500" dur="1.2s" repeatCount="indefinite"/>
    <animate attributeName="y2" values="20;520" dur="1.2s" repeatCount="indefinite"/>
  </line>
</g>

<!-- Lightning -->
<polyline points="300,50 340,150 310,150 360,260"
          stroke="#00ffff"
          stroke-width="4"
          fill="none"
          filter="url(#electricGlow)">
  <animate attributeName="opacity"
           values="0;1;0"
           dur="2s"
           repeatCount="indefinite"/>
</polyline>

<polyline points="900,70 930,170 890,170 940,280"
          stroke="#ff00ff"
          stroke-width="4"
          fill="none"
          filter="url(#electricGlow)">
  <animate attributeName="opacity"
           values="0;1;0"
           dur="3s"
           repeatCount="indefinite"/>
</polyline>

<!-- Floating Banner Image -->
<image href="banner.jpg" x="250" y="140" width="700" height="220">
  <animateTransform attributeName="transform"
                    type="translate"
                    values="0,0; 0,-15; 0,0"
                    dur="4s"
                    repeatCount="indefinite"/>
</image>

<!-- Electric Animated Name -->
<text x="600" y="420"
      text-anchor="middle"
      font-size="50"
      fill="#00ffff"
      font-family="Orbitron"
      filter="url(#electricGlow)">
  ZIYA
  <animate attributeName="fill"
           values="#00ffff;#ff00ff;#00ffff"
           dur="2s"
           repeatCount="indefinite"/>
</text>

<!-- Neon Border -->
<rect x="5" y="5" width="1190" height="490"
      fill="none"
      stroke="#ff00ff"
      stroke-width="4"
      rx="25"
      filter="url(#neonBorder)">
  <animate attributeName="stroke"
           values="#ff00ff;#00ffff;#ff00ff"
           dur="3s"
           repeatCount="indefinite"/>
</rect>

</svg>
</p>
