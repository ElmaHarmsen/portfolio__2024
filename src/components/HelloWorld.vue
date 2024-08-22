<template>
  <section class="landing-grid">
    <div class="landing-grid__content">
      <div class="content-item">
        <h1>Embracing Design for Humans, Robots & AI</h1>
        <div class="subitems-container">
          <h2>Elma Harmsen</h2>
          <h2>UI Designer & User Researcher</h2>
        </div>
      </div>
    </div>
    <div class="circle-element"></div>
  </section>
</template>

<style lang="scss" scoped>
// .line-image {
//   width: 700px;
//   transform: translateX(-80px) translateY(-230px);
//   position: absolute;
// }

// .landing-grid {
//   display: grid;
//   grid-template-columns: 5% 1fr 5%;
//   grid-template-rows: 200px auto 100px 1fr 100px;
//   min-height: 100vh;

//   &__title {
//     grid-column: 2;
//     grid-row-start: 3;
//   }

//   &__content {
//     grid-column: 2;
//     grid-row-start: 4;
//     width: 200px;
//     background-color: aquamarine;

//     .content-item {
//       display: flex;
//       flex-flow: column nowrap;
//       justify-content: end;
//       row-gap: 30px;
//     }
//   }
//   .image-container {
//     position: absolute;
//     right: calc(30% + 350px + 100px);
//     grid-column: 2;
//     grid-row: 3 / span 3;
//     align-self: end;
//   }
// }

@media (min-width: 1024px) {
  .circle-element {
    background: radial-gradient(ellipse at top right, #ff9a44, transparent),
      radial-gradient(circle at bottom left, #fc6076, transparent);
    opacity: 0.95;
    width: 600px;
    height: 600px;
    border-radius: 300px 400px 300px 400px;
    filter: blur(90px);
    position: absolute;
    z-index: -1;
    bottom: 1.5rem;
    left: 20%;
  }

  .landing-grid {
    display: grid;
    grid-template-columns: 10% 1fr 10%;
    grid-template-rows: 8rem 1fr 8rem;
    min-height: 100vh;

    &__content {
      grid-column: 2;
      grid-row: 2;
      width: 100%;
      display: flex;
      flex-flow: column nowrap;
      justify-content: end;
      // background-image: linear-gradient(
      //   to top,
      //   #c1dfc4 0%,
      //   #deecdd 100%
      // );
      // background: radial-gradient(ellipse at top, #e66465, transparent),
      //   radial-gradient(ellipse at bottom, #4d9f0c, transparent);
      padding: 2.5rem;

      .content-item {
        display: flex;
        flex-flow: column nowrap;
        row-gap: 2.5rem;
        justify-content: start;
        // backdrop-filter: blur(10px);
      }

      .header-container {
        display: flex;
        flex-flow: row nowrap;
        justify-content: space-between;
      }

      .subitems-container {
        display: flex;
        flex-flow: row nowrap;
        column-gap: 5rem;
        justify-content: start;
      }
    }
    .image-container {
      position: absolute;
      right: calc(30% + 350px + 100px);
      grid-column: 2;
      grid-row: 3 / span 3;
      align-self: end;
    }
  }
}
</style>
