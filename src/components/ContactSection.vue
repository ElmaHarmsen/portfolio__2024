<template>
  <section class="section-grid" id="contact-section">
    <div class="section-grid__content">
      <h1>Say Hello</h1>
    </div>
    <div class="flex-container subitems-container">
      <div class="flex-container">
        <a href="https://www.linkedin.com/in/elma-harmsen/" target="_blank">
          <h3><span class="h2-text">LinkedIn.com/</span>elma-harmsen</h3>
        </a>
      </div>
      <span class="nav-line"></span>
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
  grid-template-rows: 8rem calc(100vh - (3 * 8rem) - 3rem) 8rem 8rem 3rem;

  &__content {
    align-self: flex-end;
    row-gap: 2.5rem;
  }

  .flex-container {
    align-self: start;
  }

  .subitems-container {
    grid-row: 4;
    grid-column: 2;
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

  .socials-container {
    grid-row: 4;
    display: flex;
    flex-flow: row nowrap;
    justify-content: start;
    column-gap: 2rem;
    padding: 0rem 0.25rem;

    &__image {
      width: 2.5rem;
    }
  }
}

@media (min-width: 1024px) {
  .section-grid {
    &__content {
      align-items: start;
    }

    .subitems-container {
      display: flex;
      flex-flow: row nowrap;
      column-gap: 1rem;
      justify-content: start;
      align-items: center;
      padding: 1.5rem;

      .nav-line {
        display: block;
      }
    }

    .socials-container {
      grid-row: 5;
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
