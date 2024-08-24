<template>
  <section class="landing-grid">
    <div class="landing-grid__content">
      <div class="content-item">
        <h1>
          Designing <br />
          Human-Centred
        </h1>
        <div class="subitems-container">
          <h2>The full showcase of recent work</h2>
        </div>
      </div>
    </div>
  </section>
</template>

<style lang="scss" scoped>
@media (min-width: 1024px) {
  .circle-element {
    background: radial-gradient(ellipse at top right, #ff9a44, transparent),
      radial-gradient(circle at bottom left, #fc6076, transparent);
    opacity: 0.95;
    width: 600px;
    height: 600px;
    border-radius: 300px 400px 300px 400px;
    filter: blur(90px);
    position: absolute;
    z-index: -1;
    bottom: 1.5rem;
    left: 20%;
  }

  .landing-grid {
    display: grid;
    grid-template-columns: 10% 1fr 10%;
    grid-template-rows: 8rem 1fr 8rem;
    min-height: 100vh;

    &__content {
      grid-column: 2;
      grid-row: 2;
      width: 100%;
      display: flex;
      flex-flow: column nowrap;
      justify-content: end;
      padding: 2.5rem;

      .content-item {
        display: flex;
        flex-flow: column nowrap;
        row-gap: 2.5rem;
        justify-content: start;
      }

      .header-container {
        display: flex;
        flex-flow: row nowrap;
        justify-content: space-between;
      }

      .subitems-container {
        display: flex;
        flex-flow: row nowrap;
        column-gap: 5rem;
        justify-content: start;
        padding: 0 0.25rem;
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
