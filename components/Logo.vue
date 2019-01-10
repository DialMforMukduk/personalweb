<template>
  <div class="VueToNuxtLogo">
    <nuxt-link to="/home">
      <div class="Triangle">
        <img src="~assets/JCwebdev.png">
      </div>
    </nuxt-link>
  </div>
</template>

<style>
.VueToNuxtLogo {
  display: inline-block;
  animation: turn 2s linear forwards 1s;
  transform: rotateX(180deg);
  position: relative;
  overflow: hidden;
  height: 100%;
  width: 100%;
  border-width: 3em;
  border-color: black;
}


@keyframes turn {
  100% {
    transform: rotateX(0deg);
  }
}

@keyframes godown {
  100% {
    top: 180px;
  }
}

@keyframes goright {
  100% {
    left: 70px;
  }
}
</style>
