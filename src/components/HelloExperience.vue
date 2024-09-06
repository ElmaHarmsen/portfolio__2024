<template>
  <section class="landing-grid">
    <div class="landing-grid__content">
      <div class="content-item">
        <h1 class="content-item__heading">
          Always striving for <br />
          user-centred design
        </h1>
        <div class="subitems-container">
          <h2 class="subitems-container__subheading">A selection of recent work</h2>
        </div>
      </div>
    </div>
    <div class="circle-element circle-1"></div>
    <div class="circle-element circle-2"></div>
  </section>
</template>

<style lang="scss" scoped>
// .landing-grid {
//   &__content {
//     .content-item {
//       &__heading {
//         color: var(--bg-white);
//       }
//       .subitems-container {
//         &__subheading {
//           color: var(--bg-white);
//         }
//       }
//     }
//   }
// }

.circle-element {
  width: 350px;
  height: 350px;
  border-radius: 100%;
  position: absolute;
}

.circle-1 {
  clip-path: polygon(
    30% 5%,
    50% 2%,
    67% 4%,
    80% 10%,
    91% 24%,
    95% 38%,
    97% 53%,
    96% 64%,
    94% 79%,
    86% 88%,
    77% 93%,
    65% 96%,
    52% 98%,
    38% 97%,
    22% 92%,
    10% 81%,
    3% 63%,
    2% 37%,
    10% 21%,
    17% 12%
  );
  background-color: #ff512f;
  left: 50%;
  transform: translateX(-50%);
  bottom: 15rem;
  z-index: -1;
  opacity: 0.65;
}

.circle-2 {
  clip-path: polygon(
    40% 4%,
    57% 3%,
    74% 10%,
    84% 19%,
    91% 30%,
    94% 43%,
    95% 53%,
    94% 66%,
    91% 76%,
    80% 90%,
    68% 95%,
    54% 97%,
    38% 96%,
    20% 91%,
    8% 80%,
    2% 61%,
    0 38%,
    12% 14%,
    25% 6%
  );
  background-color: #f09819;
  left: 50%;
  transform: translateX(-50%);
  bottom: 5rem;
  z-index: -2;
  opacity: 1;
}

@media (min-width: 1024px) {
  .circle-1 {
    width: 675px;
    height: 675px;
    left: 35%;
    transform: unset;
    bottom: 0rem;
  }

  .circle-2 {
    width: 700px;
    height: 700px;
    left: 38%;
    transform: unset;
    bottom: 2.5rem;
  }
}
</style>
