<template>
  <section class="section-grid">
    <div class="section-grid__title">
      <h1>Work Experience</h1>
    </div>
    <div class="section-grid__content">
      <div class="content-item">
        <h2>Daily UI #27</h2>
        <img
          class="content-item__image"
          src="../assets/imgs/DailyUI27.png"
          alt="Daily UI #27 Gradient picker dropdown"
        />
      </div>
      <div class="content-item">
        <h2>Daily UI #17</h2>
        <img
          class="content-item__image"
          src="../assets/imgs/DailyUI17.png"
          alt="Daily UI #27 Gradient picker dropdown"
        />
      </div>
      <div class="content-item">
        <h2>Team Project #1</h2>
        <img
          class="content-item__image"
          src="../assets/imgs/UXProject1.png"
          alt="Daily UI #27 Gradient picker dropdown"
        />
      </div>
      <div class="content-item button-area">
        <h2>SEE ALL</h2>
        <img class="content-item__arrow" src="../assets/imgs/ArrowRight.png" alt="" />
      </div>
    </div>
  </section>
</template>

<style lang="scss" scoped>
.section-grid {
  display: grid;
  grid-template-columns: 30% 1fr 10%;
  grid-template-rows: 300px auto 1fr;
  min-height: 100vh;

  &__title {
    grid-column-start: 2;
    grid-row-start: 2;

    .arrow {
      width: 100px;
    }
  }

  &__content {
    grid-column-start: 2;
    grid-row-start: 3;
    margin: 150px 0 0 0;
    display: flex;
    flex-flow: column nowrap;
    row-gap: 150px;

    .content-item {
      &__image {
        width: 300px;
        margin: 30px 0 0 0;
        box-shadow: rgba(0, 0, 0, 0.15) 0px 5px 15px 0px;
      }

      &__arrow {
        width: 100px;
      }
    }

    .button-area {
      display: flex;
      flex-flow: row nowrap;
      column-gap: 30px;
    }
  }
}
</style>
