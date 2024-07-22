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
    <div class="landing-msg landing-grid__messages">
      <h1 class="landing-msg__heading">{{ heading }}</h1>
      <h2 class="landing-msg__subHeading">{{ subHeading }}</h2>
      <h2 class="landing-msg__greeting">Elma H.</h2>
    </div>
    <div class="landing-images landing-grid__images">
      <img class="landing-images__arrow" src="../assets/imgs/arrow.png" alt="" />

      <img
        class="landing-images__figure"
        src="../assets/imgs/stickyfig.png"
        alt="hand-drawn stick figure"
      />
    </div>
  </section>
</template>

<style lang="scss" scoped>
.landing-grid {
  display: grid;
  grid-template-columns: 30% 1fr 10%;
  grid-template-rows: 20% 1fr 1fr;
  height: 100vh;

  &__messages {
    grid-column-start: 2;
    grid-row-start: 2;
  }

  &__images {
    grid-column-start: 1;
    grid-column-end: 3;
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
