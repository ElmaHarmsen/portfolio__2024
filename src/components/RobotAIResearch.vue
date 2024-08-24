<template>
  <section class="section-grid" id="research-section">
    <div class="section-grid__content">
      <div class="content-item">
        <h1>
          Robot-AI <br />
          Research
        </h1>
      </div>
    </div>
    <div class="section-grid__content container">
      <div class="content-item">
        <p class="p-1">
          Lorem ipsum dolor sit amet, consectetur adipiscing elit. Praesent libero mauris, hendrerit
          non dapibus aliquet, scelerisque at magna. Nulla euismod est eleifend, egestas ligula sit
          amet, lobortis nulla. Nam vel urna rhoncus, ultricies ante nec, feugiat libero. Vestibulum
          porttitor fermentum lectus eu volutpat. In sit amet tempor arcu. Vivamus lacus lorem,
          vulputate a purus sed, sollicitudin imperdiet justo. Donec ex urna, maximus eget massa
          quis, vehicula pharetra diam. Aenean id nulla tellus.
        </p>
      </div>
      <div class="content-item image-grid">
        <img
          class="content-item__image"
          src="../assets/imgs/RobotScene1.png"
          alt="Daily UI #27 Gradient picker dropdown"
        />
        <img
          class="content-item__image"
          src="../assets/imgs/RobotScene3.png"
          alt="Daily UI #27 Gradient picker dropdown"
        />
        <img
          class="content-item__image"
          src="../assets/imgs/RobotScene4.png"
          alt="Daily UI #27 Gradient picker dropdown"
        />
      </div>
      <div class="content-item">
        <p class="p-2">
          Lorem ipsum dolor sit amet, consectetur adipiscing elit. Praesent libero mauris, hendrerit
          non dapibus aliquet, scelerisque at magna. Nulla euismod est eleifend, egestas ligula sit
          amet, lobortis nulla. Nam vel urna rhoncus, ultricies ante nec, feugiat libero. Vestibulum
          porttitor fermentum lectus eu volutpat. In sit amet tempor arcu. Vivamus lacus lorem,
          vulputate a purus sed, sollicitudin imperdiet justo. Donec ex urna, maximus eget massa
          quis, vehicula pharetra diam. Aenean id nulla tellus.
        </p>
        <p class="p-3">
          Lorem ipsum dolor sit amet, consectetur adipiscing elit. Praesent libero mauris, hendrerit
          non dapibus aliquet, scelerisque at magna. Nulla euismod est eleifend, egestas ligula sit
          amet, lobortis nulla. Nam vel urna rhoncus, ultricies ante nec, feugiat libero. Vestibulum
          porttitor fermentum lectus eu volutpat. In sit amet tempor arcu. Vivamus lacus lorem,
          vulputate a purus sed, sollicitudin imperdiet justo. Donec ex urna, maximus eget massa
          quis, vehicula pharetra diam. Aenean id nulla tellus.
        </p>
      </div>
    </div>
  </section>
</template>

<style lang="scss" scoped>
.section-grid {
  grid-template-rows: 8rem calc(100vh - (2 * 8rem)) 8rem 1fr 8rem;

  &__content {
    align-self: flex-end;
  }

  .container {
    grid-row: 4;
    row-gap: 8rem;

    .content-item {
      display: flex;
      flex-flow: column nowrap;
      row-gap: 8rem;

      .p-1 {
        width: 40%;
      }
      .p-2 {
        width: 65%;
      }
      .p-3 {
        width: 45%;
      }

      &__image {
        width: 100%;
        border: 0.5rem solid black;
      }
    }

    .image-grid {
      display: grid;
      grid-template-columns: 1fr 1fr 1fr;
      grid-template-rows: 1fr;
      gap: 1rem;
    }
  }
}
</style>
