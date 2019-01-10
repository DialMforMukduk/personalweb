<template>
  <section class="container-fluid">
    <div>
      <logo />
      <h1 class="title">
        Contact
      </h1>
      <div class="row justify-content-left">
        <div
          class="col-7 mx-auto"
        >
          <div class="content">
            <form
              name="contact"
              action="/thank-you"
              netlify-honeypot="bot-field"
              method="post"
              netlify
            >
              <input
                type="hidden"
                name="form-name"
                value="contact"
              >
              <p class="hidden">
                <label>
                  Don’t fill this out:
                  <input name="bot-field">
                </label>
              </p>
              <label
                class="form-label"
                for="name"
              >
                Name:
              </label><br>
              <input
                id="name"
                class="form-field"
                name="name"
              ><br>
              <label
                class="form-label"
                for="email"
              >
                Email:
              </label><br>
              <input
                id="email"
                class="form-field"
                name="email"
              ><br>
              <label
                class="form-label"
                for="message"
              >
                Message:
              </label><br>
              <textarea
                id="message"
                class="form-field"
                name="message"
                rows="3"
              /><br>
              <input
                class="form-button"
                type="submit"
                value="Send message"
              >
            </form>
          </div>
        </div>
      </div>
      <div class="links">
        <a
          href="https://twitter.com/DialMforMukduk"
          target="_blank"
        >
          <img
            src="~assets/Twitter_Social_Icon_Circle_Color.png"
            alt="Twitter"
            style="width:6.5%;height:6.5%;border:0;"
          >
        </a>
        <a
          href="https://github.com/DialMforMukduk"
          target="_blank"
        >
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
import Logo from "~/components/Logo.vue";

export default {
  components: {
    Logo
  }
};
</script>

<style>
.container-fluid {
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
  background-image: url("~assets/background.jpg");
  background-repeat: repeat;
}

.title {
  font-family: "Montserrat", sans-serif;
  display: block;
  font-size: 7vw;
  font-weight: bold;
  color: black;
  letter-spacing: 0.01vw;
}

.subtitle {
  font-family: "Montserrat", sans-serif;
  font-weight: 425;
  font-size: 3.75vw;
  color: black;
  letter-spacing: 0.01vw;
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

.hidden {
  display: none;
}

textarea {
  width: 100%;
}

</style>
