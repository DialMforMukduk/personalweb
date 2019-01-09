<template>
  <div class="VueToNuxtLogo">
    <nuxt-link to="/">
      <div class="Triangle">
        <img src="~assets/me.jpeg">
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
  height: 180px;
  width: 245px;
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
