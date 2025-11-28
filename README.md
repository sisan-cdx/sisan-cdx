<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 120 30" width="600" height="150" role="img" aria-label="Animated snake">
  <defs>
    <path id="snake-path" d="M2 15 C20 5, 40 25, 60 15 C80 5, 100 25, 118 15" fill="none"/>
    <linearGradient id="g" x1="0" x2="1">
      <stop offset="0%" stop-color="#6cc644"/>
      <stop offset="100%" stop-color="#2ea44f"/>
    </linearGradient>
  </defs>

  <!-- invisible path for reference -->
  <use href="#snake-path" fill="none" stroke="transparent" />

  <!-- repeated circles to mimic a snake body -->
  <g fill="url(#g)">
    <circle r="2.5">
      <animateMotion dur="3.5s" repeatCount="indefinite" rotate="auto">
        <mpath href="#snake-path" />
      </animateMotion>
    </circle>
    <circle r="2.5" opacity="0.9">
      <animateMotion begin="-0.25s" dur="3.5s" repeatCount="indefinite" rotate="auto">
        <mpath href="#snake-path" />
      </animateMotion>
    </circle>
    <circle r="2.5" opacity="0.8">
      <animateMotion begin="-0.5s" dur="3.5s" repeatCount="indefinite" rotate="auto">
        <mpath href="#snake-path" />
      </animateMotion>
    </circle>
    <circle r="2.5" opacity="0.7">
      <animateMotion begin="-0.75s" dur="3.5s" repeatCount="indefinite" rotate="auto">
        <mpath href="#snake-path" />
      </animateMotion>
    </circle>
    <circle r="2.5" opacity="0.6">
      <animateMotion begin="-1s" dur="3.5s" repeatCount="indefinite" rotate="auto">
        <mpath href="#snake-path" />
      </animateMotion>
    </circle>
  </g>
</svg>
