<template>
  <section class="section-grid">
    <div class="section-grid__title">
      <h1>Say Hello</h1>
      <img class="line-image" src="../assets/imgs/ooo.png" alt="" />
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
            <img class="long-image" src="../assets/imgs/long-line-1.png" alt="" />
            <h2>linkedin/elma-harmsen</h2>
          </div>
        </a>
        <a href="https://github.com/ElmaHarmsen" target="_blank">
          <div class="content-item__container">
            <img class="long-image" src="../assets/imgs/long-line-2.png" alt="" />
            <h2>github/ElmaHarmsen</h2>
          </div>
        </a>
        <div class="content-item__container">
          <img class="long-image" src="../assets/imgs/long-line-3.png" alt="" />
          <h2>drive.google/Resume</h2>
        </div>
        <div class="content-item__container">
          <img class="long-image" src="../assets/imgs/long-line-4.png" alt="" />
          <h2>elmaharmsen01@gmail.com</h2>
        </div>
        <br />
      </div>
    </div>
  </section>
</template>

<style lang="scss" scoped>
.line-image {
  width: 150px;
  transform: translateX(150px) translateY(5px);
  position: absolute;
}

.content-item {
  &__container {
    display: flex;
    flex-flow: column nowrap;

    .long-image {
      position: absolute;
      z-index: 1;
      right: 0;
      width: calc(30% + 350px);
      height: 30px;
      transform: translateY(5px);
    }
  }
}
</style>
