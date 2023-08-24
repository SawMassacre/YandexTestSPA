<template>
  <div class="fullscreen-block" :style="{ backgroundColor: color }">
    <slot></slot>
  </div>
</template>

<script>
export default {
  props: ["color"],
};
</script>

<style>
.fullscreen-block {
  width: 100vw;
  height: 100vh;
}
</style>
