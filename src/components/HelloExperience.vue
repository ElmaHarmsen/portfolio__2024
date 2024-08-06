<template>
  <section class="landing-grid">
    <div class="landing-grid__title">
      <h1>
        Design Cases &<br />
        Work Experience
      </h1>
    </div>
    <div class="landing-grid__content">
      <div class="content-item">
        <div class="content-item__container">
          <img class="line-image" src="../assets/imgs/contact-links.png" alt="" />
          <h2>Daily UI Challenges</h2>
        </div>
        <div class="content-item__container">
          <img class="line-image" src="../assets/imgs/contact-links.png" alt="" />
          <h2>UX Team Project</h2>
        </div>
        <div class="content-item__container">
          <img class="line-image" src="../assets/imgs/contact-links.png" alt="" />
          <h2>Robot-AI Research</h2>
        </div>
      </div>
    </div>
  </section>
</template>

<style lang="scss" scoped>
.line-image {
  width: 30px;
  transform: translateX(-50px) translateY(10px);
  position: absolute;
}

.landing-grid {
  display: grid;
  grid-template-columns: 35% 1fr 5%;
  grid-template-rows: 150px auto 150px 1fr 40px;
  height: 100vh;

  &__title {
    grid-column: 2;
    grid-row-start: 2;
  }

  &__content {
    grid-column: 2;
    grid-row-start: 4;
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
