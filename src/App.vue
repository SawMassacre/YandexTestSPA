<template>
  <fullscreen-block :color="'#3b71ee'" id="block1" style="display: block">
    <p class="brutalism-underlined">Приветственная страница</p>
    <sparkle-pile :number="6"></sparkle-pile>
    <sparkle-pile :number="5" style="right: 0; top: 55%"></sparkle-pile>
    <div
      class="animate__animated animate__bounceInLeft animate__delay-0.5s"
      style="
        border: 3px solid black;
        height: 95%;
        border-radius: 65px 0;
        box-shadow: 10px 10px 0px 0px black;
        overflow: hidden;
        position: absolute;
        margin-top: 1%;
        left: 30%;
        width: fit-content;
      "
    >
      <img
        src="./assets/Me.jpg"
        style="position: absolute; height: 100%; position: relative"
      />
    </div>
    <div
      class="brutalism-style animate__animated animate__bounceInLeft animate__delay-1s"
      style="
        padding: 0.5em;
        z-index: 10;
        opacity: 0.7 !important;
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
      class="animate__animated animate__bounceIn animate__delay-1s"
      ref="myElement"
      src="./assets/git.webp"
      style="position: absolute; left: 0%; height: 20em; top: 0%"
    />
    <div id="container-greeting">
      <div
        class="brutalism-style"
        style="
          border-top-left-radius: 35px;
          border-bottom-right-radius: 35px;
          display: flex;
        "
      >
        <p
          class="animate__animated animate__headShake animate__repeat-3 animate__delay-2s"
        >
          👋
        </p>
        Привет, меня зовут Женя!
      </div>
      <div class="brutalism-style">
        Это мой сайт в стиле
        <h style="font-weight: bold">необрутализм!</h>
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
            &nbsp;и задание по теме🐐🚪🏎️
          </li>
          <li>&bull; Мои контакты, ссылки на репозитории и тому подобное👾</li>
          <li>&bull; Задание 2💬</li>
        </ul>
      </div>
    </div>
    <img
      class="animate__animated animate__bounceIn animate__delay-1s"
      src="./assets/memes.webp"
      style="position: absolute; left: 84%; height: 20em; top: 66%"
    />
  </fullscreen-block>
  <fullscreen-block :color="'#fc724c'" style="display: flex" id="block2">
    <div
      data-aos="zoom-in"
      style="
        transform: rotate(-7deg);
        border: 3px solid black;
        height: 45%;
        border-radius: 45px 0;
        box-shadow: 5px 5px 0px 0px black;
        overflow: hidden;
        position: absolute;
        margin-top: 15%;
        left: 9%;
        width: fit-content;
      "
    >
      <img
        src="./assets/MeSchool.jpg"
        style="position: absolute; height: 100%; position: relative"
      />
    </div>
    <img
      data-aos="zoom-out-left"
      src="./assets/plenty.webp"
      style="
        height: 30vh;
        position: absolute;
        margin-top: 52vh;
        right: 7%;
        z-index: 10;
      "
    />
    <div
      data-aos="zoom-in"
      style="
        transform: rotate(6deg);
        border: 3px solid black;
        height: 52%;
        border-radius: 45px 0;
        box-shadow: 10px 10px 0px 0px black;
        overflow: hidden;
        position: absolute;
        margin-top: 8%;
        right: 11%;
        width: fit-content;
      "
    >
      <img
        src="./assets/MeUni.jpg"
        style="position: absolute; height: 100%; position: relative"
      />
    </div>
    <div
      class="brutalism-style"
      data-aos="zoom-out-left"
      style="
        padding: 0.5em;
        z-index: 10;
        position: absolute;
        height: fit-content;
        margin-top: 9%;
        right: 17%;
        border-radius: 20px;
        border-width: 2px;
      "
    >
      <p style="font-size: 0.3em; font-style: italic">
        Недавнее фото с дня рождения
      </p>
    </div>
    <div
      class="brutalism-style"
      data-aos="zoom-out-right"
      style="
        padding: 0.5em;
        z-index: 10;
        position: absolute;
        height: fit-content;
        margin-top: 18%;
        left: 17%;
        border-radius: 20px;
        border-width: 2px;
      "
    >
      <p style="font-size: 0.3em; font-style: italic">
        Фото в середине лета перед университетом
      </p>
    </div>
    <img
      data-aos="zoom-out-down"
      class="animate__animated animate__pulse animate__infinite"
      src="./assets/dashed.svg"
      style="position: relative; width: 45vw; display: flex; margin: 0 auto"
    />
    <sparkle-pile :number="3" style="top: 150%"></sparkle-pile>
    <sparkle-pile :number="3" style="right: 0; top: 100%"></sparkle-pile>
    <p class="brutalism-underlined">Страница с фотками</p>
  </fullscreen-block>
  <fullscreen-block :color="'#fccb4c'" id="block3"
    ><p class="brutalism-underlined">История о программировании</p>
    <img
      data-aos="zoom-out-right"
      src="./assets/way.webp"
      style="
        height: 35vh;
        padding-left: 14vw;
        position: absolute;
        margin-top: 4vh;
        z-index: 0;
      "
    />
    <sparkle-pile :number="6"></sparkle-pile>
    <sparkle-pile :number="6" style="right: 0; margin-top: 25%"></sparkle-pile>
    <div
      style="
        display: flex;
        align-items: center;
        justify-content: center;
        height: 100%;
      "
    >
      <div
        style="
          font-size: 0.5em;
          text-align: center;
          display: flex;
          flex-direction: column;
          justify-content: space-evenly;
          height: 70%;
        "
      >
        <div
          class="brutalism-style"
          style="margin: 0 auto; width: 90%; border-radius: 20px 0px"
          data-aos="zoom-out-down"
        >
          В школе я хотел стать юристом🎓, но когда пришла пора сдавать экзамены
          я
          <br />
          передумал и сел за математику с информатикой.
        </div>
        <div
          class="brutalism-style"
          style="margin: 0 auto; width: 60%; border-radius: 10px"
          data-aos="zoom-out-left"
        >
          В начале года я даже не знал как считать дискриминант!
        </div>
        <div
          class="brutalism-style"
          style="margin: 0 auto; width: 90%; border-radius: 20px 0px"
          data-aos="zoom-out-right"
        >
          На курсах по подготовке мне посоветовали сдавать на плюсах🫡🫡🫡 <br />
          но я на удивление хорошо справлялся...
        </div>
        <div
          class="brutalism-style"
          style="margin: 0 auto; width: 60%; border-radius: 10px"
          data-aos="zoom-out-left"
        >
          Поступил в ДВФУ, страдал с математикой, познал основы, начал проходить
          стажировки и далее далее
        </div>
        <div
          class="brutalism-style"
          style="margin: 0 auto; width: 90%; border-radius: 20px 0px"
          data-aos="zoom-out-up"
        >
          Но программирование я правда <strong>полюбил</strong> когда однажды
          понял - с ним ты свободен:
          <br />
          Можно найти работу в любой стране🌍
          <br />
          Можно придумать что-то совершенно новое💡
          <br />
          Можно бесконечно расти и учиться📚
          <br />
          А еще - не передать словами насколько это
          <strong>круто</strong> работать в команде!👥
          <p style="font-style: italic; font-size: 0.7em">
            Даже не знаю что бы я делал если бы занимался чем то другим
          </p>
        </div>
      </div>
    </div>
  </fullscreen-block>
  <fullscreen-block :color="'#3b71ee'" id="block4"
    ><p class="brutalism-underlined">Фишка в css</p></fullscreen-block
  >
  <fullscreen-block :color="'#fc724c'" id="block5"
    ><p class="brutalism-underlined">
      Парадокс на JavaScript
    </p></fullscreen-block
  >
  <fullscreen-block :color="'#fccb4c'" id="block6">
    <sparkle-pile :number="6"></sparkle-pile>
    <sparkle-pile :number="6" style="right: 0"></sparkle-pile>
    <p class="brutalism-underlined">Мои контакты</p>

    <div style="display: grid; place-items: center; height: 100%">
      <div style="display: flex; flex-direction: column; align-items: center">
        <button class="neobrutalism-button" data-aos="zoom-in">
          <a href="https://t.me/sawmassacre">Telegram</a>
        </button>
        <button class="neobrutalism-button" data-aos="zoom-in">
          <a href="https://github.com/SawMassacre">Github</a>
        </button>
        <button class="neobrutalism-button" data-aos="zoom-in">
          <a href="https://github.com/SawMassacre/YandexTestSPA"
            ><p style="font-size: 0.25em; font-style: italic">
              (Ссылка на этот проект)
            </p>
            Репозиторий</a
          >
        </button>
        <div
          data-aos="zoom-in"
          style="
            background-color: #282828;
            border: 3px solid black;
            box-shadow: 10px 10px 0px 0px black;
            margin-top: 2vh;
          "
        >
          <img src="./assets/devRush.gif" style="height: 25vh" />
        </div>
      </div>
    </div>
  </fullscreen-block>
  <fullscreen-block :color="'#3b71ee'" id="block7"
    ><p class="brutalism-underlined">Задание 2 - Блок 1</p></fullscreen-block
  >
  <fullscreen-block :color="'#fc724c'" id="block8"
    ><p class="brutalism-underlined">Задание 2 - Блок 2</p></fullscreen-block
  >
  <fullscreen-block :color="'#fccb4c'" id="block9"
    ><p class="brutalism-underlined">Задание 2 - Блок 3</p></fullscreen-block
  >
  <fullscreen-block
    class="brutalism-footer"
    :color="'#363636'"
    style="color: white"
  >
    <div style="display: flex">
      <ul class="footer-list" style="text-align: right">
        <li>
          <button v-on:click="moveToBlock('block1')">
            Приветственная страница
          </button>
        </li>
        <li>
          <button v-on:click="moveToBlock('block2')">Страница с фотками</button>
        </li>
        <li>
          <button v-on:click="moveToBlock('block3')">
            История о программировании
          </button>
        </li>
        <li>
          <button v-on:click="moveToBlock('block4')">Фишка в css</button>
        </li>
      </ul>
      <ul class="footer-list" style="padding-left: 2vw">
        <li>
          <button v-on:click="moveToBlock('block5')">
            Парадокс на JavaScript
          </button>
        </li>
        <li>
          <button v-on:click="moveToBlock('block6')">Мои контакты</button>
        </li>
        <li>
          <button v-on:click="moveToBlock('block7')">Задание 2 - Блок 1</button>
        </li>
        <li>
          <button v-on:click="moveToBlock('block8')">Задание 2 - Блок 2</button>
        </li>
        <li>
          <button v-on:click="moveToBlock('block9')">Задание 2 - Блок 3</button>
        </li>
      </ul>
      <div
        style="
          display: flex;
          flex-direction: row;
          justify-content: center;
          align-items: center;
        "
      >
        <p
          style="
            font-size: 8em;
            margin-bottom: 1.5vh;
            transform: scaleX(-1);
            -webkit-text-stroke: 3px black;
          "
        >
          〱
        </p>
        <div
          style="
            height: fit-content;
            width: fit-content;
            padding-left: 0.6vw;
            background-color: white;
            border-bottom-left-radius: 15px;
            border-top-left-radius: 15px;
            border: 3px solid black;
          "
        >
          <p style="font-size: 1.5em; padding: 0.3em; color: #000000">
            Если хотите взглянуть ещё раз!
          </p>
        </div>
        <img
          src="./assets/devShocked.gif"
          style="height: 25vh; padding-left: 2vw"
        />
      </div>
    </div>
    <p style="position: absolute; right: 1em">𝗰𝗼𝗱𝗲𝗺𝗮𝘀𝘀𝗮𝗰𝗿𝗲 𝟮𝟬𝟮𝟯</p>
  </fullscreen-block>
