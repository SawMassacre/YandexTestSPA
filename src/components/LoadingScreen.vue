<template>
  <div
    style="
      background-color: #fc724c;
      height: 100vh;
      width: 100vw;
      background-color: #fc724c;
      opacity: 1;
      background-image: linear-gradient(#363636 2.7px, transparent 2.7px),
        linear-gradient(to right, #363636 2.7px, #3b71ee 2.7px);
      background-size: 54px 54px;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
    "
  >
    <div class="brutalism-style" style="font-size: 2rem">
      Мои фотки довольно много весят, подождите пожалуйста :)
    </div>
    <div class="brutalism-style" style="font-size: 2rem; margin-top: 2rem">
      <div class="lds-facebook">
        <div></div>
        <div></div>
        <div></div>
      </div>
    </div>
  </div>
</template>

<style>
.lds-facebook {
  display: inline-block;
  position: relative;
  width: 80px;
  height: 80px;
}
.lds-facebook div {
  display: inline-block;
  position: absolute;
  left: 8px;
  width: 16px;
  background: #3b71ee;
  animation: lds-facebook 1.2s cubic-bezier(0, 0.5, 0.5, 1) infinite;
}
.lds-facebook div:nth-child(1) {
  left: 8px;
  animation-delay: -0.24s;
}
.lds-facebook div:nth-child(2) {
  left: 32px;
  animation-delay: -0.12s;
}
.lds-facebook div:nth-child(3) {
  left: 56px;
  animation-delay: 0;
}
@keyframes lds-facebook {
  0% {
    top: 8px;
    height: 64px;
  }
  50%,
  100% {
    top: 24px;
    height: 32px;
  }
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
</style>
