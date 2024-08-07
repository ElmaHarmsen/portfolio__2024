<template>
  <section class="section-grid" id="daily-ui-section">
    <div class="section-grid__title">
      <h1>Daily UI</h1>
      <img class="line-image" src="../assets/imgs/daily-ui.png" alt="circle over daily ui" />
    </div>
    <div class="section-grid__content">
      <div class="content-item">
        <img
          class="content-item__image"
          src="../assets/imgs/DailyUI27.png"
          alt="Daily UI #27 Gradient picker dropdown"
        />
        <p>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit. Praesent libero mauris, hendrerit
          non dapibus aliquet, scelerisque at magna.
        </p>
      </div>
      <div class="content-item">
        <img
          class="content-item__image"
          src="../assets/imgs/DailyUI17.png"
          alt="Daily UI #27 Gradient picker dropdown"
        />
        <p>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit. Praesent libero mauris, hendrerit
          non dapibus aliquet, scelerisque at magna.
        </p>
      </div>
      <div class="content-item">
        <img
          class="content-item__image"
          src="../assets/imgs/DailyUI17.png"
          alt="Daily UI #27 Gradient picker dropdown"
        />
        <p>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit. Praesent libero mauris, hendrerit
          non dapibus aliquet, scelerisque at magna.
        </p>
      </div>
    </div>
  </section>
</template>

<style lang="scss" scoped>
.line-image {
  width: 400px;
  transform: translateX(-40px) translateY(-60px);
  position: absolute;
}

.content-item {
  &__row {
    display: flex;
    flex-flow: row nowrap;
    column-gap: 100px;
    align-items: center;
  }

  &__image {
    width: 350px;
  }
  &__description {
    height: 80px;
  }
  &__number {
    height: 80px;
  }
}
</style>
