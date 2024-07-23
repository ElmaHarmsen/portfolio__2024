<template>
  <section class="section-grid">
    <div class="section-grid__title">
      <h1>A Little About Me</h1>
      <img class="line-image" src="../assets/imgs/circle-2.png" alt="" />
    </div>
    <div class="section-grid__content">
      <div class="content-item">
        <h2 class="content-item__heading">smth</h2>
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
        <h2 class="content-item__heading">smth</h2>
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
  width: 300px;
  transform: translateX(-90px) translateY(-50px);
  position: absolute;
}
</style>
