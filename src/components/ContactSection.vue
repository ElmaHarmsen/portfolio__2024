<template>
  <section class="section-grid" id="contact-section">
    <div class="section-grid__title">
      <h1>Say Hello</h1>
      <img class="say-hello-image" src="../assets/imgs/say-hello.png" alt="" />
    </div>
    <div class="section-grid__content">
      <div class="content-item">
        <p>
          When our paths cross, then let us say <span class="italic-text">hello</span>. <br />
          I am looking for new opportunities
        </p>
      </div>
      <div class="content-item">
        <a href="https://www.linkedin.com/in/elma-harmsen/" target="_blank">
          <div class="content-item__container">
            <img class="line-image" src="../assets/imgs/contact-links.png" alt="" />
            <p>linkedin/elma-harmsen</p>
          </div>
        </a>
        <a href="https://github.com/ElmaHarmsen" target="_blank">
          <div class="content-item__container">
            <img class="line-image" src="../assets/imgs/contact-links.png" alt="" />
            <p>github/ElmaHarmsen</p>
          </div>
        </a>
        <div class="content-item__container">
          <img class="line-image" src="../assets/imgs/contact-links.png" alt="" />
          <p>drive.google/Resume</p>
        </div>
        <div class="content-item__container">
          <img class="line-image" src="../assets/imgs/contact-links.png" alt="" />
          <p>elmaharmsen01@gmail.com</p>
        </div>
        <br />
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

.content-item {
  &__container {
    display: flex;
    flex-flow: column nowrap;
  }
}
</style>
