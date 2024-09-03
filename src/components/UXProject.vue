<template>
  <section class="section-grid" id="ux-project-section">
    <div class="section-grid__content">
      <div class="content-item">
        <h1>
          The UX <br />
          Case
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
      <div class="content-item image-grid">
        <div class="container">
          <img
            class="content-item__image"
            src="../assets/imgs/UXProject1.png"
            alt="Daily UI #27 Gradient picker dropdown"
          />
          <h2>description</h2>
        </div>
        <div class="container">
          <img
            class="content-item__image"
            src="../assets/imgs/UXProject1.png"
            alt="Daily UI #27 Gradient picker dropdown"
          />
          <h2>description</h2>
        </div>
        <div class="container">
          <img
            class="content-item__image"
            src="../assets/imgs/UXProject1.png"
            alt="Daily UI #27 Gradient picker dropdown"
          />
          <h2>description</h2>
        </div>
      </div>
      <div class="content-item">
        <p class="p-4">
          Lorem ipsum dolor sit amet, consectetur adipiscing elit. Praesent libero mauris, hendrerit
          non dapibus aliquet, scelerisque at magna. Nulla euismod est eleifend, egestas ligula sit
          amet, lobortis nulla. Nam vel urna rhoncus, ultricies ante nec, feugiat libero. Vestibulum
          porttitor fermentum lectus eu volutpat. In sit amet tempor arcu. Vivamus lacus lorem,
          vulputate a purus sed, sollicitudin imperdiet justo. Donec ex urna, maximus eget massa
          quis, vehicula pharetra diam. Aenean id nulla tellus.
        </p>
      </div>
    </div>
    <div class="circle-element circle-1"></div>
    <div class="circle-element circle-2"></div>
  </section>
</template>

<style lang="scss" scoped>
.section-grid {
  grid-template-rows: 8rem calc(100vh - (2 * 8rem)) 8rem 1fr 8rem;

  &__content {
    align-self: flex-end;

    .content-item {
      display: flex;
      flex-flow: column nowrap;
      row-gap: 5.5rem;

      .p-1,
      .p-2,
      .p-3,
      .p-4 {
        width: 80%;
      }

      &__image {
        width: 70%;
      }

      .container {
        display: flex;
        flex-flow: column nowrap;
        row-gap: 1rem;
      }
    }

    .image-grid {
      display: flex;
      flex-flow: column wrap;
    }
  }
  .container {
    grid-row: 4;
    display: flex;
    flex-flow: column nowrap;
    row-gap: 8rem;
  }
}

.circle-element {
  opacity: 0.95;
  width: 350px;
  height: 350px;
  border-radius: 100%;
  position: relative;
  grid-row: 2 / span 2;
  grid-column: 2;
  align-self: flex-end;
}

.circle-1 {
  background-color: #e3eeff;
  left: 50%;
  transform: translateX(calc(-50% - 10%));
  bottom: 4rem;
  z-index: -2;
  opacity: 0.55;
}

.circle-2 {
  background-color: #f3e7e9;
  left: 50%;
  transform: translateX(calc(-50% - 5%));
  bottom: 0;
  z-index: -1;
  opacity: 0.55;
}

@media (min-width: 1024px) {
  .section-grid {
    &__content {
      .content-item {
        row-gap: 8rem;

        .p-1 {
          width: 75%;
        }
        .p-2 {
          width: 40%;
        }
        .p-3 {
          width: 50%;
        }
        .p-4 {
          width: 100%;
        }

        &__image {
          width: 350px;
        }
      }

      .image-grid {
        flex-flow: row wrap;
      }
    }
  }

  .circle-element {
    width: 550px;
    height: 550px;
    border-radius: 100%;
  }

  .circle-1 {
    left: -10%;
    transform: unset;
    bottom: -1rem;
  }

  .circle-2 {
    left: -5%;
    transform: unset;
    bottom: -1.5rem;
  }
}
</style>
