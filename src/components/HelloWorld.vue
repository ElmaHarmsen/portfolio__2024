<script setup>
defineProps({
  heading: {
    type: String,
    required: true
  },
  subHeading: {
    type: String,
    required: true
  }
})
</script>

<template>
  <section class="landing-grid">
    <div class="landing-grid__title">
      <h1>{{ heading }}</h1>
      <h2>{{ subHeading }}</h2>
    </div>
    <div class="landing-images landing-grid__images">
      <img
        class="landing-images__figure"
        src="../assets/imgs/stickyfig.png"
        alt="hand-drawn stick figure"
      />
      <h2>Elma H.</h2>
    </div>
  </section>
</template>

<style lang="scss" scoped>
.landing-grid {
  display: grid;
  grid-template-columns: 5% 1fr 15%;
  grid-template-rows: 150px auto 1fr;
  min-height: 100vh;

  &__title {
    grid-column-start: 2;
    grid-row-start: 2;
  }

  &__images {
    grid-column-start: 2;
    grid-row-start: 3;
  }
}

.landing-images {
  display: grid;
  margin: 40px 0;

  &__arrow {
    height: 100px;
    align-self: end;
    justify-self: center;
  }
  &__figure {
    height: 350px;
    grid-column-start: 2;
  }
}
</style>