</template>

<script>
import FullscreenBlock from "./components/FullscreenBlock.vue";
import SparklePile from "./components/SparklePile.vue";
import "animate.css";
import "aos/dist/aos.css";
import AOS from "aos";

AOS.init({
  delay: 300,
  duration: 500,
});

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
body {
  font-weight: 400;
  color: #282828 !important;
  overflow-x: hidden;
}

.neobrutalism-button {
  font-family: monospace;
  margin: 2vh;
  background-color: #282828;
  color: #fccb4c;
  border: none;
  padding: 10px 20px;
  text-align: center;
  text-decoration: none;
  height: fit-content;
  display: inline-block;
  border: 3px solid black;
  font-size: 5em;
  box-shadow: 10px 10px 0px 0px black;
  cursor: pointer;
}

.neobrutalism-button:hover {
  background-color: #fccb4c;
  color: #282828;
}

a {
  color: white;
  text-decoration: none;
}

a:hover {
  color: #282828;
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
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-rendering: optimizeLegibility;
}

.brutalism-underlined {
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
  top: 25%;
  left: 50%;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  height: 60vh;
}

.brutalism-footer {
  height: fit-content;
  padding: 2em;
  font-size: 1.5em;
  font-family: monospace;
}

.footer-list {
  list-style: none;
  padding: 0;
}

.footer-list li {
  margin-bottom: 10px;
}

.footer-list button {
  background-color: #ffffff;
  border: none;
  font-family: monospace;
  color: #282828;
  padding: 10px 20px;
  text-align: center;
  text-decoration: none;
  display: inline-block;
  font-size: 16px;
  border-radius: 10px;
  cursor: pointer;
  border: 3px solid black;
}

.footer-list button:hover {
  background-color: #282828;
  border-color: #ffffff;
  color: #ffffff;
}
</style>
