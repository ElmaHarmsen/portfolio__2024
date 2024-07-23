<template>
  <section class="landing-grid">
    <div class="landing-grid__title">
      <h1>
        Designing <br />
        Human Centred
      </h1>
      <!-- <h2>{{ subHeading }}</h2> -->
    </div>
    <div class="landing-grid__content">
      <div class="content-item">
        <p>
          Introducing an interaction designer and user experience researcher. I am specialised in
          the researching, designing and evaluating of many kinds of human-computer based
          interactions and human-centred technologies.
        </p>
        <h2>Because we're all Human</h2>
      </div>
    </div>
    <div class="image-container">
      <img
        class="image-container__figure"
        src="../assets/imgs/stickyfig.png"
        alt="hand-drawn stick figure"
      />
    </div>
  </section>
</template>

<style lang="scss" scoped>
.landing-grid {
  display: grid;
  grid-template-columns: 5% 1fr 30%;
  grid-template-rows: 150px auto 150px 1fr 40px;
  min-height: 100vh;

  &__title {
    grid-column: 2;
    justify-self: end;
    grid-row-start: 2;
    text-align: right;
  }

  &__content {
    grid-column: 2;
    grid-row-start: 4;
    justify-self: end;
    width: 350px;

    .content-item {
      display: flex;
      flex-flow: column nowrap;
      justify-content: space-between;
      height: 100%;

      p {
        text-align: justify;
        background-color: var(--bg-white);
      }
    }
  }
  .image-container {
    grid-column: 2;
    grid-row: 3 / span 2;
    justify-self: start;
    align-self: end;

    &__figure {
      height: 500px;
      grid-column-start: 2;
    }
  }
}
</style>
