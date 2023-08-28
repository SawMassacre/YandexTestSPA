<template>
  <div class="container">
    <div
      class="neobrutalism-message"
      :class="[
        direction === 'left' ? 'triangle left-top' : 'triangle right-bottom',
        direction === 'right'
          ? ['right-justified', 'triangle left-top dark']
          : '',
      ]"
      :style="direction === 'right' ? { backgroundColor: '#ffffff' } : {}"
    >
      <div class="talktext">
        <p
          :style="
            direction === 'right' ? { color: '#363636' } : { color: '#ffffff' }
          "
          style="font-size: 0.75rem; padding: 2vh"
        >
          <slot></slot>
        </p>
      </div>
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
.container {
  display: flex;
  flex-direction: row;
  width: 100%;
}
.neobrutalism-message {
  width: fit-content;
  max-width: 50vw;
  height: fit-content;
  margin: 1.5vh;
  display: flex;
  flex-direction: row;
  position: relative;
  height: auto;
  background-color: #363636;
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
  border-color: #363636 transparent transparent transparent;
}

.triangle.right-bottom.dark::after {
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

.right-justified {
  margin-left: auto;
}
</style>
