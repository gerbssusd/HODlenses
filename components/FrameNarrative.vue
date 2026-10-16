<script setup lang="ts">
// Three nested narrative frames, revealed outside-in.
const props = defineProps<{ step?: number }>()
const rings = [
  { r: 198, color: '#2f5d62', title: 'Unnamed narrator', sub: 'aboard the Nellie, on the Thames', y: 48 },
  { r: 128, color: '#8a5a14', title: 'Marlow', sub: 'tells the tale of his voyage', y: 112 },
  { r: 62, color: '#7a2e2e', title: 'Kurtz', sub: 'via Marlow', y: 206 },
]
</script>

<template>
  <svg viewBox="0 0 420 420" class="frames" role="img"
       aria-label="Three nested circles: the unnamed narrator on the Thames contains Marlow's tale, which contains Kurtz at the center.">
    <g v-for="(f, i) in rings" :key="f.title" class="ring" :class="{ on: (props.step ?? 0) >= i + 1 }">
      <circle cx="210" cy="210" :r="f.r" :fill="f.color" :fill-opacity="0.12 + i * 0.1" :stroke="f.color" stroke-width="3" />
      <text x="210" :y="f.y" text-anchor="middle" class="t" :fill="f.color">{{ f.title }}</text>
      <text x="210" :y="f.y + 18" text-anchor="middle" class="s">{{ f.sub }}</text>
    </g>
  </svg>
</template>

<style scoped>
.frames { width: 100%; height: auto; max-height: 400px; }
.ring { opacity: 0.12; transition: opacity .6s; }
.ring.on { opacity: 1; }
.t { font: 700 19px var(--font-head); }
.s { font: italic 12.5px var(--font-body); fill: var(--c-ink-2); }
</style>
