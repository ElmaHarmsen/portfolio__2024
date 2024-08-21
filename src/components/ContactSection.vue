<template>
  <section class="footer-grid" id="contact-section">
    <div class="footer-grid__title">
      <h1>Say Hello</h1>
      <!-- <img
        class="say-hello-image"
        src="../assets/imgs/say-hello.png"
        alt="squigly line under say hello"
      /> -->
    </div>
    <div class="footer-grid__content">
      <div class="content-item">
        <!-- <a href="https://www.linkedin.com/in/elma-harmsen/" target="_blank">
          <div class="container">
            <img class="line-image" src="../assets/imgs/contact-links.png" alt="list item line" />
            <p>linkedin/elma-harmsen</p>
          </div>
        </a>
        <a
          href="https://drive.google.com/file/d/1UZjNtQ9nmxyYSvrw8UkutdDfxknvxHN2/view?usp=sharing"
          target="_blank"
        >
          <div class="container">
            <img class="line-image" src="../assets/imgs/contact-links.png" alt="list item line" />
            <p>drive.google/resume</p>
          </div>
        </a> -->
        <div class="container">
          <p>elmaharmsen01@gmail.com</p>
        </div>
      </div>
    </div>
  </section>
</template>

<style lang="scss" scoped>
.line-image {
  width: 20px;
  // transform: translateX(-50px) translateY(10px);
  // position: absolute;
}

.say-hello-image {
  width: 100%;
  // transform: translateX(-15px) translateY(80px);
  // position: absolute;
}

.footer-grid {
  display: grid;
  grid-template-columns: 15% 1fr 15%;
  grid-template-rows: 150px auto 150px 1fr 150px;

  &__content {
    grid-column: 2;
    grid-row-start: 2;

    .container {
      display: flex;
      flex-flow: column nowrap;
      row-gap: 10px;
    }
  }
}

@media (min-width: 1024px) {
  .line-image {
    width: 30px;
    transform: translateX(-50px) translateY(10px);
    position: absolute;
  }

  .say-hello-image {
    width: 450px;
    transform: translateX(20px) translateY(90px);
    position: absolute;
  }

  .footer-grid {
    display: grid;
    grid-template-columns: 10% 1fr 10%;
    grid-template-rows: 200px auto 50px 1fr 200px;
    min-height: 100vh;

    &__title {
      grid-column: 2;
      grid-row-start: 2;
    }

    &__content {
      grid-column: 2;
      grid-row-start: 4;

      .container {
        display: flex;
        flex-flow: column nowrap;
      }
    }
  }
}
</style>
