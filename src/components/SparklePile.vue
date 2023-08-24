<script>
export default {
  props: {
    number: {
      type: Number,
      default: 4,
    },
  },
  data() {
    const colors = ["#3b71ee", "#fc724c", "#fccb4c", "white"];
    return {
      sparkles: Array.from({ length: this.number }, () => ({
        rotation: (Math.random() + 35) * (Math.random() < 0.5 ? -1 : 1),
        size: Math.random() * 15 + 35,
        position: Math.random() * 30,
        zIndex: Math.floor(Math.random() * 10),
        opacity: Math.random() + 0.4,
        color: colors[Math.floor(Math.random() * colors.length)],
      })),
    };
  },
};
</script>

<template>
  <div id="sparkle-pile">
    <svg
      v-for="(sparkle, index) in sparkles"
      :key="index"
      class="sparkle"
      :style="{
        transform: `rotate(${sparkle.rotation}deg)`,
        width: `${sparkle.size}px`,
        top: `${sparkle.position}vh`,
        zIndex: sparkle.zIndex,
        opacity: sparkle.opacity,
      }"
    >
      <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 256 256">
        <rect width="256" height="256" fill="none" />
        <path
          d="M158.7,163.5l-23.2,63.8a8,8,0,0,1-15,0L97.3,163.5a8.1,8.1,0,0,0-4.8-4.8L28.7,135.5a8,8,0,0,1,0-15L92.5,97.3a8.1,8.1,0,0,0,4.8-4.8l23.2-63.8a8,8,0,0,1,15,0l23.2,63.8a8.1,8.1,0,0,0,4.8,4.8l63.8,23.2a8,8,0,0,1,0,15l-63.8,23.2A8.1,8.1,0,0,0,158.7,163.5Z"
          fill="none"
          :stroke="sparkle.color"
          stroke-linecap="round"
          stroke-linejoin="round"
          stroke-width="24"
        />
      </svg>
    </svg>
  </div>
</template>

<style>
#sparkle-pile {
  position: absolute;
  z-index: 0;
}

.sparkle {
  position: relative;
  margin: 1em;
}
</style>
