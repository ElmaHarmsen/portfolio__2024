<template>
  <section class="section-grid" id="about-section">
    <div class="section-grid__content">
      <div class="content-item">
        <h1>
          A Little <br />
          About Me
        </h1>
      </div>
    </div>
    <div class="section-grid__content paragraph">
      <div class="content-item">
        <p class="p-1">
          Lorem ipsum dolor sit amet, consectetur adipiscing elit. Praesent libero mauris, hendrerit
          non dapibus aliquet, scelerisque at magna. Nulla euismod est eleifend, egestas ligula sit
          amet, lobortis nulla. Nam vel urna rhoncus, ultricies ante nec, feugiat. Lorem ipsum dolor
          sit amet, consectetur adipiscing elit. Praesent libero mauris, hendrerit non dapibus
          aliquet, scelerisque at magna. <br />
        </p>
        <p class="p-2">
          Lorem ipsum dolor sit amet, consectetur adipiscing elit. Praesent libero mauris, hendrerit
          non dapibus aliquet, scelerisque at magna. Nulla euismod est eleifend, egestas ligula sit
          amet, lobortis nulla. Nam vel urna rhoncus, ultricies ante nec, feugiat. Lorem ipsum dolor
          sit amet, consectetur adipiscing elit. Praesent libero mauris, hendrerit non dapibus
          aliquet, scelerisque at magna. <br />
        </p>
        <p class="p-3">
          Lorem ipsum dolor sit amet, consectetur adipiscing elit. Praesent libero mauris, hendrerit
          non dapibus aliquet, scelerisque at magna. Nulla euismod est eleifend, egestas ligula sit
          amet, lobortis nulla. Nam vel urna rhoncus, ultricies ante nec, feugiat. Lorem ipsum dolor
          sit amet, consectetur adipiscing elit. Praesent libero mauris, hendrerit non dapibus
          aliquet, scelerisque at magna. <br />
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
  }

  .paragraph {
    grid-row: 4;
    align-self: start;
    justify-self: end;

    .content-item {
      display: flex;
      flex-flow: column nowrap;
      row-gap: 5.5rem;

      .p-1,
      .p-2,
      .p-3 {
        width: 85%;
      }
    }
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
  background: radial-gradient(circle at 50% 50%, #16a085, transparent);
  left: 50%;
  transform: translateX(calc(-50% - 10%));
  bottom: 4rem;
  filter: blur(50px);
  z-index: -2;
}

.circle-2 {
  background: radial-gradient(circle at 50% 50%, #f4d03f, transparent);
  left: 50%;
  transform: translateX(calc(-50% - 5%));
  bottom: 0;
  filter: blur(100px);
  z-index: -1;
}

@media (min-width: 1024px) {
  .section-grid {
    .paragraph {
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
      }
    }
  }

  .circle-element {
    width: 500px;
    height: 500px;
    border-radius: 100%;
    opacity: 1;
  }

  .circle-1 {
    left: -5%;
    transform: unset;
    bottom: 0;
    filter: blur(0px);
  }

  .circle-2 {
    left: -0%;
    transform: unset;
    bottom: -2.5rem;
    filter: blur(0px);
  }
}
</style>
