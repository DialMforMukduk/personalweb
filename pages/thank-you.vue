<template>
  <section class="container-fluid">
    <div class="content">
      <h1 class="title">
        Thank you
      </h1>
      <p class="text-center">
        <nuxt-link to="home">
          back home
        </nuxt-link>
      </p>
    </div>
  </section>
</template>

<style>
.container-fluid {
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
  background-image: url('~assets/background.jpg');
  background-repeat: repeat;
  background-size: contain;
}
</style>
