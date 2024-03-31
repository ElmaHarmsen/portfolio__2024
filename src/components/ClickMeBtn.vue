<script setup></script>

<template>
  <main class="click-me-container">
    <div class="click-me-container__button">
      <h1 class="click-me-container__text">click me</h1>
    </div>
  </main>
</template>

<style scoped lang="scss">
.click-me-container {
  display: flex;
  flex-flow: row nowrap;
  justify-content: center;

  &__button {
    border: 10px solid var(--base-green);
    border-radius: 50%;
    padding: 1rem;
  }
}
</style>
