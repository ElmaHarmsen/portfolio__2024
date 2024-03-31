<script setup></script>

<template>
  <main class="circled-section-container">
    <div class="circled-section-container__circle">
      <!-- note: replace border with hand-drawn circle -->
      <h1>smth smth</h1>
      <h1>smth smth smth</h1>
      <h1>smth smth</h1>
    </div>
  </main>
</template>

<style scoped lang="scss">
.circled-section-container {
  display: flex;
  flex-flow: column nowrap;
  align-items: center;
  row-gap: var(--small-gap);

  &__circle {
    display: flex;
    flex-flow: column nowrap;
    align-items: center;
    justify-content: center;
    width: 400px;
    height: 300px;
    border: 10px solid var(--base-green);
    border-radius: 50%;
  }
}
</style>
