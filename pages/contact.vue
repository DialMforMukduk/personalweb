<template>
  <section class="container-fluid">
    <div>
      <logo />
      <div class="row">
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
              <p class="title">
                Contact Me
              </p>
              <input
                id="name"
                class="form-field rounded"
                name="name"
                placeholder="Name"
              ><br><br>
              <input
                id="email"
                class="form-field rounded"
                name="email"
                placeholder="Email"
              ><br><br>
              <textarea
                id="message"
                class="form-field rounded"
                name="message"
                rows="3"
                placeholder="Message"
              /><br>
              <input
                class="form-button rounded"
                type="submit"
                value="Send message"
              >
            </form><br>
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
  font-size: 3vw;
  color: black;
  letter-spacing: 0.01vw;
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
  text-align: center;
}

#email {
  width: 50%;
  text-align: center;
}

#name {
  width: 35%;
  text-align: center;
}

.col-7 {
  border-radius: 1vw;
  background-color: rgba(131, 139, 139, .9);
  border-color: black;
  border-width: .1vw;
  border-style: solid;
}

</style>
