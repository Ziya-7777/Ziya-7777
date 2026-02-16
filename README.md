<p align="center">

<svg width="100%" height="500" viewBox="0 0 1200 500" xmlns="http://www.w3.org/2000/svg">

<defs>
  <linearGradient id="sky" x1="0%" y1="0%" x2="0%" y2="100%">
    <stop offset="0%" stop-color="#000000"/>
    <stop offset="100%" stop-color="#1a0033"/>
  </linearGradient>

  <filter id="glow">
    <feGaussianBlur stdDeviation="4" result="blur"/>
    <feMerge>
      <feMergeNode in="blur"/>
      <feMergeNode in="SourceGraphic"/>
    </feMerge>
  </filter>
</defs>

<!-- Background -->
<rect width="1200" height="500" fill="url(#sky)" rx="25"/>

<!-- Stars -->
<circle cx="200" cy="50" r="2" fill="white">
  <animate attributeName="cy" values="0;500" dur="8s" repeatCount="indefinite"/>
</circle>

<circle cx="800" cy="100" r="2" fill="white">
  <animate attributeName="cy" values="0;500" dur="6s" repeatCount="indefinite"/>
</circle>

<!-- Lightning -->
<polyline points="300,50 340,150 310,150 360,260"
          stroke="#00ffff"
          stroke-width="4"
          fill="none"
          filter="url(#glow)">
  <animate attributeName="opacity"
           values="0;1;0"
           dur="2s"
           repeatCount="indefinite"/>
</polyline>

<!-- Floating Image -->
<image href="banner.jpg" x="250" y="130" width="700" height="240">
  <animateTransform attributeName="transform"
                    type="translate"
                    values="0,0;0,-15;0,0"
                    dur="4s"
                    repeatCount="indefinite"/>
</image>

<!-- Glowing Name -->
<text x="600" y="420"
      text-anchor="middle"
      font-size="48"
      fill="#00ffff"
      font-family="Verdana"
      filter="url(#glow)">
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
      stroke-width="3"
      rx="25">
  <animate attributeName="stroke"
           values="#ff00ff;#00ffff;#ff00ff"
           dur="3s"
           repeatCount="indefinite"/>
</rect>

</svg>

</p>

