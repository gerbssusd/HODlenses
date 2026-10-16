<script setup lang="ts">
// Stylized (not to scale) map of Marlow's route, revealed one stop per click.
const props = defineProps<{ step?: number }>()
const stops = [
  { x: 92, y: 92, label: 'Company offices', sub: 'the unnamed "sepulchral city"', dx: 18, dy: 5 },
  { x: 150, y: 352, label: 'Outer Station', sub: 'on the coast', dx: -14, dy: 50, anchor: 'end' },
  { x: 330, y: 330, label: 'Central Station', sub: 'months repairing the sunken steamer', dx: 14, dy: 36 },
  { x: 610, y: 120, label: 'Inner Station', sub: 'Kurtz, deep in the interior', dx: -10, dy: -28, anchor: 'end' },
]
</script>

<template>
  <svg viewBox="0 0 720 430" class="route" role="img"
       aria-label="Stylized map of Marlow's journey: from the Company's offices in Europe by sea to the Outer Station on the African coast, overland to the Central Station, and upriver to Kurtz at the Inner Station.">
    <defs>
      <pattern id="hatch" width="6" height="6" patternUnits="userSpaceOnUse" patternTransform="rotate(35)">
        <line x1="0" y1="0" x2="0" y2="6" stroke="#9db7b9" stroke-width="1" />
      </pattern>
      <linearGradient id="land" x1="0" x2="1">
        <stop offset="0" stop-color="#efe7d6" /><stop offset="1" stop-color="#e2d6bd" />
      </linearGradient>
    </defs>
    <!-- ocean & land -->
    <rect x="0" y="0" width="720" height="430" fill="url(#hatch)" opacity="0.55" />
    <path d="M 120 430 C 125 380, 140 360, 132 330 C 120 290, 150 250, 200 230 C 260 205, 260 150, 300 120
             C 330 95, 420 60, 520 40 C 600 25, 680 30, 720 20 L 720 430 Z" fill="url(#land)" stroke="#b9a983" stroke-width="1.5" />
    <!-- Europe inset -->
    <rect x="30" y="40" width="190" height="95" rx="10" fill="#fbf8f1" stroke="#b9a983" />
    <text x="44" y="62" class="inset">EUROPE</text>
    <!-- sea passage -->
    <path class="sea" :class="{ on: (props.step ?? 0) >= 2 }" d="M 100 130 C 60 210, 70 300, 140 345" />
    <!-- river -->
    <path class="river" d="M 132 352 C 190 360, 260 345, 330 330 C 400 315, 430 260, 470 230 C 520 190, 560 150, 610 120 C 640 100, 660 95, 700 90" />
    <!-- overland trek -->
    <path class="trek" :class="{ on: (props.step ?? 0) >= 3 }" d="M 150 352 C 200 380, 270 370, 330 330" />
    <path class="upriver" :class="{ on: (props.step ?? 0) >= 4 }" d="M 330 330 C 400 315, 430 260, 470 230 C 520 190, 560 150, 610 120" />
    <text x="455" y="300" class="riverlabel" transform="rotate(-36 455 300)">the river</text>
    <!-- stops -->
    <g v-for="(s, i) in stops" :key="s.label" class="stop" :class="{ on: (props.step ?? 0) >= i + 1 }">
      <circle :cx="s.x" :cy="s.y" r="9" />
      <text :x="s.x + s.dx" :y="s.y + s.dy - 14" class="lbl" :text-anchor="s.anchor || 'start'">{{ s.label }}</text>
      <text :x="s.x + s.dx" :y="s.y + s.dy + 4" class="sub" :text-anchor="s.anchor || 'start'">{{ s.sub }}</text>
    </g>
    <text x="700" y="418" class="note" text-anchor="end">Schematic, not to scale</text>
  </svg>
</template>

<style scoped>
.route { width: 100%; height: auto; border-radius: 14px; background: #f4f1ea; box-shadow: 0 20px 36px -28px rgba(0,0,0,.8); }
.inset { font: 700 12px var(--font-body); letter-spacing: .2em; fill: #8a7b5c; }
.river { fill: none; stroke: #5b8a8f; stroke-width: 7; stroke-linecap: round; opacity: .55; }
.sea, .trek, .upriver { fill: none; stroke: var(--c-oxblood); stroke-width: 3.5; stroke-dasharray: 9 7; opacity: 0; transition: opacity .6s; }
.upriver { stroke-dasharray: none; stroke-width: 5; }
.sea.on, .trek.on, .upriver.on { opacity: 1; }
.stop { opacity: .18; transition: opacity .5s; }
.stop.on { opacity: 1; }
.stop circle { fill: var(--c-oxblood); stroke: #fff; stroke-width: 3; }
.lbl { font: 700 17px var(--font-head); fill: var(--c-ink); }
.sub { font: italic 13px var(--font-body); fill: var(--c-ink-2); }
.riverlabel { font: italic 15px var(--font-body); fill: #3f6d72; }
.note { font: italic 11px var(--font-body); fill: #8a7b5c; }
</style>
