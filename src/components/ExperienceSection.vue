<template>
  <section class="section-grid" id="experience-section">
    <div class="section-grid__content">
      <div class="content-item">
        <h1>
          Selected <br />
          Works
        </h1>
      </div>
    </div>
    <div class="section-grid__content container">
      <div class="content-item section-nav">
        <router-link to="/experience"><h2>See all works</h2></router-link>
        <span class="nav-line"></span>
      </div>
      <div class="image-grid">
        <div class="content-item image-grid__top">
          <div class="image-container">
            <img class="image-container__image" src="../assets//imgs/unsplash-img-1.jpg" alt="" />
            <h2>Daily UI #00</h2>
          </div>
          <div class="image-container">
            <img
              class="image-container__image img-vertical"
              src="../assets/imgs/DailyUI27.png"
              alt="Daily UI #27 Gradient picker dropdown"
            />
            <h2>Daily UI #27</h2>
          </div>
        </div>
        <div class="content-item image-grid__middle">
          <div class="image-container">
            <img
              class="image-container__image img-vertical"
              src="../assets/imgs/DailyUI27.png"
              alt="Daily UI #27 Gradient picker dropdown"
            />
            <h2>Daily UI #27</h2>
          </div>
          <div class="image-container">
            <img class="image-container__image" src="../assets//imgs/unsplash-img-1.jpg" alt="" />
            <h2>Daily UI #00</h2>
          </div>
        </div>
        <div class="content-item image-grid__bottom">
          <div class="image-container">
            <img class="image-container__image" src="../assets//imgs/unsplash-img-1.jpg" alt="" />
            <h2>Daily UI #00</h2>
          </div>
          <div class="image-container">
            <img
              class="image-container__image img-vertical"
              src="../assets/imgs/DailyUI27.png"
              alt="Daily UI #27 Gradient picker dropdown"
            />
            <h2>Daily UI #27</h2>
          </div>
        </div>
      </div>
    </div>
    <div class="circle-element circle-1"></div>
    <div class="circle-element circle-2"></div>
    <div class="circle-element circle-3"></div>
  </section>
</template>

<style lang="scss" scoped>
.section-grid {
  grid-template-rows: 8rem calc(100vh - (2 * 8rem)) 8rem 1fr 8rem;

  &__content {
    align-self: flex-end;
  }

  .container {
    grid-row: 4;
    row-gap: 5.5rem;

    .section-nav {
      display: grid;
      grid-template-columns: auto 1fr;
      gap: 1rem;
      align-items: center;
      padding: 0 0.25rem;

      .nav-line {
        display: none;
        width: 100%;
        height: 0.5rem;
        background-color: black;
      }
    }

    .image-grid {
      display: flex;
      flex-flow: column nowrap;
      row-gap: 5.5rem;
      &__top,
      &__middle,
      &__bottom {
        display: grid;
        grid-template-columns: 1fr;
        grid-template-rows: 1fr;
        gap: 5.5rem;
        padding: 0 0.25rem;

        .image-container {
          display: flex;
          flex-flow: column nowrap;
          row-gap: 1rem;
          &__image {
            width: 100%;
            height: auto;
          }
          .img-vertical {
            width: 70%;
          }
        }
      }
    }
  }
}

.circle-element {
  opacity: 0.95;
  width: 350px;
  height: 350px;
  border-radius: 100%;
  position: relative;
  z-index: -1;
  grid-row: 2 / span 2;
  grid-column: 2;
  align-self: flex-end;
}

.circle-1 {
  background-color: #396afc;
  left: 50%;
  transform: translateX(calc(-50% - 10%));
  bottom: 4rem;
}

.circle-2 {
  background-color: #2948ff;
  left: 50%;
  transform: translateX(calc(-50% + 5%));
  bottom: 0;
}

.circle-3 {
  width: 300px;
  height: 300px;
  background-color: #396afc;
  left: 50%;
  transform: translateX(calc(-50% - 20%));
  bottom: -5rem;
}

@media (min-width: 1024px) {
  .nav-line {
    display: block;
    width: 100%;
    height: 0.5rem;
    background-color: black;
  }

  .section-grid {
    .container {
      row-gap: 8rem;

      .section-nav {
        display: grid;
        grid-template-columns: auto 1fr;
        gap: 1rem;
        align-items: center;
        padding: 0 0.25rem;

        .nav-line {
          display: block;
        }
      }

      .image-grid {
        row-gap: 8rem;
        &__top,
        &__middle,
        &__bottom {
          display: grid;
          grid-template-rows: 1fr;
          gap: 8rem;
          padding: 0 0.25rem;

          .image-container {
            display: flex;
            flex-flow: column nowrap;
            row-gap: 1rem;
            &__image {
              width: 100%;
              height: auto;
            }
            .img-vertical {
              width: unset;
            }
          }
        }
        &__top,
        &__bottom {
          grid-template-columns: 65% calc(100% - 8rem - 65%);
        }
        &__middle {
          grid-template-columns: calc(100% - 8rem - 65%) 65%;
        }
      }
    }
  }

  .circle-element {
    width: 600px;
    height: 600px;
    border-radius: 100%;
  }

  .circle-1 {
    left: -10%;
    transform: unset;
    bottom: 0;
    z-index: -3;
    opacity: 0.55;
  }

  .circle-2 {
    left: -1%;
    transform: unset;
    bottom: -2rem;
    z-index: -1;
    opacity: 0.55;
  }

  .circle-3 {
    width: 550px;
    height: 550px;
    left: -5%;
    transform: unset;
    bottom: -8rem;
    z-index: -2;
    opacity: 0.55;
  }
}
</style>
