<template>
  <section class="landing-grid">
    <div class="landing-grid__title">
      <h1>My Recent Work</h1>
    </div>
    <div class="landing-grid__content">
      <div class="content-item">
        <h2>Daily UI Challenges</h2>
        <h2>UX Team Project</h2>
        <h2>Robot-AI Research</h2>
      </div>
    </div>
  </section>
</template>

<style lang="scss" scoped>
.landing-grid {
  display: grid;
  grid-template-columns: 5% 1fr 30%;
  grid-template-rows: 150px auto 150px 1fr 40px;
  height: 100vh;

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
      row-gap: 40px;
      justify-content: end;
      height: 100%;

      p {
        text-align: justify;
        background-color: var(--bg-white);
      }
    }
  }
}
</style>
