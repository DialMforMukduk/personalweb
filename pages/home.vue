<template>
  <section class="container-fluid">
    <div>
      <h1 class="title">
        Jared Carpenter
      </h1>
      <h2 class="subtitle">
        Web dev
      </h2>
      <logo />
      <div class="links">
        <a href="https://twitter.com/DialMforMukduk">
          <img
            src="~assets/Twitter_Social_Icon_Circle_Color.png"
            alt="Twitter"
            style="width:6.5%;height:6.5%;border:0;"
          >
        </a>
        <a href="https://github.com/DialMforMukduk">
          <img
            src="~assets/GitHub-Mark-120px-plus.png"
            alt="Github"
            style="width:6.5%;height:6.5%;border:0;"
          >
        </a>
        <nuxt-link to="/contact">
          <img
            src="~assets/emailme.png"
            alt="Email"
            style="width:6.5%;height:6.5%;border:0;"
          >
        </nuxt-link>
      </div>
    </div>
  </section>
</template>

<script>
import Logo from '~/components/Logo.vue'

export default {
  components: {
    Logo
  }
}
</script>

<style>

.container-fluid {
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
  background-image: url('~assets/background.jpg');
  background-repeat: repeat;
}

.title {
    font-family: 'Montserrat', sans-serif;
    display: block;
    font-size: 7vw;
    font-weight: bold;
    color: black;
    letter-spacing: .01vw;
  }

  .subtitle {
    font-family: 'Montserrat', sans-serif;
    font-weight: 425;
    font-size: 3.75vw;
    color: black;
    letter-spacing: .01vw;
    padding-top: 0vw;
  }

.links {
  padding-top: 15px;
}

img {
    max-width: 100%;
    height: auto;
    width: auto\9; /* ie8 */
}

</style>
