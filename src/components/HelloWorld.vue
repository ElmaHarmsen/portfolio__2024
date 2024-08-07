<template>
  <section class="landing-grid">
    <div class="landing-grid__title">
      <h1>
        Designing <br />
        Human-Centred
      </h1>
      <img class="line-image" src="../assets/imgs/hello-world.png" alt="" />
    </div>
    <div class="landing-grid__content">
      <div class="content-item">
        <p>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit. Praesent libero mauris, hendrerit
          non dapibus aliquet, scelerisque at magna. Nulla euismod est eleifend, egestas ligula sit
          amet, lobortis nulla. Nam vel urna rhoncus, ultricies ante nec.
        </p>
        <p>Elma H.</p>
      </div>
    </div>
  </section>
</template>

<style lang="scss" scoped>
.line-image {
  width: 700px;
  transform: translateX(-80px) translateY(-215px);
  position: absolute;
}

.landing-grid {
  display: grid;
  grid-template-columns: 35% 1fr 5%;
  grid-template-rows: 150px auto 150px 1fr 100px;
  min-height: 100vh;

  &__title {
    grid-column: 2;
    grid-row-start: 2;
  }

  &__content {
    grid-column: 2;
    grid-row-start: 4;
    width: 350px;

    .content-item {
      display: flex;
      flex-flow: column nowrap;
      justify-content: end;
      row-gap: 30px;
      height: 100%;
    }
  }
  .image-container {
    position: absolute;
    right: calc(30% + 350px + 100px);
    grid-column: 2;
    grid-row: 3 / span 3;
    align-self: end;

    &__figure {
      height: 350px;
      grid-column-start: 2;
    }
  }
}
</style>
