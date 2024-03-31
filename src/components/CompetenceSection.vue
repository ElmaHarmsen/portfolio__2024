<script setup></script>

<template>
  <main class="competence-section-container">
    <div class="competence-section-container__competence">
      <img src="../assets/scribble-1.png" alt="just a scribble" class="scribble" />
      <h1>competence</h1>
      <p>Lorem ipsum dolor sit amet consectetur</p>
    </div>
  </main>
</template>

<style scoped lang="scss">
.competence-section-container {
  display: flex;
  flex-flow: column nowrap;
  align-items: center;

  &__competence {
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
