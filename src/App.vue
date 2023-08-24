<template>
  <fullscreen-block :color="'#3b71ee'">
    <p class="brutalism-underlined">Приветственная страница</p>
    <sparkle-pile :number="8"></sparkle-pile>
    <sparkle-pile :number="5" style="right: 0; top: 55%"></sparkle-pile>
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
        Это мой сайт в стиле
        <h style="font-weight: bold">нео-брутализм!</h>
        <p style="font-size: 0.5em; font-style: italic">Не судите строго :)</p>
      </div>
      <div
        class="brutalism-style"
        style="border-bottom-left-radius: 35px; border-top-right-radius: 35px"
      >
        Тут будут:
        <ul style="font-size: 0.5em">
          <li>&bull; Мои фотки в старших классах и в унике!</li>
          <li>&bull; История о том как я полюбил программирование👨‍💻</li>
          <li style="display: flex">
            &bull;&nbsp;
            <p style="text-decoration: line-through">Надеюсь</p>
            &nbsp;крутая css фишка!
          </li>
          <li style="display: flex">
            &bull; Парадокс на&nbsp;
            <p style="color: #000000; background-color: #f7df1e; back">
              JavaScript
            </p>
            &nbsp;и задание по теме 🐐🚪🏎️
          </li>
          <li>&bull; Мои контакты, ссылки на репозитории и тому подобное👾</li>
        </ul>
      </div>
    </div>
    <img
      src="./assets/memes.webp"
      style="position: absolute; left: 84%; height: 20em; top: 66%"
    />
  </fullscreen-block>
  <fullscreen-block :color="'#fc724c'" style="display: flex">
    <img
      src="./assets/dashed.svg"
      style="position: relative; width: 45vw; display: flex; margin: 0 auto"
    />
    <sparkle-pile :number="3" style="top: 150%"></sparkle-pile>
    <sparkle-pile :number="8" style="right: 0; top: 100%"></sparkle-pile>
    <p class="brutalism-underlined">Страница с фотками</p>
  </fullscreen-block>
  <fullscreen-block :color="'#fccb4c'"
    ><p class="brutalism-underlined">
      История о том как я полюбил программирование
    </p></fullscreen-block
  >
  <fullscreen-block :color="'#3b71ee'"
    ><p class="brutalism-underlined">Фишка в css</p></fullscreen-block
  >
  <fullscreen-block :color="'#fc724c'"
    ><p class="brutalism-underlined">
      Парадокс на JavaScript
    </p></fullscreen-block
  >
  <fullscreen-block :color="'#fccb4c'"
    ><p class="brutalism-underlined">Мои контакты</p></fullscreen-block
  >
  <fullscreen-block :color="'#3b71ee'"
    ><p class="brutalism-underlined">Задание 2 - Блок 1</p></fullscreen-block
  >
  <fullscreen-block :color="'#fc724c'"
    ><p class="brutalism-underlined">Задание 2 - Блок 2</p></fullscreen-block
  >
  <fullscreen-block :color="'#fccb4c'"
    ><p class="brutalism-underlined">Задание 2 - Блок 3</p></fullscreen-block
  >
  <fullscreen-block
    class="brutalism-footer"
    :color="'#282828'"
    style="color: white"
  >
    <button v-on:click="moveToBlock('block1')">Приветственная страница</button>
    <button v-on:click="moveToBlock('block2')">Страница с фотками</button>
    <button v-on:click="moveToBlock('block3')">Фишка в css</button>
    <button v-on:click="moveToBlock('block4')">Мои контакты</button>
    <button v-on:click="moveToBlock('block5')">Задание 2 - Блок 1</button>
    <button v-on:click="moveToBlock('block6')">Задание 2 - Блок 2</button>
    <button v-on:click="moveToBlock('block7')">Задание 2 - Блок 3</button>
  </fullscreen-block>
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
  methods: {
    moveToBlock(blockId) {
      const blockElement = document.getElementById(blockId);

      if (blockElement) {
        blockElement.scrollIntoView({ behavior: "smooth" });
      }
    },
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

.brutalism-underlined {
  font-family: "Space Grotesk";
  font-size: 1.5em;
  color: #282828 !important;
  font-weight: bold;
  font-family: monospace;
  text-decoration: underline;
  position: absolute;
  right: 0;
  padding: 1em;
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

.brutalism-footer {
  height: 30vh;
  padding: 2em;
  font-size: 1.5em;
  font-family: monospace;
}
</style>
