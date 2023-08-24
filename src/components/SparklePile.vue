<template>
  <div id="sparkle-pile">
    <img
      v-for="(sparkle, index) in sparkles"
      :key="index"
      src="../assets/sparkle.webp"
      class="sparkle"
      :style="{
        transform: `rotate(${sparkle.rotation}deg)`,
        width: `${sparkle.size}px`,
        top: `${sparkle.position}vh`,
      }"
    />
  </div>
</template>

<script>
export default {
  props: {
    number: {
      type: Number,
      default: 4,
    },
  },
  data() {
    return {
      sparkles: Array.from({ length: this.number }, () => ({
        rotation: (Math.random() + 35) * (Math.random() < 0.5 ? -1 : 1),
        size: Math.random() * 15 + 35,
        position: Math.random() * 30,
      })),
    };
  },
};
</script>

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
