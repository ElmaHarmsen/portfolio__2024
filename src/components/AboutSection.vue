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
    <div class="circle-element"></div>
    <!-- <div class="circle-element-2"></div> -->
  </section>
</template>

<style lang="scss" scoped>
.circle-element {
  background: radial-gradient(ellipse at top right, #ff9a44, transparent),
    radial-gradient(circle at bottom left, #fc6076, transparent);
  opacity: 0.95;
  width: 400px;
  height: 400px;
  border-radius: 250px 300px 250px 300px;
  filter: blur(90px);
  position: relative;
  z-index: -1;
  left: 2.5rem;
  bottom: 2.5rem;
  grid-row: 2 / span 2;
  align-self: flex-end;
}

.circle-element-2 {
  background: radial-gradient(ellipse at top right, #ff9a44, transparent),
    radial-gradient(circle at bottom left, #fc6076, transparent);
  opacity: 0.95;
  width: 300px;
  height: 300px;
  border-radius: 350px 400px 350px 400px;
  filter: blur(90px);
  position: relative;
  z-index: -1;
  right: 10%;
  top: -8rem;
  grid-row: 4;
  grid-column: 2 / span 2;
  justify-self: end;
  align-self: start;
}

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
</style>
