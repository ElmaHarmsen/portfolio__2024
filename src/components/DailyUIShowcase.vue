<template>
  <section class="section-grid">
    <div class="section-grid__title">
      <h1>Daily UI</h1>
      <img class="line-image" src="../assets/imgs/daily-ui.png" alt="" />
    </div>
    <div class="section-grid__content">
      <div class="content-item__row">
        <img
          class="content-item__image"
          src="../assets/imgs/DailyUI27-1.png"
          alt="Daily UI #27 Gradient picker dropdown"
        />
        <div class="description-wrapper">
          <img class="content-item__description" src="../assets/imgs/number.png" alt="" />
          <img class="content-item__number" src="../assets/imgs/number-27.png" alt="" />
        </div>
      </div>
      <div class="content-item__row">
        <img
          class="content-item__image"
          src="../assets/imgs/DailyUI17.png"
          alt="Daily UI #27 Gradient picker dropdown"
        />
        <div class="description-wrapper">
          <img class="content-item__description" src="../assets/imgs/number.png" alt="" />
          <img class="content-item__number" src="../assets/imgs/number-17.png" alt="" />
        </div>
      </div>
    </div>
  </section>
</template>

<style lang="scss" scoped>
.line-image {
  width: 350px;
  transform: translateX(-20px) translateY(-50px);
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
