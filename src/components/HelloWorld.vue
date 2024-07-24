<template>
  <section class="landing-grid">
    <div class="landing-grid__title">
      <h1>
        Designing <br />
        Human-Centred
      </h1>
      <img class="line-image" src="../assets/imgs/under-line-1.png" alt="" />
    </div>
    <div class="landing-grid__content">
      <div class="content-item">
        <h2>Because we're all Human</h2>
        <p>Elma H.</p>
      </div>
    </div>
    <div class="image-container">
      <img
        class="image-container__figure"
        src="../assets/imgs/stick-figure-4.png"
        alt="hand-drawn stick figure"
      />
    </div>
  </section>
</template>

<style lang="scss" scoped>
.line-image {
  width: 300px;
  transform: translateX(-635px) translateY(-30px);
  position: absolute;
}

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
      row-gap: 30px;
      height: 100%;

      p {
        text-align: justify;
        background-color: var(--bg-white);
      }
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
