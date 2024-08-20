<template>
  <section class="section-grid" id="about-section">
    <div class="section-grid__title">
      <h1>
        A Little <br />
        About Me
      </h1>
      <img class="line-image" src="../assets/imgs/about-me.png" alt="circle over about me" />
    </div>
    <div class="section-grid__content">
      <div class="content-item">
        <p>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit. Praesent libero mauris, hendrerit
          non dapibus aliquet, scelerisque at magna. Nulla euismod est eleifend, egestas ligula sit
          amet, lobortis nulla. Nam vel urna rhoncus, ultricies ante nec, feugiat libero. <br />
        </p>
      </div>
      <div class="content-item">
        <p>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit. Praesent libero mauris, hendrerit
          non dapibus aliquet, scelerisque at magna. Nulla euismod est eleifend, egestas ligula sit
          amet, lobortis nulla. Nam vel urna rhoncus, ultricies ante nec, feugiat libero. Vestibulum
          porttitor fermentum lectus eu volutpat. In sit amet tempor arcu. Vivamus lacus lorem,
          vulputate a purus sed, sollicitudin imperdiet justo. Donec ex urna, maximus eget massa
          quis, vehicula pharetra diam. Aenean id nulla tellus. <br />
        </p>
      </div>
      <div class="content-item">
        <p>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit. Praesent libero mauris, hendrerit
          non dapibus aliquet, scelerisque at magna. Nulla euismod est eleifend, egestas ligula sit
          amet, lobortis nulla. Nam vel urna rhoncus, ultricies ante nec, feugiat libero. <br />
        </p>
      </div>
    </div>
  </section>
</template>

<style lang="scss" scoped>
.line-image {
  width: 100%;
}

@media (min-width: 1024px) {
  .line-image {
    width: 450px;
    transform: translateX(-30px) translateY(60px);
    position: absolute;
  }
}
</style>
