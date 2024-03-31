<script setup></script>

<template>
  <main class="value-section-container">
    <div class="value-section-container__value">
      <img src="../assets/scribble-1.png" alt="just a scribble" class="scribble" />
      <h1>value</h1>
      <p>Lorem ipsum dolor sit amet consectetur</p>
    </div>
  </main>
</template>

<style scoped lang="scss">
.value-section-container {
  display: flex;
  flex-flow: column nowrap;
  align-items: center;

  &__value {
    display: flex;
    flex-flow: column nowrap;
    align-items: center;
    row-gap: var(--small-gap);
    width: 200px;
    text-align: center;

    .scribble {
      width: 100px;
    }
  }
}
</style>
