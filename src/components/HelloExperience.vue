<template>
  <section class="landing-grid">
    <div class="landing-grid__title">
      <h1>
        Here's My <br />
        Work Experience
      </h1>
    </div>
    <div class="landing-grid__content">
      <div class="content-item">
        <div class="content-item__container">
          <img class="long-image" src="../assets/imgs/long-line-1.png" alt="" />
          <h2>Daily UI Challenges</h2>
        </div>
        <div class="content-item__container">
          <img class="long-image" src="../assets/imgs/long-line-2.png" alt="" />
          <h2>UX Team Project</h2>
        </div>
        <div class="content-item__container">
          <img class="long-image" src="../assets/imgs/long-line-3.png" alt="" />
          <h2>Robot-AI Research</h2>
        </div>
      </div>
    </div>
  </section>
</template>

<style lang="scss" scoped>
.landing-grid {
  display: grid;
  grid-template-columns: 5% 1fr 30%;
  grid-template-rows: 150px auto 150px 1fr 40px;
  height: 100vh;

  &__title {
    grid-column: 2;
    justify-self: end;
    grid-row-start: 2;
    text-align: right;
  }

  &__content {
    grid-column: 2;
    grid-row-start: 4;
    justify-self: end;
    width: 350px;

    .content-item {
      display: flex;
      flex-flow: column nowrap;
      row-gap: 40px;
      justify-content: end;
      height: 100%;

      p {
        text-align: justify;
        background-color: var(--bg-white);
      }
    }
  }
}

.line-image {
  width: 150px;
  transform: translateX(150px) translateY(5px);
  position: absolute;
}

.content-item {
  &__container {
    display: flex;
    flex-flow: column nowrap;

    .long-image {
      position: absolute;
      z-index: 1;
      right: 0;
      width: calc(30% + 350px);
      height: 30px;
      transform: translateY(5px);
    }
  }
}
</style>
