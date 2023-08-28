<template>
  <div>
    <loading-screen v-if="isLoading"></loading-screen>
    <div v-else>
      <fullscreen-block :color="'#3b71ee'" id="block1" style="display: block">
        <p class="brutalism-underlined">Приветственная страница</p>
        <sparkle-pile :number="6"></sparkle-pile>
        <sparkle-pile :number="5" style="right: 0; top: 55%"></sparkle-pile>
        <div
          class="animate__animated animate__bounceInLeft animate__delay-2s"
          style="
            border: 0.15rem solid black;
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
            @load="onImgLoad"
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
            border-radius: 15px;
            border-width: 2px;
          "
        >
          <p style="font-size: 0.7em; font-style: italic">
            Звездочки генерируются рандомно,<br />
            если они лежат некрасиво - <br />
            перезагрузите страницу (пожалуйста)
          </p>
        </div>
        <img
          class="animate__animated animate__bounceIn animate__delay-1s"
          ref="myElement"
          src="./assets/git.webp"
          style="position: absolute; left: 0%; height: 15em; top: 0%"
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
            <p style="font-size: 0.5em; font-style: italic">
              Не судите строго :)
            </p>
          </div>
          <div
            class="brutalism-style"
            style="
              border-bottom-left-radius: 35px;
              border-top-right-radius: 35px;
            "
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
                &bull; История про&nbsp;
                <p style="color: #000000; background-color: #f7df1e; back">
                  JavaScript
                </p>
                <p style="font-style: italic">(задание со звездочкой)</p>
              </li>
              <li>
                &bull; Мои контакты, ссылки на репозитории и тому подобное👾
              </li>
              <li>&bull; Задание 2💬</li>
            </ul>
          </div>
        </div>
        <img
          class="animate__animated animate__bounceIn animate__delay-1s"
          src="./assets/memes.webp"
          style="position: absolute; left: 84%; height: 15em; top: 66%"
        />
      </fullscreen-block>
      <fullscreen-block
        :color="'#fc724c'"
        id="block2"
        style="
          display: flex;
          opacity: 1;
          background-image: radial-gradient(#363636 1px, transparent 1px),
            radial-gradient(#363636 1px, #fc724c 1px);
          background-size: 40px 40px;
          background-position: 0 0, 20px 20px;
        "
      >
        <sparkle-pile :number="7" style="top: 150%"></sparkle-pile>
        <sparkle-pile :number="3" style="right: 0; top: 100%"></sparkle-pile>
        <div
          data-aos="zoom-in"
          style="
            transform: rotate(-7deg);
            border: 0.15rem solid black;
            height: 52%;
            border-radius: 30px;
            box-shadow: 5px 5px 0px 0px black;
            overflow: hidden;
            position: absolute;
            margin-top: 15%;
            left: 12%;
            width: fit-content;
          "
        >
          <img
            src="./assets/MeSchool.jpg"
            style="position: absolute; height: 100%; position</div>: relative"
          />
        </div>
        <img
          data-aos="zoom-out-left"
          src="./assets/plenty.webp"
          style="
            height: 15em;
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
            border: 0.15rem solid black;
            height: 57%;
            border-radius: 25px;
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
            margin-top: 11%;
            right: 22%;
            border-radius: 10px;
            border-width: 2px;
          "
        >
          <p style="font-size: 0.8rem">Недавнее фото с дня рождения</p>
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
            left: 16%;
            border-radius: 10px;
            border-width: 2px;
          "
        >
          <p style="font-size: 0.8rem">
            Фото в середине лета перед университетом
          </p>
        </div>
        <img
          data-aos="zoom-out-down"
          class="animate__animated animate__pulse animate__infinite"
          src="./assets/dashed.svg"
          style="position: relative; width: 35vw; display: flex; margin: 0 auto"
        />
        <p class="brutalism-underlined">Страница с фотками</p>
      </fullscreen-block>
      <fullscreen-block :color="'#fccb4c'" id="block3"
        ><p class="brutalism-underlined">История о программировании</p>
        <sparkle-pile :number="6"></sparkle-pile>
        <sparkle-pile
          :number="6"
          style="right: 0; margin-top: 25%"
        ></sparkle-pile>
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
              text-align: center;
              display: flex;
              flex-direction: column;
              justify-content: space-evenly;
              height: 70%;
              font-size: 0.9rem;
            "
          >
            <div
              class="brutalism-style"
              style="margin: 0 auto; width: 90%; border-radius: 20px 0px"
              data-aos="zoom-out-down"
            >
              В школе я хотел стать юристом🎓, но когда пришла пора сдавать
              экзамены я
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
              На курсах по подготовке мне посоветовали сдавать на плюсах🫡🫡🫡
              <br />
              но я на удивление хорошо справлялся...
            </div>
            <div
              class="brutalism-style"
              style="margin: 0 auto; width: 60%; border-radius: 10px"
              data-aos="zoom-out-left"
            >
              Поступил в ДВФУ, страдал с математикой, познал основы, начал
              проходить стажировки и далее далее
            </div>
            <div
              class="brutalism-style"
              style="margin: 0 auto; width: 90%; border-radius: 20px 0px"
              data-aos="zoom-out-up"
            >
              Но программирование я правда <strong>полюбил</strong> когда
              однажды понял - с ним ты свободен:
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
      <fullscreen-block
        :color="'#3b71ee'"
        id="block4"
        style="
          opacity: 1;
          background-image: linear-gradient(#363636 1px, transparent 1px),
            linear-gradient(to right, #363636 1px, #3b71ee 1px);
          background-size: 20px 20px;
        "
        ><p class="brutalism-underlined">Фишка в css</p>
      </fullscreen-block>
      <fullscreen-block :color="'#fc724c'" id="block5"
        ><p class="brutalism-underlined">История про JavaScript</p>
        <sparkle-pile :number="6"></sparkle-pile>
        <sparkle-pile :number="6" style="right: 0"></sparkle-pile>
        <div
          style="
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100%;
            flex-direction: column;
          "
        >
          <div
            class="brutalism-style"
            style="
              margin: 0 auto;
              width: fit-content;
              border-radius: 10px;
              border-style: ridge;
              border-width: 7px;
              border-color: #363636;
              width: 45rem;
              margin-bottom: 1rem;
            "
            data-aos="zoom-in"
          >
            На первом курсе университета я не знал толком ничего кроме основ
            с++, но под конец года нам дали курсовую: создать сайт с
            использованием библиотеки ThreeJS. Когда я приступил к заданию
            оказалось что библиотека довольно простая в использовании. Надо было
            взять откуда то вдохновение и подглядеть реализацию, в этом помогли
            сайты с примерами работ. Когда я увидел <strong>что</strong> можно
            сделать с помощью этой библиотеки я был поражен. <br />
            <br />
            Преподаватели были крайне добрые и ставили всем поголовно пятерки,
            но тем не менее мне было интересно заниматься проектом больше
            нужного. Сейчас он мне не кажется таким крутым как раньше :) Но мне
            кажется увидеть примеры работ и возможности джаваскрипта и сторонних
            библиотек нужно, чтобы понять что
            <strong>реализовать можно всё</strong>.
          </div>
          <div
            data-aos="zoom-in"
            style="
          border-style: ridge;
          border-width: 7px;
          border
          border-color: #363636;
          width: 45rem;
          border-radius: 10px;
          overflow: hidden;
          margin: 0 auto;
        "
          >
            <img
              src="./assets/demo.jpg"
              style="position: absolute; height: 100%; position: relative"
            />
          </div>
          <img
            ref="myElement"
            data-aos="zoom-out-right"
            src="./assets/fight.webp"
            style="
              right: 0%;
              height: 14em;
              margin-top: 7vh;
              transform: rotate(-15deg);
              margin-right: 4vh;
              position: absolute;
            "
          />
          <div
            class="brutalism-style"
            style="
              margin: 0 auto;
              width: fit-content;
              border-radius: 10px;
              border-style: ridge;
              border-width: 7px;
              border-color: #363636;
              width: 45rem;
              margin-top: 1rem;
            "
            data-aos="zoom-in"
          >
            Выше - моя работа. А вот ниже будет то, что может вдохновлять по
            настоящему. Я предлагаю посмотреть на примеры, а затем попробовать
            реализовать что нибудь!
          </div>
        </div>
      </fullscreen-block>
      <fullscreen-block
        class="brutalism-footer"
        :color="'#363636'"
        style="
          color: white;
          padding: 1.5vh;
          display: flex;
          justify-content: center;
          font-size: 1rem;
        "
      >
        <p data-aos="fade-in">
          <strong
            >↓ Примеры внизу!
            <span style="font-style: italic"
              >(надеюсь не сильно нагружают комп...)</span
            >
            ↓</strong
          >
        </p>
      </fullscreen-block>
      <iframe
        ref="iframe"
        src="https://0x.se/"
        width="100%"
        height="550px"
        scrolling="yes"
      ></iframe>
      <iframe
        ref="iframe"
        src="https://jesse-zhou.com/"
        width="100%"
        height="550px"
        scrolling="yes"
      ></iframe>
      <fullscreen-block
        :color="'#fccb4c'"
        id="block6"
        style="
          opacity: 1;
          background-image: linear-gradient(#363636 1px, transparent 1px),
            linear-gradient(to right, #363636 1px, #fccb4c 1px);
          background-size: 20px 20px;
        "
      >
        <sparkle-pile :number="6"></sparkle-pile>
        <sparkle-pile :number="6" style="right: 0"></sparkle-pile>
        <p class="brutalism-underlined">Мои контакты</p>

        <div style="display: grid; place-items: center; height: 100%">
          <div
            style="
              display: flex;
              flex-direction: column;
              align-items: center;
              justify-content: center;
            "
          >
            <a href="https://t.me/sawmassacre">
              <button class="neobrutalism-button" data-aos="zoom-in">
                Telegram
              </button>
            </a>
            <a href="https://github.com/SawMassacre">
              <button class="neobrutalism-button" data-aos="zoom-in">
                Github
              </button>
            </a>
            <a href="https://github.com/SawMassacre/YandexTestSPA">
              <button class="neobrutalism-button" data-aos="zoom-in">
                Репозиторий
                <p style="font-size: 0.25em; font-style: italic">
                  (Ссылка на этот проект)
                </p>
              </button>
            </a>
            <div
              data-aos="zoom-in"
              style="
                background-color: #363636;
                border: 0.15rem solid black;
                box-shadow: 10px 10px 0px 0px black;
                margin-top: 2vh;
              "
            >
              <img src="./assets/devRush.gif" style="height: 13rem" />
            </div>
          </div>
        </div>
      </fullscreen-block>
      <fullscreen-block
        class="brutalism-footer"
        :color="'#363636'"
        style="
          color: white;
          padding: 1.5vh;
          display: flex;
          justify-content: center;
          font-size: 1rem;
        "
      >
        <p data-aos="fade-in">
          <strong>↓ Отсюда начинается второе задание ↓</strong>
        </p>
      </fullscreen-block>
      <fullscreen-block :color="'#3b71ee'" id="block7"
        ><p class="brutalism-underlined">Задание 2 - Блок 1</p>
        <sparkle-pile :number="10"></sparkle-pile>
        <sparkle-pile
          :number="8"
          style="margin-top: 25%; right: 0"
        ></sparkle-pile>
        <img
          ref="myElement"
          data-aos="zoom-out-right"
          src="./assets/emo.webp"
          style="
            left: 0%;
            height: 13em;
            margin-top: 7vh;
            transform: rotate(-15deg);
            margin-left: 1.5vw;
            position: absolute;
          "
        />
        <div
          class="message-container"
          style="
            display: flex;
            flex-direction: column;
            justify-content: center;
            height: 100vh;
            margin-left: 15%;
            margin-right: 15%;
          "
        >
          <neobrutalism-message direction="left" data-aos="zoom-in-right">
            🥱 Этот курс совсем для новичков, он таким до конца и будет или мы
            будем делать что-то поинтереснее?
          </neobrutalism-message>
          <neobrutalism-message direction="right" data-aos="zoom-in-left">
            <strong>
              Привет, я уверен далее в курсе найдется то, что будет для тебя в
              новинку! Если ты опережаешь программу то могу порекомендовать
              материал для изучения вне рамок курса. Например можешь
              ознакомиться с typescript, на курсе его всё равно не будет, так
              что потом тебе не будет скучно!
            </strong>
          </neobrutalism-message>
          <neobrutalism-message direction="left" data-aos="zoom-in-right">
            😟 Я ничего не успеваю, успел только один урок посмотреть, а на
            практику времени не хватает(((
          </neobrutalism-message>
          <neobrutalism-message direction="right" data-aos="zoom-in-left">
            <strong>
              Я понимаю насколько неприятно догонять, но нельзя сильно
              расстраиваться. У тебя все еще есть время выполнить часть заданий,
              это уже лучше чем сдаться. Сделай все что можешь и ты рано или
              поздно догонишь! Если совсем не можешь посмотреть уроки, то прочти
              конспекты:
              <a
                href="https://www.youtube.com/watch?v=m6pE8psWJXE"
                style="color: #fc724c"
                >вродессылка.com</a
              >.
            </strong>
          </neobrutalism-message>
          <neobrutalism-message direction="left" data-aos="zoom-in-right">
            😵‍💫 Я пропустила вебинар и теперь ничего вообще не понимаю, что
            происходит
          </neobrutalism-message>
          <neobrutalism-message direction="right" data-aos="zoom-in-left">
            <strong>
              Без паники, всё можно посмотреть в записи. Ставь на 1.5х и успеешь
              и посмотреть и сделать! Если совсем не успеваешь то прочти
              материал в pdf, ставь на 2х и решай фоном, лучше сделать что-то,
              чем ничего! Запись тут:
              <a
                href="https://www.youtube.com/watch?v=m6pE8psWJXE"
                style="color: #fc724c"
                >типассылка.com</a
              >, а пдфка лежит тут:
              <a
                href="https://www.youtube.com/watch?v=m6pE8psWJXE"
                style="color: #fc724c"
                >тожессылка.com.</a
              >
            </strong>
          </neobrutalism-message>
          <neobrutalism-message direction="left" data-aos="zoom-in-right">
            🙄 Вот на этой странице на платформе /скрин/ 3я картинка ну вообще
            не к месту( Да и вообще дизайн странноватый…
          </neobrutalism-message>
          <neobrutalism-message direction="right" data-aos="zoom-in-left">
            <strong
              >Ты можешь скачать аддон для браузера и накинуть свои стили на
              сайт, как раз опробуешь знания на практике! А поводу картинки: она
              кажется тебе отталкивающей/оскорбительной или просто не нравится с
              точки зрения дизайна??
            </strong>
          </neobrutalism-message>
        </div>
      </fullscreen-block>
      <fullscreen-block :color="'#fc724c'" id="block8"
        ><p class="brutalism-underlined">Задание 2 - Блок 2</p>
        <sparkle-pile :number="10"></sparkle-pile>
        <sparkle-pile
          :number="8"
          style="margin-top: 25%; right: 0"
        ></sparkle-pile>
        <img
          ref="myElement"
          data-aos="zoom-out-left"
          src="./assets/agile.webp"
          style="
            right: 0%;
            height: 15em;
            margin-top: 7vh;
            margin-right: 4vw;
            position: absolute;
          "
        />
        <div
          style="
            display: flex;
            justify-content: center;
            flex-direction: column;
            align-items: center;
            height: 100%;
          "
        >
          <neobrutalism-idea style="width: 60%">
            <template v-slot:title>
              <h2>Идеи для пет-проектов</h2>
            </template>

            <template v-slot:description>
              <p>
                Можно предложить обсудить какой личный проект хотели бы сделать
                ребята. Предложить набор тем, затем обсудить реализацию,
                привести примеры из личного опыта.
              </p>
            </template>

            <template v-slot:pros>
              <li>
                &bull; Может вызвать бурное обсуждение если у кого-то совпадут
                идеи.
              </li>
              <li>&bull; Может возникнуть кооперация между учениками.</li>
              <li>&bull; Может замотивировать развиваться вне рамок курса.</li>
            </template>
          </neobrutalism-idea>
          <neobrutalism-idea style="width: 60%">
            <template v-slot:title>
              <h2>Обсудить недавно просмотренное/любимое</h2>
            </template>

            <template v-slot:description>
              <p>
                Можно обсудить любимые фильмы , сериалы, книги, музыку,
                приложения, сайты и так далее.
              </p>
            </template>

            <template v-slot:pros>
              <li>&bull; Точно вызывает обсуждение.</li>
              <li>
                &bull; Дает почувствовать связь с курсом не только в учебном
                плане.
              </li>
              <li>&bull; Привлекает внимание к чату.</li>
              <li>
                &bull; Участвовать в обсуждении могут все, а не только
                прошаренные в программировании (как в других идеях).
              </li>
            </template>
          </neobrutalism-idea>
          <neobrutalism-idea style="width: 60%">
            <template v-slot:title>
              <h2>
                Можно скидывать недавно просмотренные видео по популярному
                программированию/новым технологиям
              </h2>
            </template>

            <template v-slot:description>
              <p>
                Допустим вышла новая библиотека и ее быстрый обзор. Можно
                скинуть ссылку в чат и обсудить, объяснить в чем крутость или
                наоборот недостатки.
              </p>
            </template>

            <template v-slot:pros>
              <li>&bull; Дополняет знания курса.</li>
              <li>
                &bull; Дает материал для изучения тем, кто идет быстрее (см.
                Блок - 1).
              </li>
              <li>&bull; Показывает обширность изучаемой темы.</li>
            </template>
          </neobrutalism-idea>
        </div>
      </fullscreen-block>
      <fullscreen-block
        :color="'#fccb4c'"
        id="block9"
        style="
          opacity: 1;
          background-image: radial-gradient(#363636 1px, transparent 1px),
            radial-gradient(#363636 1px, #fccb4c 1px);
          background-size: 40px 40px;
          background-position: 0 0, 20px 20px;
        "
      >
        <p class="brutalism-underlined">Задание 2 - Блок 3</p>
        <sparkle-pile
          :number="10"
          style="margin-top: 25%; left: 0"
        ></sparkle-pile>
        <sparkle-pile :number="8" style="right: 0"></sparkle-pile>
        <div
          style="
            display: flex;
            flex-direction: row;
            align-items: center;
            justify-content: center;
            height: 100%;
          "
        >
          <div
            data-aos="fade-right"
            style="
              background-color: #363636;
              border: 0.15rem solid black;
              box-shadow: 10px 10px 0px 0px black;
              display: flex;
              justify-content: center;
              align-items: center;
              width: 13rem;
              height: 13rem;
            "
          >
            <div style="height: 100%; width: 100%">
              <img
                src="./assets/devDeadline.gif"
                style="width: 100%; object-fit: contain"
              />
            </div>
          </div>
          <div
            data-aos="fade-left"
            style="
              background-color: #363636;
              border: 0.15rem solid black;
              font-family: monospace;
              padding: 1.5rem;
              font-size: 1rem;
              height: 13rem;
              width: 55rem;
              margin-left: 1.5rem;
              color: #ffffff;
              box-shadow: 10px 10px 0px 0px black;
            "
          >
            <span style="color: #fc724c">@all</span> Ребята, напоминаю что срок
            сдачи практического задания истекает сегодня! В этот раз сдало
            маловато людей - у кого проблемы пишите мне в ЛС. Если задание
            кажется вам слишком сложным то пожалуйста напишите с чем возникают
            сложности, главное не молчите. Я думаю вы не отвечаете потому, что
            боитесь спросить - так делать не надо. Вы тут чтобы спрашивать!!!
            <br /><br />
            И еще вот что: сдавать задания это не всегда о знаниях, иногда надо
            сдать даже не до конца сделанную работу, главное сдайте. Дисциплина
            так же важна как и знания!
          </div>
        </div>
      </fullscreen-block>
      <fullscreen-block
        class="brutalism-footer"
        :color="'#363636'"
        style="color: white"
      >
        <div style="display: flex; height: 100%">
          <ul class="footer-list" style="text-align: right">
            <li>
              <button v-on:click="moveToBlock('block1')">
                Приветственная страница
              </button>
            </li>
            <li>
              <button v-on:click="moveToBlock('block2')">
                Страница с фотками
              </button>
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
                История про JavaScript
              </button>
            </li>
            <li>
              <button v-on:click="moveToBlock('block6')">Мои контакты</button>
            </li>
            <li>
              <button v-on:click="moveToBlock('block7')">
                Задание 2 - Блок 1
              </button>
            </li>
            <li>
              <button v-on:click="moveToBlock('block8')">
                Задание 2 - Блок 2
              </button>
            </li>
            <li>
              <button v-on:click="moveToBlock('block9')">
                Задание 2 - Блок 3
              </button>
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
                font-size: 7.5rem;
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
                border: 0.15rem solid black;
              "
            >
              <p style="font-size: 1.25rem; padding: 0.3em; color: #000000">
                Если хотите взглянуть ещё раз!
              </p>
            </div>
            <img
              src="./assets/devShocked.gif"
              style="height: 12em; padding-left: 2vw"
            />
          </div>
        </div>
        <p style="position: absolute; right: 1em">𝗰𝗼𝗱𝗲𝗺𝗮𝘀𝘀𝗮𝗰𝗿𝗲 𝟮𝟬𝟮𝟯</p>
      </fullscreen-block>
    </div>
  </div>
</template>

<script>
import NeobrutalismMessage from "./components/NeobrutalismMessage.vue";
import FullscreenBlock from "./components/FullscreenBlock.vue";
import NeobrutalismIdea from "./components/NeobrutalismIdea.vue";
import SparklePile from "./components/SparklePile.vue";
import LoadingScreen from "./components/LoadingScreen.vue";
import "animate.css";
import "aos/dist/aos.css";
import AOS from "aos";

AOS.init({
  delay: 200,
  duration: 700,
});

export default {
  name: "App",
  components: {
    FullscreenBlock,
    SparklePile,
    NeobrutalismMessage,
    NeobrutalismIdea,
    LoadingScreen,
  },
  methods: {
    onImgLoad() {
      this.isLoading = false;
    },
    moveToBlock(blockId) {
      const blockElement = document.getElementById(blockId);

      if (blockElement) {
        blockElement.scrollIntoView({ behavior: "smooth" });
      }
    },
  },
  data() {
    return {
      isLoading: true,
    };
  },
  mounted() {
    this.isLoading = false;
  },
};
</script>

<style>
body {
  font-weight: 400;
  color: #363636 !important;
  overflow-x: hidden;
  background-color: #363636;
}

.neobrutalism-button {
  font-family: monospace;
  margin: 2vh;
  background-color: #363636;
  color: #ffffff;
  border: none;
  padding: 10px 20px;
  text-align: center;
  text-decoration: none;
  height: fit-content;
  display: inline-block;
  border: 0.15rem solid black;
  font-size: 3rem;
  box-shadow: 10px 10px 0px 0px black;
  cursor: pointer;
}

.neobrutalism-button:hover {
  background-color: #fccb4c;
  color: #363636;
}

.brutalism-style {
  position: relative;
  width: fit-content;
  font-family: monospace;
  color: black;
  background-color: white;
  padding: 1em;
  border: 0.15rem solid black;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-rendering: optimizeLegibility;
}

.brutalism-underlined {
  font-size: 1.5em;
  color: #363636 !important;
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
  left: 47%;
  font-size: 1.7rem;
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
  color: #363636;
  padding: 10px 20px;
  text-align: center;
  text-decoration: none;
  display: inline-block;
  font-size: 0.755rem;
  border-radius: 10px;
  cursor: pointer;
  border: 0.15rem solid black;
}

.footer-list button:hover {
  background-color: #363636;
  border-color: #ffffff;
  color: #ffffff;
}
</style>
