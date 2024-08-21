<template>
  <section class="landing-grid">
    <div class="landing-grid__title">
      <h1>Embracing Design for Humans, Robots & AI</h1>
    </div>
    <div class="landing-grid__content">
      <div class="content-item">
        <h2>UI Designer & User Researcher</h2>
      </div>
    </div>
  </section>
</template>

<style lang="scss" scoped>
.line-image {
  width: 700px;
  transform: translateX(-80px) translateY(-230px);
  position: absolute;
}

.landing-grid {
  display: grid;
  grid-template-columns: 5% 1fr 5%;
  grid-template-rows: 200px auto 100px 1fr 100px;
  min-height: 100vh;

  &__title {
    grid-column: 2;
    grid-row-start: 3;
  }

  &__content {
    grid-column: 2;
    grid-row-start: 4;
    width: 200px;

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
  }
}

@media (min-width: 1024px) {
  .landing-grid {
    display: grid;
    grid-template-columns: 10% 1fr 10%;
    grid-template-rows: 250px auto 100px 1fr 200px;
    min-height: 100vh;

    &__title {
      grid-column: 2;
      grid-row: 2;
    }

    &__content {
      grid-column: 2;
      grid-row-start: 4;
      width: 100%;

      .content-item {
        display: flex;
        flex-flow: column nowrap;
        justify-content: start;
        align-items: center;
      }
    }
    .image-container {
      position: absolute;
      right: calc(30% + 350px + 100px);
      grid-column: 2;
      grid-row: 3 / span 3;
      align-self: end;
    }
  }
}
</style>
