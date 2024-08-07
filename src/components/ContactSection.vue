<template>
  <section class="footer-grid" id="contact-section">
    <div class="section-grid__title">
      <h1>Say Hello</h1>
      <img
        class="say-hello-image"
        src="../assets/imgs/say-hello.png"
        alt="squigly line under say hello"
      />
    </div>
    <div class="section-grid__content item-offset">
      <div class="content-item">
        <a href="https://www.linkedin.com/in/elma-harmsen/" target="_blank">
          <div class="container">
            <img class="line-image" src="../assets/imgs/contact-links.png" alt="list item line" />
            <p>linkedin/elma-harmsen</p>
          </div>
        </a>
        <a href="https://github.com/ElmaHarmsen" target="_blank">
          <div class="container">
            <img class="line-image" src="../assets/imgs/contact-links.png" alt="list item line" />
            <p>github/ElmaHarmsen</p>
          </div>
        </a>
        <div class="container">
          <img class="line-image" src="../assets/imgs/contact-links.png" alt="list item line" />
          <p>drive.google/Resume</p>
        </div>
        <div class="container">
          <img class="line-image" src="../assets/imgs/contact-links.png" alt="list item line" />
          <p>elmaharmsen01@gmail.com</p>
        </div>
      </div>
    </div>
  </section>
</template>

<style lang="scss" scoped>
.line-image {
  width: 30px;
  transform: translateX(-50px) translateY(10px);
  position: absolute;
}

.say-hello-image {
  width: 350px;
  transform: translateX(-15px) translateY(80px);
  position: absolute;
}

.footer-grid {
  display: grid;
  grid-template-columns: 35% 1fr 5%;
  grid-template-rows: 150px auto 250px 1fr 150px;

  &__content {
    grid-column: 2;
    grid-row-start: 2;

    .container {
      display: flex;
      flex-flow: column nowrap;
    }
  }

  .item-offset {
    transform: translateX(50px);
  }
}
</style>
