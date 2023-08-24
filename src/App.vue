<template>
  <fullscreen-block :color="'#3b71ee'"></fullscreen-block>
  <fullscreen-block :color="'#fc724c'"></fullscreen-block>
  <fullscreen-block :color="'#fccb4c'"></fullscreen-block>
</template>

<script>
import FullscreenBlock from "./components/FullscreenBlock.vue";

export default {
  name: "App",
  components: {
    FullscreenBlock,
  },
};
</script>
