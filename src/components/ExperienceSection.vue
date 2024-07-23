<template>
  <section class="section-grid">
    <div class="section-grid__title">
      <h1>My Recent Work</h1>
      <img class="line-image" src="../assets/imgs/line-3.png" alt="" />
    </div>
    <div class="section-grid__content">
      <div class="content-item">
        <img
          class="content-item__image"
          src="../assets/imgs/DailyUI27-1.png"
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
      <router-link to="/experience">
        <div class="content-item__container">
          <h2 class="link-text">There's More To See</h2>
          <img class="long-image" src="../assets/imgs/long-line-1.png" alt="" />
        </div>
      </router-link>
    </div>
  </section>
</template>

<style lang="scss" scoped>
.line-image {
  width: 350px;
  transform: translateX(10px) translateY(25px);
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

  // &__image {
  //   box-shadow: rgba(0, 0, 0, 0.15) 0px 5px 15px 0px;
  // }

  &__arrow {
    width: 150px;
  }
}

.content-item {
  &__container {
    display: flex;
    flex-flow: column nowrap;

    .link-text {
      text-align: right;
    }

    .long-image {
      position: absolute;
      z-index: 1;
      left: 0;
      width: calc(100% - (30%));
      height: 30px;
      transform: translateY(10px);
    }
  }
}
</style>
