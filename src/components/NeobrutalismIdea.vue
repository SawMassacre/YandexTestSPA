<template>
  <div class="brutalism-idea" data-aos="flip-up">
    <h2 class="idea-title">
      <slot name="title">Идея</slot>
    </h2>
    <p class="idea-description">
      <slot name="description">Описание</slot>
    </p>
    <ul class="idea-pros">
      <strong>Плюсы:</strong>
      <slot name="pros" class="idea-pro">
        <li>Плюс</li>
        <li>Плюс</li>
        <li>Плюс</li>
      </slot>
    </ul>
  </div>
</template>

<script>
export default {
  name: "BrutalismIdea",
};
</script>

<style scoped>
.brutalism-idea {
  background-color: #ffffff;
  color: #363636;
  font-family: monospace;
  padding: 1em;
  border: 5px dashed #fc724c;
  margin: 1vh;
}

.idea-pros {
  list-style-type: square;
  font-size: 1.5em;
}
.idea-title {
  font-size: 2.5em;
  margin-bottom: 0.5em;
}

.idea-description {
  margin-bottom: 0.75em;
  font-size: 1.8em;
}
</style>
