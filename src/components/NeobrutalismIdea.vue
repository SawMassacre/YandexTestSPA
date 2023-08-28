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
  padding: 1rem;
  border: 5px dashed #fc724c;
  margin: 0.8rem;
}

.idea-pros {
  list-style-type: square;
  font-size: 0.7rem;
}
.idea-title {
  font-size: 1.75rem;
  margin-bottom: 0.6rem;
}

.idea-description {
  margin-bottom: 0.75em;
  font-size: 0.9rem;
}
</style>
