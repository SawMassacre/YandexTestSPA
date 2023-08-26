<template>
  <div
    class="neobrutalism-message"
    :class="[
      direction === 'left' ? 'triangle left-top' : 'triangle right-bottom',
    ]"
  >
    <div class="talktext">
      <p style="color: #282828; font-size: 1.5em; padding: 1em">
        <slot></slot>
      </p>
    </div>
  </div>
</template>

<script>
export default {
  name: "NeobrutalismMessage",
  props: {
    direction: {
      type: String,
      default: "left",
      validator: function (value) {
        return ["left", "right"].includes(value);
      },
    },
  },
};
</script>

<style scoped>
.neobrutalism-message {
  margin: 40px;
  display: inline-block;
  position: relative;
  height: auto;
  background-color: #ffffff;
  font-family: monospace;
}

.triangle.left-top::after {
  content: " ";
  position: absolute;
  width: 0;
  height: 0;
  left: -20px;
  right: auto;
  top: 0px;
  bottom: auto;
  border: 22px solid;
  border-color: #ffffff transparent transparent transparent;
}

.triangle.right-bottom::after {
  content: " ";
  position: absolute;
  width: 0;
  height: 0;
  right: -20px;
  left: auto;
  top: auto;
  bottom: 0px;
  border: 22px solid;
  border-color: transparent transparent #ffffff transparent;
}
</style>
