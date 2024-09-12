<template>
  <section class="section-grid" id="daily-ui-section">
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
        <p class="p-1">
          The Daily UI challenges are a series of 100 tasks given to design UI elements or pages.
          The Daily UI’s have been keeping my design skills sharp after my graduation from Human
          Computer Interaction earlier this year. To me, the Daily UI’s have been a true inspiration
          to experiment with different colours, interactions and explore the importance of
          accessibility when it comes to UI. <br />
        </p>
      </div>
      <div class="image-grid">
        <div class="content-item image-grid__top">
          <div class="image-container">
            <img
              class="image-container__image"
              src="../assets//imgs/DUI-search.png"
              alt="Daily UI #022 Search images of cats and dogs on Pinterest-like website"
            />
            <h2>#022 Search</h2>
          </div>
          <div class="image-container">
            <img
              class="image-container__image img-vertical"
              src="../assets/imgs/DUI-countdown.png"
              alt="Daily UI #014 music festival countdown"
            />
            <h2>#014 Countdown</h2>
          </div>
        </div>
        <div class="content-item image-grid__middle">
          <div class="image-container">
            <img
              class="image-container__image img-vertical"
              src="../assets/imgs/DUI-landing-page.png"
              alt="Daily UI #003 Landing page for book site"
            />
            <h2>#003 Landing page</h2>
          </div>
          <div class="image-container">
            <img class="image-container__image" src="../assets//imgs/DUI-music-player.png" alt="" />
            <h2>#009 Music Player</h2>
          </div>
        </div>
        <div class="content-item image-grid__bottom">
          <div class="image-container">
            <img
              class="image-container__image"
              src="../assets//imgs/DUI-calculator.png"
              alt="Daily UI #004 Calculator page"
            />
            <h2>#004 Calculation</h2>
          </div>
          <div class="image-container">
            <img
              class="image-container__image img-vertical"
              src="../assets/imgs/DUI-purchase-receipt.png"
              alt="Daily UI #17 Purchase receipt for Steam game redesign"
            />
            <h2>#024 Purchase Receipt</h2>
          </div>
        </div>
      </div>
    </div>
    <!-- <div class="circle-element circle-1"></div>
    <div class="circle-element circle-2"></div> -->
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

      .p-1 {
        width: 85%;
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
  grid-row: 2 / span 2;
  grid-column: 2;
  align-self: flex-end;
}

.circle-1 {
  background-color: #f8b500;
  left: 50%;
  transform: translateX(calc(-50% - 10%));
  bottom: 4rem;
  z-index: -2;
  opacity: 0.55;
}

.circle-2 {
  background-color: #fceabb;
  left: 50%;
  transform: translateX(calc(-50% - 5%));
  bottom: 0;
  z-index: -1;
  opacity: 0.55;
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

        .p-1 {
          width: 65%;
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
    width: 550px;
    height: 550px;
    border-radius: 100%;
  }

  .circle-1 {
    left: -10%;
    transform: unset;
    bottom: -1rem;
  }

  .circle-2 {
    left: -5%;
    transform: unset;
    bottom: -1.5rem;
  }
}
</style>
