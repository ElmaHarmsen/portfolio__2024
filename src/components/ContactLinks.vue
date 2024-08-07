<template>
  <section class="section-grid">
    <div class="section-grid__content">
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

.content-item {
  display: flex;
  flex-flow: column nowrap;
  justify-content: flex-end;
  height: 100%;

  &__container {
    display: flex;
    flex-flow: column nowrap;
  }
}
</style>
