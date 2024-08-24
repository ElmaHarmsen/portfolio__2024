<template>
  <section class="section-grid" id="experience-section">
    <div class="section-grid__content">
      <div class="content-item">
        <h1>
          Daily UI <br />
          Challenges
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
    <div class="circle-element"></div>
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
  background: radial-gradient(ellipse at top right, #ff9a44, transparent),
    radial-gradient(circle at bottom left, #fc6076, transparent);
  opacity: 0.95;
  width: 300px;
  height: 300px;
  border-radius: 300px 300px 300px 400px;
  filter: blur(90px);
  position: relative;
  z-index: -1;
  left: -2.5rem;
  bottom: -10rem;
  grid-row: 2 / span 2;
  align-self: flex-end;
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
    background: radial-gradient(ellipse at top right, #ff9a44, transparent),
      radial-gradient(circle at bottom left, #fc6076, transparent);
    opacity: 0.95;
    width: 800px;
    height: 800px;
    border-radius: 300px 300px 300px 400px;
    filter: blur(90px);
    position: relative;
    z-index: -1;
    left: -2.5rem;
    bottom: -10rem;
    grid-row: 2 / span 2;
    align-self: flex-end;
  }
}
</style>
