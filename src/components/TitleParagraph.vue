<script setup>
defineProps({
  title: String,
  paragraph: String
})
</script>

<!-- prop title
prop text  -->

<template>
  <main class="title-paragraph-container">
    <h1 class="title-paragraph-container__title">{{ title }}</h1>
    <p class="title-paragraph-container__paragraph">{{ paragraph }}</p>
  </main>
</template>

<style scoped lang="scss">
.title-paragraph-container {
  display: flex;
  flex-flow: column nowrap;
  align-items: center;
  row-gap: var(--small-gap);
  &__title {
  }

  &__paragraph {
    width: 800px;
    text-align: center;
  }
}
</style>
