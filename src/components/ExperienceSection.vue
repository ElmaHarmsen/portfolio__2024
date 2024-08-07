<template>
  <section class="section-grid" id="experience-section">
    <div class="section-grid__title">
      <h1>Recent Work</h1>
      <img class="line-image" src="../assets/imgs/recent-work.png" alt="" />
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
      <!-- <router-link to="/experience">
        <div class="content-item__container">
          <img class="button-image" src="../assets/imgs/see-all-work-arrow.png" alt="" />
          <h2 class="content-item__heading">See All Work</h2>
        </div>
      </router-link> -->
    </div>
  </section>
</template>

<style lang="scss" scoped>
.line-image {
  width: 350px;
  transform: translateX(110px) translateY(30px);
  position: absolute;
}

.content-item {
  display: flex;
  flex-flow: column nowrap;
  row-gap: 30px;

  &__image {
    width: 350px;
  }

  &__heading {
    text-align: justify;
  }

  &__arrow {
    width: 150px;
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
