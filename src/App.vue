<template>
  <fullscreen-block :color="'#3b71ee'">
    <div id="container-greeting">
      <div class="brutalism-style">👋Привет меня зовут Женя!</div>
      <div class="brutalism-style">
        Это мой сайт в стиле нео-брутализма!
        <p style="font-size: 0.5em; font-style: italic">Не судите строго :)</p>
      </div>
      <div class="brutalism-style">
        Далее будут:
        <ul style="font-size: 0.5em">
          <li>&bull; Я в старших классах и в унике!</li>
          <li>&bull; История о том как я полюбил программирование👨‍💻</li>
          <li style="display: flex">
            &bull;&nbsp;
            <p style="text-decoration: line-through">Надеюсь</p>
            &nbsp;крутая css фишка!
          </li>
          <li>&bull; Мои контакты, ссылки на репозитории и тому подобное👾</li>
        </ul>
      </div>
    </div>
  </fullscreen-block>
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

<style>
@import url("https://fonts.googleapis.com/css?family=Space+Grotesk");

body {
  font-weight: 400;
  font-family: "Space Grotesk";
  color: #282828 !important;
}

.brutalism-style {
  position: relative;
  width: fit-content;
  font-family: monospace;
  font-size: 3em;
  color: black;
  background-color: white;
  padding: 1em;
  border: 3px solid black;
}

#container-greeting {
  position: relative;
  top: 30%;
  left: 50%;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  height: 55vh;
}
</style>
