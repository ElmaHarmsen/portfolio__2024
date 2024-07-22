<template>
  <section class="section-grid">
    <h1 class="section-grid__title">How To Contact Me</h1>
    <div class="section-grid__content">
      <div class="social-link">
        <img
          class="social-link__icon"
          src="../assets/imgs/LinkedinIcon.png"
          alt="Linkedin logo black"
        />
        <a href="https://www.linkedin.com/in/elma-harmsen/" target="_blank">
          <h2>/elma-harmsen</h2>
        </a>
      </div>
      <div class="social-link">
        <img
          class="social-link__icon"
          src="../assets/imgs/GithubIcon.png"
          alt="Linkedin logo black"
        />
        <a href="https://github.com/ElmaHarmsen" target="_blank">
          <h2>/ElmaHarmsen</h2>
        </a>
      </div>
      <div class="social-link">
        <img
          class="social-link__icon"
          src="../assets/imgs/ResumeIcon.png"
          alt="Linkedin logo black"
        />
        <h2>Resume</h2>
      </div>
      <div class="social-link">
        <img
          class="social-link__icon"
          src="../assets/imgs/EmailIcon.png"
          alt="Linkedin logo black"
        />
        <h2>elmaharmsen01@gmail.com</h2>
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
  }

  &__content {
    grid-column-start: 2;
    grid-row-start: 3;
    margin: 150px 0 30px 0;
    display: flex;
    flex-flow: column nowrap;
    row-gap: 30px;

    .social-link {
      display: flex;
      flex-flow: row nowrap;
      align-items: center;
      column-gap: 30px;

      &__icon {
        width: 40px;
        height: auto;
        border-radius: 50%;
      }
    }
  }
}
</style>
