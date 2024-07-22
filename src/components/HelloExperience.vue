<script setup>
defineProps({
  heading: {
    type: String,
    required: true
  },
  subHeading: {
    type: String,
    required: false
  }
})
</script>

<template>
  <section class="landing-grid">
    <div class="landing-msg landing-grid__messages">
      <h1 class="landing-msg__heading">{{ heading }}</h1>
      <h2>{{ subHeading }}</h2>
    </div>
    <div class="landing-grid__images">
      <img src="../assets/imgs/arrow.png" alt="" />
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
    grid-column-start: 2;
    grid-row-start: 3;
    align-self: flex-end;

    img {
      height: 100px;
    }
  }
}
</style>
