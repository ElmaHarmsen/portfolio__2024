<template>
  <section class="section-grid" id="contact-section">
    <div class="section-grid__content">
      <h1>Say Hello</h1>
      <div class="subitems-container">
        <div class="flex-container">
          <h3>elmaharmsen01<span class="h2-text">@gmail.com</span></h3>
        </div>
        <span class="nav-line"></span>
      </div>
    </div>
    <div class="section-grid__content socials-container">
      <a href="https://www.linkedin.com/in/elma-harmsen/" target="_blank"
        ><img class="socials-container__image" src="../assets/imgs/linkedin.png" alt=""
      /></a>
      <a href="https://github.com/ElmaHarmsen" target="_blank"
        ><img class="socials-container__image" src="../assets/imgs/github.png" alt=""
      /></a>
    </div>
    <!--IDEA: 4 colour gradient circles spread over the viewport width-->
  </section>
</template>

<style lang="scss" scoped>
.section-grid {
  grid-template-rows: 8rem calc(100vh - (2 * 8rem)) 8rem;

  &__content {
    align-self: flex-end;
    row-gap: 2.5rem;

    .subitems-container {
      padding: 0 0.25rem;

      .h2-text {
        font-size: 20px;
        font-family: 'NotoSans-Bold';
        text-transform: uppercase;
        font-variant: small-caps;
      }

      .nav-line {
        display: none;
      }
    }
  }

  .socials-container {
    grid-row: 3;
    display: flex;
    flex-flow: row nowrap;
    justify-content: start;
    column-gap: 2rem;
    padding: 2rem 0.25rem;

    &__image {
      width: 2.5rem;
    }
  }
}

@media (min-width: 1024px) {
  .section-grid {
    &__content {
      .subitems-container {
        display: flex;
        flex-flow: row nowrap;
        column-gap: 1rem;
        justify-content: start;
        align-items: center;

        .nav-line {
          display: block;
        }
      }
    }

    .socials-container {
      justify-content: end;
      column-gap: 2.5rem;
      padding: 1.5rem 1.75rem;

      &__image {
        width: 2.5rem;
      }
    }
  }
}
</style>
