<template>
  <section class="section-grid">
    <h1 class="section-grid__title">About Me</h1>
    <div class="section-grid__content">
      <p>
        Lorem ipsum dolor sit amet, consectetur adipiscing elit. Praesent libero mauris, hendrerit
        non dapibus aliquet.<br />
        <br />
        Lorem ipsum dolor sit amet, consectetur adipiscing elit. Praesent libero mauris, hendrerit
        non dapibus aliquet, scelerisque at magna. Nulla euismod est eleifend, egestas ligula sit
        amet, lobortis nulla. Nam vel urna rhoncus, ultricies ante nec, feugiat libero. Vestibulum
        porttitor fermentum lectus eu volutpat. In sit amet tempor arcu. Vivamus lacus lorem,
        vulputate a purus sed, sollicitudin imperdiet justo. Donec ex urna, maximus eget massa quis,
        vehicula pharetra diam. Aenean id nulla tellus. <br />
        <br />
        Lorem ipsum dolor sit amet, consectetur adipiscing elit. Praesent libero mauris, hendrerit
        non dapibus aliquet. <br />
        <br />
        Lorem ipsum dolor sit amet, consectetur adipiscing elit. Praesent libero mauris, hendrerit
        non dapibus aliquet, scelerisque at magna. Nulla euismod est eleifend, egestas ligula sit
        amet, lobortis nulla. Nam vel urna rhoncus, ultricies ante nec, feugiat libero. Vestibulum
        porttitor fermentum lectus eu volutpat. In sit amet tempor arcu. Vivamus lacus lorem,
        vulputate a purus sed, sollicitudin imperdiet justo. Donec ex urna, maximus eget massa quis,
        vehicula pharetra diam. Aenean id nulla tellus.
      </p>
    </div>
  </section>
</template>

<style lang="scss" scoped>
.section-grid {
  display: grid;
  grid-template-columns: 30% 1fr 20%;
  grid-template-rows: 300px auto 1fr;
  min-height: 100vh;

  &__title {
    grid-column-start: 2;
    grid-row-start: 2;
  }

  &__content {
    grid-column-start: 2;
    grid-row-start: 3;
    margin: 150px 0 0 0;
    display: flex;
    flex-flow: column nowrap;
    row-gap: 150px;
  }
}
</style>
