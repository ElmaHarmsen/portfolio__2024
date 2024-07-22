<template>
  <section class="section-grid">
    <div class="section-grid__title">
      <h1>Robot/AI Research</h1>
    </div>
    <div class="section-grid__content">
      <div class="content-item">
        <img
          class="content-item__image"
          src="../assets/imgs/RobotScene1.png"
          alt="Daily UI #27 Gradient picker dropdown"
        />
      </div>
      <div class="content-item">
        <h2>Paragraph Title</h2>
        <p>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit. Praesent libero mauris, hendrerit
          non dapibus aliquet, scelerisque at magna. Nulla euismod est eleifend, egestas ligula sit
          amet, lobortis nulla. Nam vel urna rhoncus, ultricies ante nec, feugiat libero. Vestibulum
          porttitor fermentum lectus eu volutpat. In sit amet tempor arcu. Vivamus lacus lorem,
          vulputate a purus sed, sollicitudin imperdiet justo. Donec ex urna, maximus eget massa
          quis, vehicula pharetra diam. Aenean id nulla tellus.
        </p>
      </div>
      <div class="content-item">
        <img
          class="content-item__image"
          src="../assets/imgs/RobotScene3.png"
          alt="Daily UI #27 Gradient picker dropdown"
        />
      </div>
      <div class="content-item">
        <h2>Paragraph Title</h2>
        <p>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit. Praesent libero mauris, hendrerit
          non dapibus aliquet, scelerisque at magna. Nulla euismod est eleifend, egestas ligula sit
          amet, lobortis nulla. Nam vel urna rhoncus, ultricies ante nec, feugiat libero. Vestibulum
          porttitor fermentum lectus eu volutpat. In sit amet tempor arcu. Vivamus lacus lorem,
          vulputate a purus sed, sollicitudin imperdiet justo. Donec ex urna, maximus eget massa
          quis, vehicula pharetra diam. Aenean id nulla tellus.
        </p>
      </div>
      <div class="content-item">
        <img
          class="content-item__image"
          src="../assets/imgs/RobotScene4.png"
          alt="Daily UI #27 Gradient picker dropdown"
        />
      </div>
      <div class="content-item">
        <h2>Paragraph Title</h2>
        <p>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit. Praesent libero mauris, hendrerit
          non dapibus aliquet, scelerisque at magna. Nulla euismod est eleifend, egestas ligula sit
          amet, lobortis nulla. Nam vel urna rhoncus, ultricies ante nec, feugiat libero. Vestibulum
          porttitor fermentum lectus eu volutpat. In sit amet tempor arcu. Vivamus lacus lorem,
          vulputate a purus sed, sollicitudin imperdiet justo. Donec ex urna, maximus eget massa
          quis, vehicula pharetra diam. Aenean id nulla tellus.
        </p>
      </div>
      <div class="content-item">
        <img
          class="content-item__image"
          src="../assets/imgs/AIScene1.png"
          alt="Daily UI #27 Gradient picker dropdown"
        />
      </div>
    </div>
  </section>
</template>

<style lang="scss" scoped>
.section-grid {
  display: grid;
  grid-template-columns: 30% 1fr 15%;
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

    .content-item {
      display: flex;
      flex-flow: column nowrap;
      row-gap: 30px;

      &__image {
        width: 500px;
        box-shadow: rgba(0, 0, 0, 0.15) 0px 5px 15px 0px;
      }
    }
  }
}
</style>
