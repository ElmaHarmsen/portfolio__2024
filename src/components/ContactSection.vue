<template>
  <section class="section-grid">
    <div class="section-grid__title">
      <h1>Say Hello</h1>
      <img class="line-image" src="../assets/imgs/ooo.png" alt="" />
    </div>
    <div class="section-grid__content">
      <div class="content-item">
        <p>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit. Praesent libero mauris, hendrerit
          non dapibus aliquet, scelerisque at magna. Nulla euismod est eleifend, egestas ligula sit
          amet, lobortis nulla.
        </p>
      </div>
      <div class="content-item">
        <a href="https://www.linkedin.com/in/elma-harmsen/" target="_blank">
          <h2>linkedin/elma-harmsen</h2>
        </a>
        <a href="https://github.com/ElmaHarmsen" target="_blank">
          <h2>github/ElmaHarmsen</h2>
        </a>
        <h2>drive.google/Resume</h2>
        <h2>elmaharmsen01@gmail.com</h2>
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
</style>
