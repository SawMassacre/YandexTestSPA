<template>
  <fullscreen-block :color="'#3b71ee'">
    <img
      src="./assets/memes.webp"
      style="position: absolute; left: 84%; height: 20em; top: 66%"
    />
    <sparkle-pile :number="7"></sparkle-pile>
    <div
      class="brutalism-style"
      style="
        padding: 0.5em;
        z-index: 10;
        opacity: 0.7;
        top: 25%;
        left: 4%;
        border-radius: 20px;
        border-width: 2px;
      "
    >
      <p style="font-size: 0.3em; font-style: italic">
        Звездочки генерируются рандомно,<br />
        если они лежат некрасиво - <br />
        перезагрузите страницу (пожалуйста)
      </p>
    </div>
    <img
      src="./assets/git.webp"
      style="position: absolute; left: 0%; height: 20em; top: 0%"
    />
    <div id="container-greeting">
      <div
        class="brutalism-style"
        style="border-top-left-radius: 35px; border-bottom-right-radius: 35px"
      >
        👋Привет меня зовут Женя!
      </div>
      <div class="brutalism-style">
        Это мой сайт в стиле нео-брутализма!
        <p style="font-size: 0.5em; font-style: italic">Не судите строго :)</p>
      </div>
      <div
        class="brutalism-style"
        style="border-bottom-left-radius: 35px; border-top-right-radius: 35px"
      >
        Далее будут:
        <ul style="font-size: 0.5em">
          <li>&bull; Я в старших классах и в унике!</li>
          <li>&bull; История о том как я полюбил программирование👨‍💻</li>
          <li style="display: flex">
            &bull;&nbsp;
            <p style="text-decoration: line-through">Надеюсь</p>
            &nbsp;крутая css фишка!
          </li>
          <li>&bull; Парадокс на JS🐐🚪🏎️</li>
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
import SparklePile from "./components/SparklePile.vue";

export default {
  name: "App",
  components: {
    FullscreenBlock,
    SparklePile,
  },
};
</script>

<style>
@import url("https://fonts.googleapis.com/css?family=Space+Grotesk");

body {
  font-weight: 400;
  font-family: "Space Grotesk";
  color: #282828 !important;
  overflow-x: hidden;
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
