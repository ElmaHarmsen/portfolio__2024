<template>
  <section class="landing-grid">
    <div class="landing-grid__title">
      <h1>
        Embracing Design for <br />
        Humans, Robots & AI
      </h1>
      <!-- <img
        class="line-image"
        src="../assets/imgs/hello-world.png"
        alt="circle over designing human-centred"
      /> -->
    </div>
    <div class="landing-grid__content">
      <div class="content-item">
        <p>Hi! My name is Elma. I am an User Interface Designer and User Researcher.</p>
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
    grid-template-columns: 5% 1fr 5% 1fr 5%;
    grid-template-rows: 200px auto 100px 1fr 100px;
    min-height: 100vh;

    &__title {
      grid-column: 2 / span 3;
      grid-row: 3;
    }

    &__content {
      grid-column: 4;
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
    }
  }
}
</style>
