<template>
  <section class="section-grid" id="experience-section">
    <div class="section-grid__title">
      <h1>
        Selected <br />
        Work
      </h1>
      <img
        class="line-image"
        src="../assets/imgs/recent-work.png"
        alt="squigly line under recent work"
      />
    </div>
    <div class="section-grid__content">
      <div class="content-item">
        <img
          class="content-item__image"
          src="../assets/imgs/DailyUI27.png"
          alt="Daily UI #27 Gradient picker dropdown"
        />
        <h2 class="content-item__heading">Daily UI #27</h2>
      </div>
      <div class="content-item">
        <img
          class="content-item__image"
          src="../assets/imgs/DailyUI17.png"
          alt="Daily UI #27 Gradient picker dropdown"
        />
        <h2 class="content-item__heading">Daily UI #17</h2>
      </div>
      <div class="content-item">
        <img
          class="content-item__image"
          src="../assets/imgs/DailyUI17.png"
          alt="Daily UI #27 Gradient picker dropdown"
        />
        <h2 class="content-item__heading">Daily UI #00</h2>
      </div>
    </div>
  </section>
</template>

<style lang="scss" scoped>
.line-image {
  width: 100%;
  transform: translateX(0px) translateY(-50px);
  position: relative;
}

.content-item {
  display: flex;
  flex-flow: column nowrap;
  row-gap: 30px;

  &__image {
    width: 100%;
  }

  &__heading {
    text-align: justify;
  }

  &__arrow {
    width: 150px;
  }
}

@media (min-width: 1024px) {
  .line-image {
    width: 400px;
    transform: translateX(-10px) translateY(30px);
    position: absolute;
  }

  .content-item {
    &__image {
      width: 350px;
    }
  }
}

.content-item {
  &__container {
    display: flex;
    flex-flow: column nowrap;

    .button-image {
      width: 150px;
      transform: translateX(-20px) translateY(40px);
      position: absolute;
    }
  }
}
</style>
