<template>
  <!-- A small river-steamer silhouette crossing a line of water: decorative motif -->
  <svg viewBox="0 0 900 90" class="steamer" role="img" aria-label="Decorative silhouette of a stern-wheel river steamer on a river.">
    <path d="M0 70 Q 75 62 150 70 T 300 70 T 450 70 T 600 70 T 750 70 T 900 70" class="water" />
    <path d="M0 80 Q 75 72 150 80 T 300 80 T 450 80 T 600 80 T 750 80 T 900 80" class="water thin" />
    <g class="boat">
      <path d="M 20 62 L 150 62 L 140 70 L 30 70 Z" />
      <rect x="40" y="44" width="80" height="18" rx="2" />
      <rect x="55" y="30" width="44" height="14" rx="2" />
      <rect x="100" y="12" width="8" height="32" />
      <circle cx="150" cy="58" r="11" class="wheel" />
      <path d="M 104 10 q 10 -8 22 -4 q 12 4 24 -2" class="smoke" />
    </g>
  </svg>
</template>

<style scoped>
.steamer { width: 100%; height: auto; }
.water { fill: none; stroke: #5b8a8f; stroke-width: 3; opacity: .6; }
.water.thin { stroke-width: 1.5; opacity: .35; }
.boat { fill: #2a231d; animation: drift 14s linear infinite alternate; }
.wheel { fill: none; stroke: #2a231d; stroke-width: 4; stroke-dasharray: 4 3; }
.smoke { fill: none; stroke: #8b8073; stroke-width: 3; stroke-linecap: round; opacity: .7; }
@keyframes drift { from { transform: translateX(40px); } to { transform: translateX(680px); } }
@media print { .boat { animation: none; transform: translateX(360px); } }
</style>
