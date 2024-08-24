<template>
  <section class="landing-grid">
    <div class="landing-grid__content">
      <div class="content-item">
        <h1>Embracing Design for Humans, Robots & AI</h1>
        <div class="subitems-container">
          <h2>Elma Harmsen</h2>
          <h2>
            UI/UX Designer & <br class="phone-only" />
            User Researcher
          </h2>
        </div>
      </div>
    </div>
    <div class="circle-element"></div>
  </section>
</template>

<style lang="scss" scoped>
.landing-grid {
  display: grid;
  grid-template-columns: 2rem calc(100% - (2 * 2rem)) 2rem;
  grid-template-rows: 8rem 1fr 8rem;
  min-height: 100vh;

  &__content {
    grid-column: 2;
    grid-row: 2;
    width: 100%;
    display: flex;
    flex-flow: column nowrap;
    justify-content: end;

    .content-item {
      display: flex;
      flex-flow: column nowrap;
      row-gap: 2.5rem;
      justify-content: start;
    }

    .subitems-container {
      display: flex;
      flex-flow: column nowrap;
      row-gap: 2rem;
      justify-content: start;
      padding: 0 0.25rem;
    }
  }
}

.circle-element {
  background: radial-gradient(ellipse at top right, #ff9a44, transparent),
    radial-gradient(circle at bottom left, #fc6076, transparent);
  opacity: 0.95;
  width: 400px;
  height: 400px;
  border-radius: 300px 250px 300px 250px;
  filter: blur(70px);
  position: absolute;
  z-index: -1;
  bottom: 5.5rem;
  left: 1%;
}

@media (min-width: 1024px) {
  .landing-grid {
    grid-template-columns: 10% 1fr 10%;

    &__content {
      padding: 2.5rem;

      .subitems-container {
        flex-flow: row nowrap;
        column-gap: 5rem;
      }
    }
  }

  .circle-element {
    width: 600px;
    height: 600px;
    border-radius: 300px 400px 300px 400px;
    filter: blur(90px);
    bottom: 1.5rem;
    left: 20%;
  }
}
</style>
